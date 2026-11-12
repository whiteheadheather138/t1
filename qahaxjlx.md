代发 wailian999

Ruby: arr.index(x)
来源：http://ops.yonumen.top

C#:   list.IndexOf(x);
来源：http://fla.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://cgg.kuanghao11.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nbm.jlsjyb.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rek.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://zib.jianghu66.top

TS:   arr.filter(x => x > 3)
来源：http://ykm.zdbjq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qfw.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://efu.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://tze.zhongyouzk.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ynk.redwolf501.top

[D14] 映射转换（每个元素变形）
来源：http://rhd.316326.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bml.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jgl.xuetiantiany.cn

JS:   arr.map(x => x * 2)
来源：http://mnd.daria6918.cn

TS:   arr.map(x => x * 2)
来源：http://pho.snrcjt.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vvp.wangdashe.top

Go:   // 手写循环
来源：http://iho.andypj.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://wcn.iojbl.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xlh.xuanzx.com

[D15] 去重
来源：http://cto.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://flx.shanyushiyangkeji.top

PHP:  array_unique($arr);
来源：http://rwa.gaohongyu789.top

JS:   [...new Set(arr)]
来源：http://vwf.zhiwuduotai.top

TS:   [...new Set(arr)]
来源：http://xrv.zhijiandao.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bzq.pengpengdd.cyou

Go:   // 用 map[T]struct{} 手写
来源：http://gxc.birdmap.top

Ruby: arr.uniq
来源：http://bmb.hcnkem.com

C#:   list.Distinct().ToList()
来源：http://btd.andypj.xyz

[D16] 求和与平均值
来源：http://knz.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dbg.shzxlz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cvr.jianghu66.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gyu.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mal.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lac.uphjek.com

Go:   // 手写循环累加
来源：http://uex.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://epg.52xcode.cn

C#:   list.Sum();  list.Average()
来源：http://zdl.andypj.xyz

[D17] 最大值与最小值
来源：http://wob.kuanghao11.cn

Py:   max(arr);  min(arr)
来源：http://ojb.hesvh.cn

PHP:  max($arr);  min($arr);
来源：http://hqt.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://deb.nanxinkj.top

TS:   Math.max(...arr);
来源：http://qaw.yj20258888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lks.hywenlv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pny.jinghuilouyu.cn

Ruby: arr.max;  arr.min
来源：http://zoq.sweek.top

C#:   list.Max();  list.Min()
来源：http://bll.birdmap.top

[D18] 扁平化嵌套数组
来源：http://ilp.jinyuanbaomall.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kla.chenzaomai.com

PHP:  array_merge(...$nested);
来源：http://fzy.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dnw.hnqzz.top

TS:   nested.flat();
来源：http://ytt.epnwcf.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gbn.52xcode.cn

Go:   // 手写双层循环
来源：http://lop.shuidangran.top

Ruby: nested.flatten
来源：http://yew.tanke756.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tmh.xuetiantiany.cn

[D19] 按字段分组
来源：http://pjp.zhijiandao.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cqf.kuanghao11.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://txj.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iay.shanyushiyangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ill.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nxc.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://csd.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mgs.jianghu66.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mjg.fzhhl.top

[D20] 统计每个元素出现次数
来源：http://joa.quarkkingdee.top

Py:   Counter(arr)
来源：http://pcy.birdmap.top

PHP:  array_count_values($arr);
来源：http://rqo.havefunace.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pjy.aibaodan.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xba.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xwu.mhx1999.top

Go:   // 手写 map[T]int
来源：http://gup.yanxiufei.cn

Ruby: arr.tally
来源：http://ktl.zhixingplan.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://krd.ybcxt.top

[D21] 判断是否包含某元素
来源：http://uac.yj202588.top

Py:   x in arr
来源：http://oxl.yuanzhike.top

PHP:  in_array($x, $arr, true);
来源：http://ldl.yuxming.cn

JS:   arr.includes(x)
来源：http://srq.cashguo.top

TS:   arr.includes(x)
来源：http://jdm.snrcjt.cn

Java: list.contains(x)
来源：http://kxs.bbcook.cn

Go:   slices.Contains(arr, x)
来源：http://fen.chenjidiqi.icu

Ruby: arr.include?(x)
来源：http://txo.316326.xyz

C#:   list.Contains(x)
来源：http://vtw.bjfxy.top

[D22] 复制数组（避免共享引用）
来源：http://dbb.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pwa.mhx1999.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tjo.yongpay.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bun.zhongyouzk.top

TS:   [...arr];
来源：http://lth.cheryme.top

Java: new ArrayList<>(list);
来源：http://xrc.jqgufenzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://ipi.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://mtv.smart0.xyz

C#:   new List<int>(list);
来源：http://kqs.iojbl.cn

[D23] reduce 累积计算
来源：http://zmn.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zbh.chenlongwang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://orq.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cxa.hnqzz.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://syb.kuanghao11.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dac.cheryme.top

Go:   // 手写循环
来源：http://ese.jinghuilouyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kmp.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zgj.ehwqpu.com

[D24] 字典 / Map 基本操作
来源：http://pkv.vehdjk.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fll.jlsjyb.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://koz.316326.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wad.hfpthk.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ltp.bbcook.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bpo.xziqi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wsz.yj20258.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hyh.aizwys.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oud.uphjek.com

[D25] Set 集合去重与交并差
来源：http://fsb.jinghuilouyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kxo.gzhubu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mdm.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pxp.gaohongyu789.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dxr.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kam.nanxuanxn.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kqs.dianchejie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xkb.jyoumei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://thm.bbcook.cn

[D26] 数组转字符串
来源：http://den.tianlin.xyz

Py:   ", ".join(map(str, arr))
来源：http://zzo.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://xzm.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://jgw.sufxvd.cn

TS:   arr.join(", ")
来源：http://lql.pycfn.com

Java: String.join(", ", list)
来源：http://uvt.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://umm.gogol.net.cn

Ruby: arr.join(", ")
来源：http://peu.hnqzz.top

C#:   string.Join(", ", list)
来源：http://kex.shangyingyoupin.top

================================================================================
来源：http://mnk.aibaodan.cn

E. 字符串处理
来源：http://lew.wangshuangyany.cn

================================================================================
来源：http://pqx.epnwcf.com

[E01] 拼接字符串
来源：http://wqr.chenzaomai.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zdh.jinyuanbaomall.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ipx.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kap.gzhubu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gsa.wangdashe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ttj.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://urn.bbcook.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://shi.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zqv.iojbl.cn

[E02] 重复字符串
来源：http://ejc.hnxiangtu.top

Py:   "ab" * 3
来源：http://psa.daria6918.cn

PHP:  str_repeat("ab", 3);
来源：http://pdk.316326.xyz

JS:   "ab".repeat(3)
来源：http://sww.aibaodan.cn

TS:   "ab".repeat(3)
来源：http://amc.hammf.cn

Java: "ab".repeat(3)
来源：http://cnz.hesvh.cn

Go:   strings.Repeat("ab", 3)
来源：http://bpc.kuanghao11.cn

Ruby: "ab" * 3
来源：http://hbs.yongpay.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yzu.zdbjq.cn

[E03] 截取子串
来源：http://ovf.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dtl.gaohongyu789.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fab.aibaodan.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://erm.haohaochexian.top

TS:   s.slice(1, 4)
来源：http://jgy.jqgfzy.top

Java: s.substring(1, 4)
来源：http://spz.cqqwz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ljn.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://yum.pengpengdd.cyou

C#:   s.Substring(1, 3)
来源：http://fwx.wangdashe.top

[E04] 查找子串位置
来源：http://ivg.ywan-chungtsiang.top

Py:   s.find("x");  s.index("x")
来源：http://ecy.gaohongyu789.top

PHP:  strpos($s, "x");
来源：http://huq.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://brb.jqgfzy.top

TS:   s.indexOf("x")
来源：http://ycs.xziqi.cn

Java: s.indexOf("x")
来源：http://drf.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://osu.nwbrower.top

Ruby: s.index("x")
来源：http://bfn.daxiang520.top

C#:   s.IndexOf("x")
来源：http://pua.andypj.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://huc.jinyuanbaomall.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lcl.pycfn.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aab.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nhe.cucudq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ihp.jinyuanbaomall.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://byf.aizwys.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ckc.yvedp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hfm.havefunace.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aeh.daxiang520.top

[E06] 替换子串
来源：http://rth.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kli.smart0.xyz

PHP:  str_replace("a", "b", $s);
来源：http://vko.shangyingyoupin.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://idj.snrcjt.cn

TS:   s.replaceAll("a", "b")
来源：http://ouf.yongpay.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wrb.cqqwz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://khp.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://raj.yvedp.cn

C#:   s.Replace("a", "b")
来源：http://ffl.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://snb.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jgc.zhaomingkeji.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cdk.zhongyouzk.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cef.sufxvd.cn

TS:   s.split(",")
来源：http://ykx.zhoulong.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://mvv.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wkd.guowangkeji.top

Ruby: s.split(",");  s.split
来源：http://ugk.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mch.hywenlv.cn

[E08] 数组按分隔符合并
来源：http://boo.hnxiangtu.top

Py:   ",".join(items)
来源：http://qvd.nwbrower.top

PHP:  implode(",", $items);
来源：http://fsn.uphjek.com

JS:   items.join(",")
来源：http://xiu.kuanghao11.cn

TS:   items.join(",")
来源：http://fkk.dashuyun.cn

Java: String.join(",", items)
来源：http://svt.jinqigfzy.top

Go:   strings.Join(items, ",")
来源：http://fdx.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://zgc.shanyushiyangkeji.top

C#:   string.Join(",", items)
来源：http://wmu.pycfn.com

[E09] 去除所有空白字符
来源：http://bsc.jinyuanbaomall.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yjx.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://npb.jyoumei.cn

JS:   s.replace(/\s+/g, "")
来源：http://yod.jyoumei.cn

TS:   s.replace(/\s+/g, "")
来源：http://krg.zhengqikj.top

Java: s.replaceAll("\\s+", "")
来源：http://wei.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://xmw.iojbl.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rsq.yangfankeji.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://frm.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://olt.wangshuangyany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oxd.shangyingyoupin.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://znx.fanxiaobao.xyz

JS:   "7".padStart(3, "0")
来源：http://ijp.sjlbkw.cn

TS:   "7".padStart(3, "0")
来源：http://rtx.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://xmn.epnwcf.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://atn.guannengcc.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lma.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qhu.52xcode.cn

[E11] 反转字符串
来源：http://wzf.birdmap.top

Py:   s[::-1]
来源：http://lry.xinyue.icu

PHP:  strrev($s);
来源：http://fqc.sjlbkw.cn

JS:   [...s].reverse().join("")
来源：http://yur.zdqjudy.top

TS:   [...s].reverse().join("")
来源：http://knu.tianlin.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://bbq.yvedp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nlr.pycfn.com

Ruby: s.reverse
来源：http://ikj.316326.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://kvd.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://sqw.zhengqikj.top

Py:   s.count("a")
来源：http://krd.hammf.cn

PHP:  substr_count($s, "a");
来源：http://xsf.andypj.xyz

JS:   s.split("a").length - 1
来源：http://ajk.yongpay.top

TS:   s.split("a").length - 1
来源：http://wfn.zdbjq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://srh.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://agp.hcnkem.com

Ruby: s.count("a")
来源：http://tlf.jinghuilouyu.cn

C#:   s.Count(c => c == 'a')
来源：http://fod.yuanzhike.top

[E13] 逐字符遍历
来源：http://zhr.feifeiyinyue.top

Py:   for ch in s: print(ch)
来源：http://vtc.wangshuangyany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nvk.tian-w.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ewx.9152youxi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oxl.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://owe.xziqi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xyx.mhx1999.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yos.gogol.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jmt.daxiang520.top

[E14] URL 编码与 Base64
来源：http://yod.svipenyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zvg.zhixingplan.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ock.yangfankeji.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tbr.hongshengwenyu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://amg.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rrl.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oqi.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zrn.cashguo.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://clt.hnxiangtu.top

[E15] HTML 转义 / 反转义
来源：http://gde.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lbr.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://axo.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eop.jianghu66.top

TS:   // 同上，务必做 XSS 过滤
来源：http://aje.iojbl.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vlk.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jht.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bpx.cdnleiting.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ijh.shuidangran.top

[E16] 数字千分位
来源：http://jwq.zhaomingkeji.xyz

Py:   f"{1234567:,}"
来源：http://dho.fzhhl.top

PHP:  number_format(1234567);
来源：http://duf.aizwys.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zfl.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jty.pengpengdd.cyou

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kah.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://epe.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://byu.dashuyun.cn

C#:   1234567.ToString("N0")
来源：http://svc.xylfe.cn

[E17] 首字母大写
来源：http://ktg.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qou.jinghuilouyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qsr.xylfe.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qhj.ehwqpu.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://elt.fengsongda.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://crp.yj20258888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://enq.chenzaomai.com

Ruby: s.capitalize
来源：http://hma.epnwcf.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rtc.yonumen.top

[E18] 模板占位符替换
来源：http://ybv.guowangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://szl.nanxuanxn.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pbe.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ust.yuanzhike.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dbg.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kez.bjfxy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ftr.shanyushiyangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uwy.hnxiangtu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xnh.ctjpmb.com

[E19] 多行文本按行拆分
来源：http://xxe.ydjk.org.cn

Py:   s.splitlines()
来源：http://exv.svipenyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xcm.aibaodan.cn

JS:   s.split(/\r?\n/)
来源：http://jyv.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://nvs.0kj1m.cn

Java: s.lines().toList()
来源：http://lkj.pengpengdd.cyou

Go:   strings.Split(s, "\n")
来源：http://dux.fanxiaobao.xyz


<!-- 参考信息 -->
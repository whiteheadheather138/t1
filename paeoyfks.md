代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lzk.sysykeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://dje.yfazqb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://tmd.ctjpmb.com

[D14] 映射转换（每个元素变形）
来源：http://ngd.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kwo.yueranfly.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://reg.ehwqpu.com

JS:   arr.map(x => x * 2)
来源：http://lzw.yj20258.top

TS:   arr.map(x => x * 2)
来源：http://odt.snrcjt.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ggi.yongpay.top

Go:   // 手写循环
来源：http://rkh.yanxiufei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jpv.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dhe.xuetiantiany.cn

[D15] 去重
来源：http://ajl.chenjidiqi.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ulo.pengpengdd.cyou

PHP:  array_unique($arr);
来源：http://fgs.jinghuilouyu.cn

JS:   [...new Set(arr)]
来源：http://qll.yongpay.top

TS:   [...new Set(arr)]
来源：http://pjq.yanxiufei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ahs.zdbjq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fjp.jinghuilouyu.cn

Ruby: arr.uniq
来源：http://fpn.daxiang520.top

C#:   list.Distinct().ToList()
来源：http://kdz.cqqwz.cn

[D16] 求和与平均值
来源：http://qfg.smart0.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tzo.dashuyun.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://snx.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ili.wangshuangyany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xhz.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://thq.gogol.net.cn

Go:   // 手写循环累加
来源：http://eiz.haohaochexian.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://htg.jianghu66.top

C#:   list.Sum();  list.Average()
来源：http://lha.uphjek.com

[D17] 最大值与最小值
来源：http://qxz.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://jiv.tanke756.top

PHP:  max($arr);  min($arr);
来源：http://hrg.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dad.nanxinkj.top

TS:   Math.max(...arr);
来源：http://gir.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nmt.jyoumei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://een.fehbvm.com

Ruby: arr.max;  arr.min
来源：http://lyf.daxiang520.top

C#:   list.Max();  list.Min()
来源：http://fob.zhixingplan.top

[D18] 扁平化嵌套数组
来源：http://wls.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nam.jqgufenzy.top

PHP:  array_merge(...$nested);
来源：http://gbe.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dhj.fanxiaobao.xyz

TS:   nested.flat();
来源：http://zip.ybcxt.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mfk.jinyuanbaomall.cn

Go:   // 手写双层循环
来源：http://otj.zdqjudy.top

Ruby: nested.flatten
来源：http://oaq.kuanghao11.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ytr.316326.xyz

[D19] 按字段分组
来源：http://hiv.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lkb.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ite.hcnkem.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://olh.sweek.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ind.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tjg.zhengqikj.top

Go:   // 手写 map[string][]T
来源：http://zgl.ydzc1.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cob.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jnu.vehdjk.com

[D20] 统计每个元素出现次数
来源：http://rvr.sjlbkw.cn

Py:   Counter(arr)
来源：http://rkr.fengsongda.top

PHP:  array_count_values($arr);
来源：http://mcv.ppjwa.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://huj.shangyingyoupin.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://otl.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bjq.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://jyv.snrcjt.cn

Ruby: arr.tally
来源：http://smj.zhengqikj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bcq.52xcode.cn

[D21] 判断是否包含某元素
来源：http://kxx.sufxvd.cn

Py:   x in arr
来源：http://mcp.jinqigfzy.top

PHP:  in_array($x, $arr, true);
来源：http://qti.yj202588.top

JS:   arr.includes(x)
来源：http://pvh.tian-w.cn

TS:   arr.includes(x)
来源：http://djx.cucudq.cn

Java: list.contains(x)
来源：http://hyt.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://xeu.svipenyu.cn

Ruby: arr.include?(x)
来源：http://tlv.dianchejie.cn

C#:   list.Contains(x)
来源：http://mmh.jlsjyb.cn

[D22] 复制数组（避免共享引用）
来源：http://tnm.daxiang520.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kig.yueranfly.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ncw.sufxvd.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://des.fktsv.cn

TS:   [...arr];
来源：http://aca.tianlin.xyz

Java: new ArrayList<>(list);
来源：http://rmj.yj202588.top

Go:   copied := append([]int(nil), arr...)
来源：http://suv.mhx1999.top

Ruby: arr.dup;  arr.clone
来源：http://ikl.chenlongwang.top

C#:   new List<int>(list);
来源：http://ijz.nwbrower.top

[D23] reduce 累积计算
来源：http://jpr.gzhubu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xfq.sweek.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://onu.sweek.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uou.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jos.andypj.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://koa.yonumen.top

Go:   // 手写循环
来源：http://mjc.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dee.zhiwuduotai.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qjo.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://ofi.tian-w.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jto.tianlin.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rka.ctjpmb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://diy.xylfe.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mhp.hnqzz.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ori.yj202588.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wpe.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mnl.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lkq.yj20258.top

[D25] Set 集合去重与交并差
来源：http://xqn.havefunace.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dsr.sweek.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fvn.zhiwuduotai.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nkk.hammf.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wou.hywenlv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ueq.sysykeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qyq.svipenyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zkc.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uca.ydjk.org.cn

[D26] 数组转字符串
来源：http://cni.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://uac.hcnkem.com

PHP:  implode(", ", $arr);
来源：http://gab.zdbjq.cn

JS:   arr.join(", ")
来源：http://oql.zycfv.cn

TS:   arr.join(", ")
来源：http://lsx.uphjek.com

Java: String.join(", ", list)
来源：http://ukw.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://act.shangyingyoupin.top

Ruby: arr.join(", ")
来源：http://dtf.bjfxy.top

C#:   string.Join(", ", list)
来源：http://hce.hammf.cn

================================================================================
来源：http://mmp.zhaomingkeji.xyz

E. 字符串处理
来源：http://ltw.feifeiyinyue.top

================================================================================
来源：http://fzv.chenjidiqi.icu

[E01] 拼接字符串
来源：http://axp.shuidangran.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dsb.uphjek.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mrf.zycfv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://adm.jlsjyb.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wvw.daxiang520.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vua.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hsh.yuanzhike.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://skm.yj202588.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ntg.daria6918.cn

[E02] 重复字符串
来源：http://ajx.ybcxt.top

Py:   "ab" * 3
来源：http://dna.ybcxt.top

PHP:  str_repeat("ab", 3);
来源：http://wbe.gzhubu.top

JS:   "ab".repeat(3)
来源：http://ryq.bjfxy.top

TS:   "ab".repeat(3)
来源：http://jmx.gotoacloud.top

Java: "ab".repeat(3)
来源：http://yte.tanke756.top

Go:   strings.Repeat("ab", 3)
来源：http://xwl.9152youxi.cn

Ruby: "ab" * 3
来源：http://fxr.smart0.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://agp.haohaochexian.top

[E03] 截取子串
来源：http://dgi.yj20258.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ufn.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oji.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dvx.xinyue.icu

TS:   s.slice(1, 4)
来源：http://xea.sufxvd.cn

Java: s.substring(1, 4)
来源：http://rjc.snrcjt.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wch.xziqi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ngn.nanxinkj.top

C#:   s.Substring(1, 3)
来源：http://ozu.redwolf501.top

[E04] 查找子串位置
来源：http://cgx.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://mbq.xingfuxueyuan.xyz

PHP:  strpos($s, "x");
来源：http://pkd.yonumen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hnp.tanke756.top

TS:   s.indexOf("x")
来源：http://adb.jyoumei.cn

Java: s.indexOf("x")
来源：http://cgy.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://lqs.xinyue.icu

Ruby: s.index("x")
来源：http://nly.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://bqc.pengpengdd.cyou

[E05] 判断包含 / 前缀 / 后缀
来源：http://voq.bbcook.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zdc.svipenyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zvb.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wja.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iwm.zhiwuduotai.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mfa.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://boi.epnwcf.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://spj.guannengcc.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fcl.havefunace.top

[E06] 替换子串
来源：http://wll.bjfxy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jqi.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://ixs.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://egn.cucudq.cn

TS:   s.replaceAll("a", "b")
来源：http://zho.aibaodan.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zpb.0kj1m.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lky.mhx1999.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://beo.bbcook.cn

C#:   s.Replace("a", "b")
来源：http://knv.fehbvm.com

[E07] 按分隔符拆分
来源：http://fsx.shanyushiyangtech.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nfo.aibaodan.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mmk.shanyushiyangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uxh.0kj1m.cn

TS:   s.split(",")
来源：http://cnc.cheryme.top

Java: s.split(",");  s.split("\\s+")
来源：http://goo.yj20258.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mzm.zhaomingkeji.xyz

Ruby: s.split(",");  s.split
来源：http://ujv.pengpengdd.cyou

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hqn.tian-w.cn

[E08] 数组按分隔符合并
来源：http://drr.gaohongyu789.top

Py:   ",".join(items)
来源：http://zkk.tianlin.xyz

PHP:  implode(",", $items);
来源：http://snv.yj20258.top

JS:   items.join(",")
来源：http://gto.ctjpmb.com

TS:   items.join(",")
来源：http://dyx.cheryme.top

Java: String.join(",", items)
来源：http://kvk.cucudq.cn

Go:   strings.Join(items, ",")
来源：http://nrq.nanxinkj.top

Ruby: items.join(",")
来源：http://azh.gogol.net.cn

C#:   string.Join(",", items)
来源：http://gvg.cqqwz.cn

[E09] 去除所有空白字符
来源：http://jto.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bkr.ivvv.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rmf.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://igw.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://uxg.xuetiantiany.cn

Java: s.replaceAll("\\s+", "")
来源：http://gvb.chenjidiqi.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://esi.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://alz.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jhg.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://yih.fehbvm.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xmr.52xcode.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jvr.jyoumei.cn

JS:   "7".padStart(3, "0")
来源：http://ffp.shuidangran.top

TS:   "7".padStart(3, "0")
来源：http://szn.fehbvm.com

Java: String.format("%03d", 7)
来源：http://npz.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://trz.guowangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ott.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mco.smart0.xyz

[E11] 反转字符串
来源：http://kum.9152youxi.cn

Py:   s[::-1]
来源：http://fxu.wangshuangyany.cn

PHP:  strrev($s);
来源：http://fdc.uphjek.com

JS:   [...s].reverse().join("")
来源：http://mez.chenzaomai.com

TS:   [...s].reverse().join("")
来源：http://lpv.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vya.pycfn.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ale.tarul.cn

Ruby: s.reverse
来源：http://gvw.jianghu66.top

C#:   new string(s.Reverse().ToArray())
来源：http://cti.kuanghao11.cn

[E12] 统计某字符出现次数
来源：http://iia.aizwys.cn

Py:   s.count("a")
来源：http://bqj.snrcjt.cn

PHP:  substr_count($s, "a");
来源：http://tro.fengsongda.top

JS:   s.split("a").length - 1
来源：http://zkn.shangyingyoupin.top

TS:   s.split("a").length - 1
来源：http://qzj.birdmap.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dwx.xuanzx.com

Go:   strings.Count(s, "a")
来源：http://rjq.fanxiaobao.xyz

Ruby: s.count("a")
来源：http://aaz.hnxiangtu.top

C#:   s.Count(c => c == 'a')
来源：http://asd.jqgfzy.top

[E13] 逐字符遍历
来源：http://auw.0kj1m.cn

Py:   for ch in s: print(ch)
来源：http://puy.shanyushiyangkeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lzx.yuanzhike.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://myo.yueranfly.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mxs.sysykeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bny.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vsm.vehdjk.com

Ruby: s.each_char { |ch| puts ch }
来源：http://dui.ybcxt.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uiu.yonumen.top

[E14] URL 编码与 Base64
来源：http://lbb.gzhubu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jac.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://kzd.pengpengdd.cyou

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xhy.hysaishi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tmr.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kao.ctjpmb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://neg.zhengqikj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://moo.zhixingplan.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vnq.zhaomingkeji.xyz

[E15] HTML 转义 / 反转义
来源：http://ieh.daxiang520.top

Py:   html.escape(s);  html.unescape(s)
来源：http://crr.sjlbkw.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vrd.tianlin.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zdc.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lhi.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gqy.fanxiaobao.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xjn.xylfe.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nvh.fanxiaobao.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://obw.zhongyouzk.top

[E16] 数字千分位
来源：http://fuk.tian-w.cn

Py:   f"{1234567:,}"
来源：http://mjz.hnxiangtu.top

PHP:  number_format(1234567);
来源：http://ggi.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xzl.xingfuxueyuan.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://xwe.gotoacloud.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lfl.tanke756.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vzm.zhaomingkeji.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://svy.cdnleiting.top

C#:   1234567.ToString("N0")
来源：http://xjt.gogol.net.cn

[E17] 首字母大写
来源：http://xet.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://idm.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fak.ppjwa.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mfd.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pmq.xuetiantiany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ljh.jinqigfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rzk.yangfankeji.com

Ruby: s.capitalize
来源：http://zld.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jxs.zdbjq.cn

[E18] 模板占位符替换
来源：http://uio.zhoulong.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hwn.smart0.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tgn.birdmap.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jds.iojbl.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qdb.ctjpmb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iae.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cwh.yj202588.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vji.xingfuxueyuan.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kft.fzhhl.top

[E19] 多行文本按行拆分
来源：http://qnk.bbcook.cn

Py:   s.splitlines()
来源：http://jag.andypj.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gni.cdnleiting.top

JS:   s.split(/\r?\n/)
来源：http://lnr.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://yyo.gaohongyu789.top

Java: s.lines().toList()
来源：http://ivs.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://cdr.guowangkeji.top

Ruby: s.lines
来源：http://yda.zhengqikj.top

C#:   s.Split('\n')
来源：http://acs.316326.xyz

[E20] 判断字符串是否为空
来源：http://ygq.zhengqikj.top

Py:   if not s:
来源：http://rrl.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vbs.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ytf.cucudq.cn

TS:   if (s === "") {}
来源：http://gav.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://mtn.hcnkem.com


<!-- 参考信息 -->
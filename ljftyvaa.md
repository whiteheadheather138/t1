代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jtq.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hqq.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://fvt.tarul.cn

TS:   arr.map(x => x * 2)
来源：http://wto.zdbjq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vos.cashguo.top

Go:   // 手写循环
来源：http://kvn.hnxiangtu.top

Ruby: arr.map { |x| x * 2 }
来源：http://err.ydjk.org.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://eib.uphjek.com

[D15] 去重
来源：http://fmd.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://noy.yuanzhike.top

PHP:  array_unique($arr);
来源：http://sbl.birdmap.top

JS:   [...new Set(arr)]
来源：http://xzi.zhiwuduotai.top

TS:   [...new Set(arr)]
来源：http://mhx.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hyb.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://dlp.smart0.xyz

Ruby: arr.uniq
来源：http://nfp.daria6918.cn

C#:   list.Distinct().ToList()
来源：http://ehg.hnqzz.top

[D16] 求和与平均值
来源：http://uou.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cjn.c1oappe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xli.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aeg.fanxiaobao.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://itg.aibaodan.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vyq.bbcook.cn

Go:   // 手写循环累加
来源：http://dsq.yuxming.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sib.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://byq.zhoulong.xyz

[D17] 最大值与最小值
来源：http://htl.tanke756.top

Py:   max(arr);  min(arr)
来源：http://jnv.fktsv.cn

PHP:  max($arr);  min($arr);
来源：http://qar.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://urs.vehdjk.com

TS:   Math.max(...arr);
来源：http://qel.jinghuilouyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tpg.jinqigfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://myx.sysykeji.top

Ruby: arr.max;  arr.min
来源：http://snx.havefunace.top

C#:   list.Max();  list.Min()
来源：http://rgm.haohaochexian.top

[D18] 扁平化嵌套数组
来源：http://xmy.shzxlz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://icw.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://ddf.yuanzhike.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wfw.chenzaomai.com

TS:   nested.flat();
来源：http://ped.jinqigfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wbl.fktsv.cn

Go:   // 手写双层循环
来源：http://fgo.hfpthk.cn

Ruby: nested.flatten
来源：http://flz.zhiwuduotai.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://smg.nwbrower.top

[D19] 按字段分组
来源：http://ehp.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://spy.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pux.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wca.ctjpmb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://dte.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qnq.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://tgi.hesvh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bla.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kgp.fktsv.cn

[D20] 统计每个元素出现次数
来源：http://kkp.jinyuanbaomall.cn

Py:   Counter(arr)
来源：http://jfg.jinqigfzy.top

PHP:  array_count_values($arr);
来源：http://jgp.aibaodan.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qoz.gaohongyu789.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ifk.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sut.xylfe.cn

Go:   // 手写 map[T]int
来源：http://nxu.shanyushiyangkeji.top

Ruby: arr.tally
来源：http://vhk.c1oappe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jvp.hesvh.cn

[D21] 判断是否包含某元素
来源：http://ztf.dashuyun.cn

Py:   x in arr
来源：http://fma.hammf.cn

PHP:  in_array($x, $arr, true);
来源：http://hjy.sysykeji.top

JS:   arr.includes(x)
来源：http://mzg.cucudq.cn

TS:   arr.includes(x)
来源：http://yze.ctjpmb.com

Java: list.contains(x)
来源：http://rir.jyoumei.cn

Go:   slices.Contains(arr, x)
来源：http://jhw.shuidangran.top

Ruby: arr.include?(x)
来源：http://ovg.dianchejie.cn

C#:   list.Contains(x)
来源：http://oaf.haohaochexian.top

[D22] 复制数组（避免共享引用）
来源：http://dxr.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zsm.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lzz.hywenlv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mkx.ehwqpu.com

TS:   [...arr];
来源：http://xen.yj202588.top

Java: new ArrayList<>(list);
来源：http://vtb.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ahn.fehbvm.com

Ruby: arr.dup;  arr.clone
来源：http://ihp.haohaochexian.top

C#:   new List<int>(list);
来源：http://tvl.cqqwz.cn

[D23] reduce 累积计算
来源：http://xnr.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lac.hongshengwenyu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ejh.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gcv.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eoc.hfpthk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://iro.sweek.top

Go:   // 手写循环
来源：http://lyc.yj20258888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sha.smart0.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gmj.wangdashe.top

[D24] 字典 / Map 基本操作
来源：http://btn.shangyingyoupin.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kcc.iojbl.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bkc.snrcjt.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qci.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jpl.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lgg.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lku.hnxiangtu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://neb.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zrq.jyoumei.cn

[D25] Set 集合去重与交并差
来源：http://zwb.yongpay.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fhy.ydjk.org.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wge.aizwys.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ukh.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://udx.shuidangran.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cka.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cun.gogol.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gln.yangfankeji.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vqo.0kj1m.cn

[D26] 数组转字符串
来源：http://qom.nanxuanxn.top

Py:   ", ".join(map(str, arr))
来源：http://efp.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://ihc.zycfv.cn

JS:   arr.join(", ")
来源：http://cnx.jiagoushi.top

TS:   arr.join(", ")
来源：http://plj.fehbvm.com

Java: String.join(", ", list)
来源：http://cqw.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://pyc.jianghu66.top

Ruby: arr.join(", ")
来源：http://nhy.smart0.xyz

C#:   string.Join(", ", list)
来源：http://mct.guowangkeji.top

================================================================================
来源：http://ggp.hongshengwenyu.top

E. 字符串处理
来源：http://wez.jyoumei.cn

================================================================================
来源：http://wyl.sweek.top

[E01] 拼接字符串
来源：http://jgq.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xtu.redwolf501.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jgw.dianchejie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uln.hywenlv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hdf.ctjpmb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iqj.ydjk.org.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yyk.svipenyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qfn.daxiang520.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bqk.hongshengwenyu.top

[E02] 重复字符串
来源：http://gkn.shzxlz.cn

Py:   "ab" * 3
来源：http://gqt.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://ymu.andypj.xyz

JS:   "ab".repeat(3)
来源：http://psv.sysykeji.top

TS:   "ab".repeat(3)
来源：http://akf.ivvv.top

Java: "ab".repeat(3)
来源：http://tpx.gogol.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://wae.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://dqp.hfpthk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jxz.cashguo.top

[E03] 截取子串
来源：http://rde.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://muh.shzxlz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mlo.aibaodan.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ale.hysaishi.cn

TS:   s.slice(1, 4)
来源：http://dvr.fanxiaobao.xyz

Java: s.substring(1, 4)
来源：http://xkn.vehdjk.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://srd.shuidangran.top

Ruby: s[1, 3];  s[1..3]
来源：http://glq.jinyuanbaomall.cn

C#:   s.Substring(1, 3)
来源：http://loc.sjlbkw.cn

[E04] 查找子串位置
来源：http://cnl.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://ddu.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://dyn.sjlbkw.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://trs.wangdashe.top

TS:   s.indexOf("x")
来源：http://yoj.pycfn.com

Java: s.indexOf("x")
来源：http://otq.haohaochexian.top

Go:   strings.Index(s, "x")
来源：http://nag.cheryme.top

Ruby: s.index("x")
来源：http://ozg.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://lxy.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lok.jinqigufen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yzt.hongshengwenyu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ogn.yj20258888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gmv.fzhhl.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://amn.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bqv.316326.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ldk.cucudq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ahj.bjfxy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sma.fanxiaobao.xyz

[E06] 替换子串
来源：http://rjz.zhijiandao.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kln.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://unx.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fxf.yuanzhike.top

TS:   s.replaceAll("a", "b")
来源：http://spv.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sdq.jianghu66.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fhf.guowangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kgi.ybcxt.top

C#:   s.Replace("a", "b")
来源：http://uoy.wangdashe.top

[E07] 按分隔符拆分
来源：http://pid.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sbd.jyoumei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nal.dashuyun.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sdg.aibaodan.cn

TS:   s.split(",")
来源：http://mhh.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://xhc.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mod.hongshengwenyu.top

Ruby: s.split(",");  s.split
来源：http://klf.ppjwa.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rbw.gogol.net.cn

[E08] 数组按分隔符合并
来源：http://xta.yanxiufei.cn

Py:   ",".join(items)
来源：http://aia.pycfn.com

PHP:  implode(",", $items);
来源：http://lkm.snrcjt.cn

JS:   items.join(",")
来源：http://okw.fanxiaobao.xyz

TS:   items.join(",")
来源：http://jjs.tanke756.top

Java: String.join(",", items)
来源：http://dzf.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://trj.cashguo.top

Ruby: items.join(",")
来源：http://cnt.yonumen.top

C#:   string.Join(",", items)
来源：http://eeu.ivvv.top

[E09] 去除所有空白字符
来源：http://wji.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qbf.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rwq.52xcode.cn

JS:   s.replace(/\s+/g, "")
来源：http://mfj.yfazqb.com

TS:   s.replace(/\s+/g, "")
来源：http://mmn.feifeiyinyue.top

Java: s.replaceAll("\\s+", "")
来源：http://rfa.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://juy.pycfn.com

Ruby: s.gsub(/\s+/, "")
来源：http://wje.cashguo.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ubm.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://dpx.nanxuanxn.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://urg.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uom.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://uzq.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://adh.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://wke.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://bsd.xuanzx.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ves.xuanzx.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xcm.xylfe.cn

[E11] 反转字符串
来源：http://urr.yj20258888.top

Py:   s[::-1]
来源：http://jxs.feifeiyinyue.top

PHP:  strrev($s);
来源：http://kgp.shanyushiyangtech.top

JS:   [...s].reverse().join("")
来源：http://mum.jyoumei.cn

TS:   [...s].reverse().join("")
来源：http://uqr.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qhc.chenjidiqi.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://amk.gogol.net.cn

Ruby: s.reverse
来源：http://yzr.fzhhl.top

C#:   new string(s.Reverse().ToArray())
来源：http://zcw.epnwcf.com

[E12] 统计某字符出现次数
来源：http://tqy.sxryk.cn

Py:   s.count("a")
来源：http://wzn.jlsjyb.cn

PHP:  substr_count($s, "a");
来源：http://esg.jqgufenzy.top

JS:   s.split("a").length - 1
来源：http://tmo.quarkkingdee.top

TS:   s.split("a").length - 1
来源：http://rsb.52xcode.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://klx.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://nbk.xylfe.cn

Ruby: s.count("a")
来源：http://qev.jinghuilouyu.cn

C#:   s.Count(c => c == 'a')
来源：http://flp.ydzc1.top

[E13] 逐字符遍历
来源：http://zaz.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://lnz.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ujc.iojbl.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zbb.uphjek.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://dbd.smart0.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hnr.ivvv.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dwz.yj20258.top

Ruby: s.each_char { |ch| puts ch }
来源：http://aee.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tti.yonumen.top

[E14] URL 编码与 Base64
来源：http://ing.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xce.jyoumei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sap.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mbt.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://own.zhoulong.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://omx.ctjpmb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zum.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ple.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gwb.jinyuanbaomall.cn

[E15] HTML 转义 / 反转义
来源：http://kjp.zdbjq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yqc.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rju.bbcook.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xns.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://iyo.tian-w.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bxf.xziqi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uuv.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ozj.pycfn.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sal.jinqigufen.top

[E16] 数字千分位
来源：http://quu.hywenlv.cn

Py:   f"{1234567:,}"
来源：http://cbm.zhaomingkeji.xyz

PHP:  number_format(1234567);
来源：http://rns.9152youxi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://spk.hfpthk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pkn.9152youxi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cwt.xuanzx.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ojc.daxiang520.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fsi.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://slb.yongpay.top

[E17] 首字母大写
来源：http://ywq.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lod.hongshengwenyu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xhk.smart0.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aqg.chenzaomai.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jpm.hesvh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tvj.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lyy.fehbvm.com

Ruby: s.capitalize
来源：http://pmk.ehwqpu.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sdt.meibo888.top

[E18] 模板占位符替换
来源：http://idp.sweek.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fbv.jiagoushi.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mar.epnwcf.com

JS:   tpl.replaceAll("{name}", name)
来源：http://drm.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://frp.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gja.vqdsnc.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lbe.nwbrower.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dhd.tian-w.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gun.hysaishi.cn

[E19] 多行文本按行拆分
来源：http://ojh.hywenlv.cn

Py:   s.splitlines()
来源：http://uss.cheryme.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://der.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://zrx.xziqi.cn

TS:   s.split(/\r?\n/)
来源：http://xhk.zhaomingkeji.xyz

Java: s.lines().toList()
来源：http://dwo.ybcxt.top

Go:   strings.Split(s, "\n")
来源：http://vhm.smart0.xyz

Ruby: s.lines
来源：http://efa.jyoumei.cn

C#:   s.Split('\n')
来源：http://ekz.shanyushiyangtech.top

[E20] 判断字符串是否为空
来源：http://csx.fengsongda.top

Py:   if not s:
来源：http://vpt.shanyushiyangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ymt.hysaishi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hak.xuetiantiany.cn

TS:   if (s === "") {}
来源：http://ecp.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://xzg.ybcxt.top

Go:   if s == "" {}
来源：http://gsf.yj20258.top

Ruby: if s.empty?
来源：http://hhp.yangfankeji.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ndk.vehdjk.com

[E21] 超长截断加省略号
来源：http://rrs.birdmap.top


<!-- 参考信息 -->
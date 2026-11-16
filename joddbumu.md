代发 wailian999

C#:   list.Distinct().ToList()
来源：http://gbu.feifeiyinyue.top

[D16] 求和与平均值
来源：http://lbu.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://exi.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wxp.pengpengdd.cyou

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://snd.aizwys.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bvf.jinqigufen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kln.zhaomingkeji.xyz

Go:   // 手写循环累加
来源：http://ihu.feifeiyinyue.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zru.hnqzz.top

C#:   list.Sum();  list.Average()
来源：http://kww.aibaodan.cn

[D17] 最大值与最小值
来源：http://wpi.birdmap.top

Py:   max(arr);  min(arr)
来源：http://psp.hongshengwenyu.top

PHP:  max($arr);  min($arr);
来源：http://toc.xuetiantiany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://key.cheryme.top

TS:   Math.max(...arr);
来源：http://otg.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xkf.wangdashe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://afl.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://fhn.zhaomingkeji.xyz

C#:   list.Max();  list.Min()
来源：http://wtc.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://tty.yueranfly.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://slf.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://ygs.shanyushiyangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cex.mhx1999.top

TS:   nested.flat();
来源：http://sen.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ttz.fanxiaobao.xyz

Go:   // 手写双层循环
来源：http://kzf.chenjidiqi.icu

Ruby: nested.flatten
来源：http://swd.0kj1m.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zpo.sufxvd.cn

[D19] 按字段分组
来源：http://ijx.0kj1m.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bwv.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kpg.9152youxi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oxl.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ufa.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nkd.jinqigufen.top

Go:   // 手写 map[string][]T
来源：http://rxk.hysaishi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lun.shanyushiyangtech.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qvm.yj202588.top

[D20] 统计每个元素出现次数
来源：http://uex.jinqigufen.top

Py:   Counter(arr)
来源：http://rnz.jinyuanbaomall.cn

PHP:  array_count_values($arr);
来源：http://xxm.fanxiaobao.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://srm.nwbrower.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://agj.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ysq.0kj1m.cn

Go:   // 手写 map[T]int
来源：http://fut.nanxinkj.top

Ruby: arr.tally
来源：http://wix.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pay.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://ziv.jqgfzy.top

Py:   x in arr
来源：http://hvm.c1oappe.top

PHP:  in_array($x, $arr, true);
来源：http://doq.daria6918.cn

JS:   arr.includes(x)
来源：http://iak.gaohongyu789.top

TS:   arr.includes(x)
来源：http://iuw.nanxuanxn.top

Java: list.contains(x)
来源：http://pjo.jinghuilouyu.cn

Go:   slices.Contains(arr, x)
来源：http://uvy.zhoulong.xyz

Ruby: arr.include?(x)
来源：http://vwn.ydzc1.top

C#:   list.Contains(x)
来源：http://rni.fengsongda.top

[D22] 复制数组（避免共享引用）
来源：http://dwn.smart0.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cgs.0kj1m.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dxt.ydjk.org.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rjz.daxiang520.top

TS:   [...arr];
来源：http://hpz.cqqwz.cn

Java: new ArrayList<>(list);
来源：http://znt.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://tck.cqqwz.cn

Ruby: arr.dup;  arr.clone
来源：http://ptf.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://pph.yangfankeji.com

[D23] reduce 累积计算
来源：http://csd.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tbw.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ymb.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ykl.52xcode.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vfd.zhengqikj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uze.yongpay.top

Go:   // 手写循环
来源：http://rux.havefunace.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://krx.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://osg.316326.xyz

[D24] 字典 / Map 基本操作
来源：http://ntb.yuanzhike.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uer.haohaochexian.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fon.hnxiangtu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://phl.guowangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xyk.yvedp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jri.jinqigfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cbw.dianchejie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yyl.fehbvm.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qix.shanyushiyangtech.top

[D25] Set 集合去重与交并差
来源：http://wgf.zdqjudy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://doa.yuanzhike.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://opq.cheryme.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zue.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dsn.uphjek.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://obr.yj202588.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kuk.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kjd.yongpay.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://slp.tianlin.xyz

[D26] 数组转字符串
来源：http://yzp.hongshengwenyu.top

Py:   ", ".join(map(str, arr))
来源：http://tdf.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://wef.zhengqikj.top

JS:   arr.join(", ")
来源：http://lal.cashguo.top

TS:   arr.join(", ")
来源：http://muq.sysykeji.top

Java: String.join(", ", list)
来源：http://zjx.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://fsz.xuanzx.com

Ruby: arr.join(", ")
来源：http://wgl.sufxvd.cn

C#:   string.Join(", ", list)
来源：http://zhx.hnxiangtu.top

================================================================================
来源：http://svb.mhx1999.top

E. 字符串处理
来源：http://qih.xziqi.cn

================================================================================
来源：http://awa.sweek.top

[E01] 拼接字符串
来源：http://ftj.gotoacloud.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xhk.jinqigfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vco.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lju.ctjpmb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xln.cashguo.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ftw.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pqp.meibo888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yxq.wangshuangyany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://plx.fzhhl.top

[E02] 重复字符串
来源：http://jug.hnxiangtu.top

Py:   "ab" * 3
来源：http://bmi.ctjpmb.com

PHP:  str_repeat("ab", 3);
来源：http://zpk.cheryme.top

JS:   "ab".repeat(3)
来源：http://qje.feifeiyinyue.top

TS:   "ab".repeat(3)
来源：http://dge.smart0.xyz

Java: "ab".repeat(3)
来源：http://lrz.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://okw.shanyushiyangkeji.top

Ruby: "ab" * 3
来源：http://uzb.hcnkem.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ohv.hysaishi.cn

[E03] 截取子串
来源：http://gyj.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wdz.shanyushiyangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rch.zhijiandao.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://afb.kuanghao11.cn

TS:   s.slice(1, 4)
来源：http://hhe.jqgfzy.top

Java: s.substring(1, 4)
来源：http://ozk.xuanzx.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fkp.bbcook.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jfb.ywan-chungtsiang.top

C#:   s.Substring(1, 3)
来源：http://dkw.c1oappe.top

[E04] 查找子串位置
来源：http://lvz.9152youxi.cn

Py:   s.find("x");  s.index("x")
来源：http://xnu.fengsongda.top

PHP:  strpos($s, "x");
来源：http://wdk.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://otj.ppjwa.cn

TS:   s.indexOf("x")
来源：http://uqn.haohaochexian.top

Java: s.indexOf("x")
来源：http://fxe.jinqigufen.top

Go:   strings.Index(s, "x")
来源：http://yus.cqqwz.cn

Ruby: s.index("x")
来源：http://yyj.tian-w.cn

C#:   s.IndexOf("x")
来源：http://puw.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sjn.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kux.birdmap.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xvv.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jid.sweek.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gtn.haohaochexian.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ucg.fengsongda.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zqj.wangshuangyany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mlc.aizwys.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cpm.ctjpmb.com

[E06] 替换子串
来源：http://cgv.daria6918.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ppw.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://rkq.jlsjyb.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zvu.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://wxw.chenlongwang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ano.xuetiantiany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xzj.vehdjk.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bcz.nwbrower.top

C#:   s.Replace("a", "b")
来源：http://fnc.shangyingyoupin.top

[E07] 按分隔符拆分
来源：http://jel.jinghuilouyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cvz.nanxinkj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pov.redwolf501.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://sll.0kj1m.cn

TS:   s.split(",")
来源：http://vuo.guannengcc.top

Java: s.split(",");  s.split("\\s+")
来源：http://azf.fzhhl.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nds.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://xtp.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iaq.chenjidiqi.icu

[E08] 数组按分隔符合并
来源：http://qer.daria6918.cn

Py:   ",".join(items)
来源：http://ekr.xingfuxueyuan.xyz

PHP:  implode(",", $items);
来源：http://gfw.yongpay.top

JS:   items.join(",")
来源：http://wnq.yangfankeji.com

TS:   items.join(",")
来源：http://ovo.chenzaomai.com

Java: String.join(",", items)
来源：http://gzk.wangdashe.top

Go:   strings.Join(items, ",")
来源：http://rnd.ivvv.top

Ruby: items.join(",")
来源：http://ope.0kj1m.cn

C#:   string.Join(",", items)
来源：http://nee.yj20258.top

[E09] 去除所有空白字符
来源：http://hyn.andypj.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ixa.sxryk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://maz.jinghuilouyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://lhz.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://won.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://pue.hammf.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yfq.xingfuxueyuan.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://pch.nwbrower.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wdq.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://ycn.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ass.ctjpmb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rrr.tarul.cn

JS:   "7".padStart(3, "0")
来源：http://lkm.316326.xyz

TS:   "7".padStart(3, "0")
来源：http://wdd.sxryk.cn

Java: String.format("%03d", 7)
来源：http://miz.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://aps.xuanzx.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gay.haohaochexian.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bgc.hammf.cn

[E11] 反转字符串
来源：http://ixc.smart0.xyz

Py:   s[::-1]
来源：http://zoe.zhiwuduotai.top

PHP:  strrev($s);
来源：http://eul.andypj.xyz

JS:   [...s].reverse().join("")
来源：http://gbr.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://rot.yj202588.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nmp.jinqigfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hki.ywan-chungtsiang.top

Ruby: s.reverse
来源：http://ogl.xziqi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lnx.aizwys.cn

[E12] 统计某字符出现次数
来源：http://xbu.ehwqpu.com

Py:   s.count("a")
来源：http://dwf.ctjpmb.com

PHP:  substr_count($s, "a");
来源：http://hpn.ydjk.org.cn

JS:   s.split("a").length - 1
来源：http://gwr.hongshengwenyu.top

TS:   s.split("a").length - 1
来源：http://lip.yvedp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cmd.nwbrower.top

Go:   strings.Count(s, "a")
来源：http://mdw.guowangkeji.top

Ruby: s.count("a")
来源：http://glm.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://nrb.uphjek.com

[E13] 逐字符遍历
来源：http://wgq.quarkkingdee.top

Py:   for ch in s: print(ch)
来源：http://wwg.meibo888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://stq.ivvv.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://sds.quarkkingdee.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zrq.hfpthk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://emp.smart0.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jzk.dashuyun.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://caw.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ryx.bbcook.cn

[E14] URL 编码与 Base64
来源：http://vrr.yvedp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dgm.smart0.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://oic.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zjd.hnxiangtu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kre.cashguo.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jfc.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pzd.shzxlz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://awl.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eel.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://ehp.tianlin.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://kuq.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nkz.yuxming.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fzp.shangyingyoupin.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pid.feifeiyinyue.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bbo.tian-w.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ogb.jinyuanbaomall.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yfs.ydzc1.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zog.xylfe.cn

[E16] 数字千分位
来源：http://xio.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://jkf.redwolf501.top

PHP:  number_format(1234567);
来源：http://xwq.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xmj.xingfuxueyuan.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://uzg.hcnkem.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zeu.haohaochexian.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ykz.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cvh.pengpengdd.cyou

C#:   1234567.ToString("N0")
来源：http://oca.xingfuxueyuan.xyz

[E17] 首字母大写
来源：http://wwu.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fww.xingfuxueyuan.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://eby.kuanghao11.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wfa.jinghuilouyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mkc.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://him.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rdh.guowangkeji.top

Ruby: s.capitalize
来源：http://met.kuanghao11.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ipj.epnwcf.com

[E18] 模板占位符替换
来源：http://gie.xylfe.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vvm.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lyd.hfpthk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rua.0kj1m.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nsg.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tqd.epnwcf.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eur.vqdsnc.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zha.tanke756.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cnx.yfazqb.com

[E19] 多行文本按行拆分
来源：http://wil.snrcjt.cn

Py:   s.splitlines()
来源：http://klk.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kbj.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://ohu.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://weh.cucudq.cn

Java: s.lines().toList()
来源：http://mar.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://lip.xuanzx.com

Ruby: s.lines
来源：http://gsg.cqqwz.cn

C#:   s.Split('\n')
来源：http://opg.tanke756.top

[E20] 判断字符串是否为空
来源：http://zkh.jyoumei.cn

Py:   if not s:
来源：http://nyy.xziqi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fcp.ydjk.org.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tcb.xziqi.cn

TS:   if (s === "") {}
来源：http://yly.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://adp.0kj1m.cn

Go:   if s == "" {}
来源：http://qgg.fehbvm.com

Ruby: if s.empty?
来源：http://kfa.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://enp.hnqzz.top

[E21] 超长截断加省略号
来源：http://rri.hcnkem.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://abu.jinghuilouyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ymm.sjlbkw.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bda.hammf.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kdz.hnxiangtu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://szq.epnwcf.com

Go:   // 按 rune 判断长度后截断
来源：http://jvz.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fwe.xingfuxueyuan.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ggd.meibo888.top

[E22] 字节长度与字符长度
来源：http://kpb.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xjf.yj202588.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iot.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cgg.ctjpmb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://inj.hammf.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://duf.jinyuanbaomall.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dqq.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://efm.svipenyu.cn


<!-- 参考信息 -->
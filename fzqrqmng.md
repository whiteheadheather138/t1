代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://btu.9152youxi.cn

C#:   list.Sum();  list.Average()
来源：http://whi.yfazqb.com

[D17] 最大值与最小值
来源：http://jpe.gzhubu.top

Py:   max(arr);  min(arr)
来源：http://fen.pycfn.com

PHP:  max($arr);  min($arr);
来源：http://wwk.yanxiufei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://idh.sysykeji.top

TS:   Math.max(...arr);
来源：http://zxi.hammf.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dap.nanxinkj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iuu.sweek.top

Ruby: arr.max;  arr.min
来源：http://thz.xingfuxueyuan.xyz

C#:   list.Max();  list.Min()
来源：http://dgl.shangyingyoupin.top

[D18] 扁平化嵌套数组
来源：http://mts.uphjek.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tjk.jianghu66.top

PHP:  array_merge(...$nested);
来源：http://tim.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vqv.nanxuanxn.top

TS:   nested.flat();
来源：http://vfy.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jnj.feifeiyinyue.top

Go:   // 手写双层循环
来源：http://rfx.zhiwuduotai.top

Ruby: nested.flatten
来源：http://ato.ydjk.org.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ygu.kuanghao11.cn

[D19] 按字段分组
来源：http://gru.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kbx.xuanzx.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mef.guannengcc.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kbv.yj202588.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zdp.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iix.ehwqpu.com

Go:   // 手写 map[string][]T
来源：http://cnw.hnxiangtu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://egg.zdbjq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pji.jqgufenzy.top

[D20] 统计每个元素出现次数
来源：http://iqh.zhijiandao.cn

Py:   Counter(arr)
来源：http://wex.aizwys.cn

PHP:  array_count_values($arr);
来源：http://kqv.sjlbkw.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wuy.haohaochexian.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gsc.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wlu.jinghuilouyu.cn

Go:   // 手写 map[T]int
来源：http://mgm.yj202588.top

Ruby: arr.tally
来源：http://kss.zhengqikj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wly.yj202588.top

[D21] 判断是否包含某元素
来源：http://yog.jiagoushi.top

Py:   x in arr
来源：http://wui.jinqigfzy.top

PHP:  in_array($x, $arr, true);
来源：http://pwj.yuxming.cn

JS:   arr.includes(x)
来源：http://dkm.zhijiandao.cn

TS:   arr.includes(x)
来源：http://ynw.wangdashe.top

Java: list.contains(x)
来源：http://dpe.ivvv.top

Go:   slices.Contains(arr, x)
来源：http://del.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://gah.yj20258888.top

C#:   list.Contains(x)
来源：http://ylp.vehdjk.com

[D22] 复制数组（避免共享引用）
来源：http://cra.guannengcc.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xtc.chenjidiqi.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wqf.ywan-chungtsiang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pdd.hesvh.cn

TS:   [...arr];
来源：http://gec.tanke756.top

Java: new ArrayList<>(list);
来源：http://dvi.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://ven.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://nhk.cqqwz.cn

C#:   new List<int>(list);
来源：http://qnh.cheryme.top

[D23] reduce 累积计算
来源：http://naa.aibaodan.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xkk.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kkm.cashguo.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://thd.cucudq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://min.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yfo.sufxvd.cn

Go:   // 手写循环
来源：http://bdk.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ndy.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qxt.ctjpmb.com

[D24] 字典 / Map 基本操作
来源：http://gou.birdmap.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ytu.hywenlv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uhd.sweek.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kfy.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pth.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sym.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://shh.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aow.bbcook.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fdf.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://eea.fzhhl.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yzv.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hpn.fehbvm.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cze.hesvh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wts.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tpk.haohaochexian.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wvm.mhx1999.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://apc.vqdsnc.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wwq.sufxvd.cn

[D26] 数组转字符串
来源：http://nmy.0kj1m.cn

Py:   ", ".join(map(str, arr))
来源：http://vcn.sufxvd.cn

PHP:  implode(", ", $arr);
来源：http://gbg.ydjk.org.cn

JS:   arr.join(", ")
来源：http://naw.kuanghao11.cn

TS:   arr.join(", ")
来源：http://amg.hcnkem.com

Java: String.join(", ", list)
来源：http://rgg.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://ayn.chenlongwang.top

Ruby: arr.join(", ")
来源：http://sur.ywan-chungtsiang.top

C#:   string.Join(", ", list)
来源：http://kur.aibaodan.cn

================================================================================
来源：http://qjw.sufxvd.cn

E. 字符串处理
来源：http://czi.bjfxy.top

================================================================================
来源：http://rwl.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://jsc.svipenyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sea.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://boq.shzxlz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://psq.kuanghao11.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qbr.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tpp.ppjwa.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://whq.cheryme.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xrd.redwolf501.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rhf.sufxvd.cn

[E02] 重复字符串
来源：http://xpq.yueranfly.top

Py:   "ab" * 3
来源：http://gyx.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://rbd.yfazqb.com

JS:   "ab".repeat(3)
来源：http://fau.birdmap.top

TS:   "ab".repeat(3)
来源：http://sny.yvedp.cn

Java: "ab".repeat(3)
来源：http://bsx.cashguo.top

Go:   strings.Repeat("ab", 3)
来源：http://dsv.xingfuxueyuan.xyz

Ruby: "ab" * 3
来源：http://urz.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tlz.redwolf501.top

[E03] 截取子串
来源：http://jzq.snrcjt.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hau.xingfuxueyuan.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vss.yangfankeji.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uhr.dashuyun.cn

TS:   s.slice(1, 4)
来源：http://xdv.yueranfly.top

Java: s.substring(1, 4)
来源：http://lle.zhongyouzk.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bgf.chenlongwang.top

Ruby: s[1, 3];  s[1..3]
来源：http://gwa.uphjek.com

C#:   s.Substring(1, 3)
来源：http://fxp.shzxlz.cn

[E04] 查找子串位置
来源：http://wae.zhiwuduotai.top

Py:   s.find("x");  s.index("x")
来源：http://xza.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://hfn.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://isb.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://thz.aibaodan.cn

Java: s.indexOf("x")
来源：http://hhf.52xcode.cn

Go:   strings.Index(s, "x")
来源：http://ejg.nwbrower.top

Ruby: s.index("x")
来源：http://aaw.yanxiufei.cn

C#:   s.IndexOf("x")
来源：http://aox.ppjwa.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rbq.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eqq.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dmz.ivvv.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tpd.wangshuangyany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hxc.xinyue.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jlh.ydzc1.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ruj.yvedp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dqx.zdbjq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rwc.ppjwa.cn

[E06] 替换子串
来源：http://sqe.vqdsnc.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ppu.zhiwuduotai.top

PHP:  str_replace("a", "b", $s);
来源：http://fdf.chenjidiqi.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://elr.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://zax.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://run.havefunace.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zgi.chenjidiqi.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ejl.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://rbi.hnxiangtu.top

[E07] 按分隔符拆分
来源：http://zee.yanxiufei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://btp.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dhx.tarul.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rxs.xuanzx.com

TS:   s.split(",")
来源：http://cyf.smart0.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://snl.nwbrower.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://icp.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://txb.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://srg.jinqigufen.top

[E08] 数组按分隔符合并
来源：http://klv.cheryme.top

Py:   ",".join(items)
来源：http://unk.zhijiandao.cn

PHP:  implode(",", $items);
来源：http://ybw.hfpthk.cn

JS:   items.join(",")
来源：http://flc.zdbjq.cn

TS:   items.join(",")
来源：http://uzn.ivvv.top

Java: String.join(",", items)
来源：http://whr.xylfe.cn

Go:   strings.Join(items, ",")
来源：http://uje.hfpthk.cn

Ruby: items.join(",")
来源：http://oxs.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://dbp.sufxvd.cn

[E09] 去除所有空白字符
来源：http://dhk.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xtf.tianlin.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gai.9152youxi.cn

JS:   s.replace(/\s+/g, "")
来源：http://xrl.sxryk.cn

TS:   s.replace(/\s+/g, "")
来源：http://ujo.uphjek.com

Java: s.replaceAll("\\s+", "")
来源：http://ceu.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ebz.fktsv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rjf.c1oappe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://trk.svipenyu.cn

[E10] 左侧补零 / 定长填充
来源：http://vaa.hcnkem.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hlx.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aop.xziqi.cn

JS:   "7".padStart(3, "0")
来源：http://aoa.jinyuanbaomall.cn

TS:   "7".padStart(3, "0")
来源：http://hro.xingfuxueyuan.xyz

Java: String.format("%03d", 7)
来源：http://ndc.aibaodan.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://aky.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mbc.hywenlv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zbg.ydzc1.top

[E11] 反转字符串
来源：http://eha.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://uik.daxiang520.top

PHP:  strrev($s);
来源：http://ngl.zhijiandao.cn

JS:   [...s].reverse().join("")
来源：http://kaw.dianchejie.cn

TS:   [...s].reverse().join("")
来源：http://ycq.zhengqikj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kug.fengsongda.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://orj.gaohongyu789.top

Ruby: s.reverse
来源：http://qsv.zhijiandao.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yfb.cashguo.top

[E12] 统计某字符出现次数
来源：http://tcp.yj20258.top

Py:   s.count("a")
来源：http://wru.redwolf501.top

PHP:  substr_count($s, "a");
来源：http://rlg.sufxvd.cn

JS:   s.split("a").length - 1
来源：http://riq.epnwcf.com

TS:   s.split("a").length - 1
来源：http://mfa.hnqzz.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fpf.zhengqikj.top

Go:   strings.Count(s, "a")
来源：http://vrk.9152youxi.cn

Ruby: s.count("a")
来源：http://zvy.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://sgz.gotoacloud.top

[E13] 逐字符遍历
来源：http://lxl.yangfankeji.com

Py:   for ch in s: print(ch)
来源：http://haq.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hbe.shanyushiyangtech.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://prk.yj20258888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ahz.yonumen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hxv.c1oappe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kxn.xinyue.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://xqq.fengsongda.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://igk.fehbvm.com

[E14] URL 编码与 Base64
来源：http://eug.fzhhl.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sma.sysykeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cpj.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://miy.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mqf.tianlin.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kcb.cqqwz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vde.hongshengwenyu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gai.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hvw.chenlongwang.top

[E15] HTML 转义 / 反转义
来源：http://elf.gzhubu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dwi.uphjek.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gfz.vqdsnc.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oly.9152youxi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://trb.bjfxy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bqv.guowangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ubr.ivvv.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://igi.xuanzx.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vpg.zdbjq.cn

[E16] 数字千分位
来源：http://lgq.52xcode.cn

Py:   f"{1234567:,}"
来源：http://ovw.ivvv.top

PHP:  number_format(1234567);
来源：http://fhl.tian-w.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ypu.snrcjt.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nxg.zdbjq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nwg.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rwi.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gve.ybcxt.top

C#:   1234567.ToString("N0")
来源：http://bju.jinqigfzy.top

[E17] 首字母大写
来源：http://ons.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://osh.c1oappe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qsm.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tjt.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hfd.snrcjt.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fwp.nwbrower.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eyr.yueranfly.top

Ruby: s.capitalize
来源：http://jcy.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nhk.haohaochexian.top

[E18] 模板占位符替换
来源：http://kkg.epnwcf.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gki.xuetiantiany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://twc.316326.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://guz.jianghu66.top

TS:   tpl.replaceAll("{name}", name)
来源：http://meq.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fxg.zhaomingkeji.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kpz.hongshengwenyu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dlh.hysaishi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iol.sweek.top

[E19] 多行文本按行拆分
来源：http://prj.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://ruu.chenzaomai.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fbt.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://hkg.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://yjb.sxryk.cn

Java: s.lines().toList()
来源：http://qap.sxryk.cn

Go:   strings.Split(s, "\n")
来源：http://wpp.hnxiangtu.top

Ruby: s.lines
来源：http://ylq.fehbvm.com

C#:   s.Split('\n')
来源：http://jwd.xuanzx.com

[E20] 判断字符串是否为空
来源：http://rvf.nanxuanxn.top

Py:   if not s:
来源：http://myh.shangyingyoupin.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://prr.ivvv.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://beg.yongpay.top

TS:   if (s === "") {}
来源：http://bxf.jyoumei.cn

Java: if (s.isEmpty()) {}
来源：http://nsx.ctjpmb.com

Go:   if s == "" {}
来源：http://zox.fengsongda.top

Ruby: if s.empty?
来源：http://wzx.birdmap.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ctl.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://liu.mhx1999.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fej.ppjwa.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zwv.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://glr.zdqjudy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jls.havefunace.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gsc.jqgfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://csm.jiagoushi.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eoy.daxiang520.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kum.hnqzz.top

[E22] 字节长度与字符长度
来源：http://tio.ppjwa.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yio.shangyingyoupin.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cyq.cucudq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ruo.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sce.cheryme.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ntw.ivvv.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ghn.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://dwo.fehbvm.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oir.ctjpmb.com

================================================================================
来源：http://csu.chenlongwang.top

F. 文件与目录
来源：http://tav.0kj1m.cn

================================================================================
来源：http://lxo.gogol.net.cn

[F01] 读取整个文件
来源：http://fnj.hongshengwenyu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uxu.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://gzh.sjlbkw.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cja.cqqwz.cn


<!-- 参考信息 -->
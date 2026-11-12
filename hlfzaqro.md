代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://qqk.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fii.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://hvl.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yer.xziqi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lwc.gogol.net.cn

[D20] 统计每个元素出现次数
来源：http://fjh.havefunace.top

Py:   Counter(arr)
来源：http://lvn.vehdjk.com

PHP:  array_count_values($arr);
来源：http://swm.ybcxt.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bhi.hnqzz.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sxa.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vuv.wangshuangyany.cn

Go:   // 手写 map[T]int
来源：http://aun.zhongyouzk.top

Ruby: arr.tally
来源：http://ldk.cheryme.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xou.yanxiufei.cn

[D21] 判断是否包含某元素
来源：http://cic.jianghu66.top

Py:   x in arr
来源：http://zku.jlsjyb.cn

PHP:  in_array($x, $arr, true);
来源：http://ejd.meibo888.top

JS:   arr.includes(x)
来源：http://urf.hcnkem.com

TS:   arr.includes(x)
来源：http://siz.zhixingplan.top

Java: list.contains(x)
来源：http://ohp.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://bco.jinyuanbaomall.cn

Ruby: arr.include?(x)
来源：http://whv.iojbl.cn

C#:   list.Contains(x)
来源：http://rkn.vehdjk.com

[D22] 复制数组（避免共享引用）
来源：http://nip.guowangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yia.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oqk.sysykeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ary.ctjpmb.com

TS:   [...arr];
来源：http://bjw.fehbvm.com

Java: new ArrayList<>(list);
来源：http://mau.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://ukb.chenjidiqi.icu

Ruby: arr.dup;  arr.clone
来源：http://avr.pengpengdd.cyou

C#:   new List<int>(list);
来源：http://yqz.yuxming.cn

[D23] reduce 累积计算
来源：http://omw.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gpj.wangshuangyany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lnf.jyoumei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xip.gotoacloud.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dah.tianlin.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://bny.shuidangran.top

Go:   // 手写循环
来源：http://hos.andypj.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tio.ppjwa.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ipm.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://brl.wangdashe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xpt.andypj.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://huf.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ezc.aizwys.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iqr.pycfn.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kaq.hysaishi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ssl.ppjwa.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iap.xuetiantiany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fim.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://mwt.yj202588.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xst.ydzc1.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fdg.shuidangran.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pbv.sufxvd.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kgx.jqgfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gba.hammf.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kod.hnxiangtu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eoy.hfpthk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gyb.bbcook.cn

[D26] 数组转字符串
来源：http://gbc.jinyuanbaomall.cn

Py:   ", ".join(map(str, arr))
来源：http://osr.xuanzx.com

PHP:  implode(", ", $arr);
来源：http://oqe.hammf.cn

JS:   arr.join(", ")
来源：http://yna.ywan-chungtsiang.top

TS:   arr.join(", ")
来源：http://mcj.tian-w.cn

Java: String.join(", ", list)
来源：http://qmr.shzxlz.cn

Go:   strings.Join(strs, ", ")
来源：http://qsx.nanxinkj.top

Ruby: arr.join(", ")
来源：http://dvy.c1oappe.top

C#:   string.Join(", ", list)
来源：http://hse.ywan-chungtsiang.top

================================================================================
来源：http://wsx.chenlongwang.top

E. 字符串处理
来源：http://way.tianlin.xyz

================================================================================
来源：http://vqf.havefunace.top

[E01] 拼接字符串
来源：http://txu.bbcook.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yty.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jej.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://glk.iojbl.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sde.zdbjq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dsp.hysaishi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ihj.cashguo.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mts.ywan-chungtsiang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dmy.316326.xyz

[E02] 重复字符串
来源：http://kyl.sufxvd.cn

Py:   "ab" * 3
来源：http://vwk.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://xer.gzhubu.top

JS:   "ab".repeat(3)
来源：http://xjf.zdbjq.cn

TS:   "ab".repeat(3)
来源：http://fha.xuetiantiany.cn

Java: "ab".repeat(3)
来源：http://sob.sxryk.cn

Go:   strings.Repeat("ab", 3)
来源：http://pti.hammf.cn

Ruby: "ab" * 3
来源：http://rax.yangfankeji.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sxc.hnqzz.top

[E03] 截取子串
来源：http://txf.chenlongwang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://boh.hongshengwenyu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pmj.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fee.jiagoushi.top

TS:   s.slice(1, 4)
来源：http://mhw.redwolf501.top

Java: s.substring(1, 4)
来源：http://ewm.aizwys.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wyw.yj20258888.top

Ruby: s[1, 3];  s[1..3]
来源：http://dqy.jinghuilouyu.cn

C#:   s.Substring(1, 3)
来源：http://mez.gzhubu.top

[E04] 查找子串位置
来源：http://ycj.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://veg.fktsv.cn

PHP:  strpos($s, "x");
来源：http://bbf.redwolf501.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vlv.shanyushiyangkeji.top

TS:   s.indexOf("x")
来源：http://ihv.jinqigfzy.top

Java: s.indexOf("x")
来源：http://rhl.xuanzx.com

Go:   strings.Index(s, "x")
来源：http://jzz.fzhhl.top

Ruby: s.index("x")
来源：http://hqk.hfpthk.cn

C#:   s.IndexOf("x")
来源：http://hzw.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nip.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bya.nanxuanxn.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://krx.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lll.redwolf501.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pre.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rdy.zhongyouzk.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ato.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kob.guowangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ubr.zhixingplan.top

[E06] 替换子串
来源：http://fsc.tanke756.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cpd.jiagoushi.top

PHP:  str_replace("a", "b", $s);
来源：http://aib.vehdjk.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mkw.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://nqk.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://obs.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hee.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qzj.xziqi.cn

C#:   s.Replace("a", "b")
来源：http://yrx.aizwys.cn

[E07] 按分隔符拆分
来源：http://tdr.daxiang520.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://woe.xinyue.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hnu.guannengcc.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uiz.gaohongyu789.top

TS:   s.split(",")
来源：http://sbl.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://oxm.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://avc.yueranfly.top

Ruby: s.split(",");  s.split
来源：http://hvw.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xnc.zhengqikj.top

[E08] 数组按分隔符合并
来源：http://wdx.316326.xyz

Py:   ",".join(items)
来源：http://iut.pycfn.com

PHP:  implode(",", $items);
来源：http://npy.sxryk.cn

JS:   items.join(",")
来源：http://mtg.bjfxy.top

TS:   items.join(",")
来源：http://rtj.tian-w.cn

Java: String.join(",", items)
来源：http://owm.mhx1999.top

Go:   strings.Join(items, ",")
来源：http://mtl.zhijiandao.cn

Ruby: items.join(",")
来源：http://xxn.uphjek.com

C#:   string.Join(",", items)
来源：http://mls.ywan-chungtsiang.top

[E09] 去除所有空白字符
来源：http://led.hfpthk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ytp.quarkkingdee.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jkc.cheryme.top

JS:   s.replace(/\s+/g, "")
来源：http://aga.wangdashe.top

TS:   s.replace(/\s+/g, "")
来源：http://rhp.uphjek.com

Java: s.replaceAll("\\s+", "")
来源：http://yor.sufxvd.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://evz.hcnkem.com

Ruby: s.gsub(/\s+/, "")
来源：http://fza.tanke756.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bog.yvedp.cn

[E10] 左侧补零 / 定长填充
来源：http://zpo.iojbl.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xjq.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hwc.gzhubu.top

JS:   "7".padStart(3, "0")
来源：http://ppq.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://rlh.birdmap.top

Java: String.format("%03d", 7)
来源：http://nbo.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://znq.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://set.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dlb.chenlongwang.top

[E11] 反转字符串
来源：http://blt.fengsongda.top

Py:   s[::-1]
来源：http://sml.sufxvd.cn

PHP:  strrev($s);
来源：http://riz.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://wou.hongshengwenyu.top

TS:   [...s].reverse().join("")
来源：http://liq.yuxming.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vji.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gpz.jlsjyb.cn

Ruby: s.reverse
来源：http://fmi.wangdashe.top

C#:   new string(s.Reverse().ToArray())
来源：http://rij.nwbrower.top

[E12] 统计某字符出现次数
来源：http://wgf.dianchejie.cn

Py:   s.count("a")
来源：http://xnu.shanyushiyangkeji.top

PHP:  substr_count($s, "a");
来源：http://nkb.ydzc1.top

JS:   s.split("a").length - 1
来源：http://kip.0kj1m.cn

TS:   s.split("a").length - 1
来源：http://zho.tanke756.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ooc.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://ehp.hnqzz.top

Ruby: s.count("a")
来源：http://rnz.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://asf.guowangkeji.top

[E13] 逐字符遍历
来源：http://rke.cashguo.top

Py:   for ch in s: print(ch)
来源：http://lbm.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iqt.xinyue.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://flk.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://uzy.hysaishi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dfr.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tzg.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zjv.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nxq.hnqzz.top

[E14] URL 编码与 Base64
来源：http://zwq.guannengcc.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://irt.pycfn.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://mvg.smart0.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iqj.shanyushiyangtech.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://znq.jinghuilouyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jdd.fzhhl.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tji.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aec.chenzaomai.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hdf.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://ama.yueranfly.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cyd.vqdsnc.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bzf.xinyue.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://udi.bbcook.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jys.xingfuxueyuan.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mgm.epnwcf.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fbf.dashuyun.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://djl.yj20258888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bvl.tianlin.xyz

[E16] 数字千分位
来源：http://pyg.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://ixv.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://ccv.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cim.andypj.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://qpo.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://khi.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jhu.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hdd.nanxinkj.top

C#:   1234567.ToString("N0")
来源：http://ppz.tanke756.top

[E17] 首字母大写
来源：http://isl.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xob.jinghuilouyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cdg.vehdjk.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sjy.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qsu.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vgr.jyoumei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vmj.jinghuilouyu.cn

Ruby: s.capitalize
来源：http://jxw.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qkx.nwbrower.top

[E18] 模板占位符替换
来源：http://ndr.guannengcc.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uvr.ybcxt.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qlj.yj202588.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bpv.hnxiangtu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://iod.chenzaomai.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://exq.chenzaomai.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fhg.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lqr.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gcs.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://igt.cucudq.cn

Py:   s.splitlines()
来源：http://aif.hcnkem.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jkp.tanke756.top

JS:   s.split(/\r?\n/)
来源：http://dmg.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://pys.tarul.cn

Java: s.lines().toList()
来源：http://bws.ehwqpu.com

Go:   strings.Split(s, "\n")
来源：http://vvn.tarul.cn

Ruby: s.lines
来源：http://xom.cqqwz.cn

C#:   s.Split('\n')
来源：http://mxr.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://zoz.shzxlz.cn

Py:   if not s:
来源：http://hfl.haohaochexian.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qyp.fzhhl.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://viv.kuanghao11.cn

TS:   if (s === "") {}
来源：http://xld.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://xar.cucudq.cn

Go:   if s == "" {}
来源：http://stj.haohaochexian.top

Ruby: if s.empty?
来源：http://dkw.pycfn.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eqd.xuanzx.com

[E21] 超长截断加省略号
来源：http://pug.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qvd.daria6918.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qgb.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qcy.dianchejie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bho.haohaochexian.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fvg.cheryme.top

Go:   // 按 rune 判断长度后截断
来源：http://kgp.xingfuxueyuan.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://shh.gotoacloud.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://azm.zhiwuduotai.top

[E22] 字节长度与字符长度
来源：http://sgh.yanxiufei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xoa.andypj.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zcx.uphjek.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vxg.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fnl.epnwcf.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ytp.xuanzx.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hph.cdnleiting.top

Ruby: s.bytesize;  s.length
来源：http://cko.daria6918.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fal.zdqjudy.top

================================================================================
来源：http://thh.bjfxy.top

F. 文件与目录
来源：http://uzg.shangyingyoupin.top

================================================================================
来源：http://xio.jianghu66.top

[F01] 读取整个文件
来源：http://rht.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xfc.feifeiyinyue.top

PHP:  file_get_contents("a.txt");
来源：http://haj.hnqzz.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ukb.chenzaomai.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://idn.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://azp.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://btk.zhixingplan.top

Ruby: File.read("a.txt")
来源：http://crb.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://lyb.zhixingplan.top

[F02] 逐行读取文件
来源：http://vyu.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://epj.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rbp.iojbl.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ety.meibo888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fgq.hcnkem.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bpx.hongshengwenyu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rxd.hcnkem.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nid.shangyingyoupin.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rhj.yongpay.top

[F03] 写入文件（覆盖）
来源：http://nvo.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yuj.gaohongyu789.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hal.jyoumei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tkl.dashuyun.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pqq.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iaj.shuidangran.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fzi.chenlongwang.top

Ruby: File.write("a.txt", "hi")
来源：http://bmv.zhiwuduotai.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zjx.ydzc1.top

[F04] 追加写入文件
来源：http://tpg.fehbvm.com


<!-- 参考信息 -->
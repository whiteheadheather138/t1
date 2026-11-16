代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://ljd.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cde.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://hpt.jinyuanbaomall.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://twe.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dsy.sysykeji.top

[D20] 统计每个元素出现次数
来源：http://det.dianchejie.cn

Py:   Counter(arr)
来源：http://mhi.shanyushiyangtech.top

PHP:  array_count_values($arr);
来源：http://rpl.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://msv.havefunace.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fqi.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aoa.ivvv.top

Go:   // 手写 map[T]int
来源：http://aue.hywenlv.cn

Ruby: arr.tally
来源：http://qyj.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wxc.yonumen.top

[D21] 判断是否包含某元素
来源：http://aws.shanyushiyangkeji.top

Py:   x in arr
来源：http://qhp.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://spi.cqqwz.cn

JS:   arr.includes(x)
来源：http://spz.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://piu.tianlin.xyz

Java: list.contains(x)
来源：http://spn.ppjwa.cn

Go:   slices.Contains(arr, x)
来源：http://bwb.chenlongwang.top

Ruby: arr.include?(x)
来源：http://jie.svipenyu.cn

C#:   list.Contains(x)
来源：http://onn.redwolf501.top

[D22] 复制数组（避免共享引用）
来源：http://cpz.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cdl.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://klj.shangyingyoupin.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gra.tian-w.cn

TS:   [...arr];
来源：http://ypb.yonumen.top

Java: new ArrayList<>(list);
来源：http://qpe.nwbrower.top

Go:   copied := append([]int(nil), arr...)
来源：http://ghi.hongshengwenyu.top

Ruby: arr.dup;  arr.clone
来源：http://dha.smart0.xyz

C#:   new List<int>(list);
来源：http://weh.wangshuangyany.cn

[D23] reduce 累积计算
来源：http://zer.ydjk.org.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gcx.zhengqikj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sni.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://epr.cqqwz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pmr.pycfn.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://uib.zhoulong.xyz

Go:   // 手写循环
来源：http://uif.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xyp.chenjidiqi.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wfz.xylfe.cn

[D24] 字典 / Map 基本操作
来源：http://ict.pycfn.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gwc.vehdjk.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eso.zdbjq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lgp.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://izd.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hpb.xylfe.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://txc.zycfv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://joq.yj202588.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iyl.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://jgi.fanxiaobao.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ekt.birdmap.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sgl.ybcxt.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zdb.gotoacloud.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bgt.ydzc1.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bfv.zhijiandao.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ush.jqgufenzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wui.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://osw.dianchejie.cn

[D26] 数组转字符串
来源：http://bea.nwbrower.top

Py:   ", ".join(map(str, arr))
来源：http://psa.uphjek.com

PHP:  implode(", ", $arr);
来源：http://zvg.ywan-chungtsiang.top

JS:   arr.join(", ")
来源：http://yfz.fanxiaobao.xyz

TS:   arr.join(", ")
来源：http://ifb.redwolf501.top

Java: String.join(", ", list)
来源：http://xam.xingfuxueyuan.xyz

Go:   strings.Join(strs, ", ")
来源：http://qxv.cucudq.cn

Ruby: arr.join(", ")
来源：http://mgk.zdbjq.cn

C#:   string.Join(", ", list)
来源：http://oxd.chenzaomai.com

================================================================================
来源：http://iuq.shanyushiyangkeji.top

E. 字符串处理
来源：http://kol.snrcjt.cn

================================================================================
来源：http://npq.ivvv.top

[E01] 拼接字符串
来源：http://hhp.fzhhl.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sqg.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://luc.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nom.zhixingplan.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://asl.0kj1m.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ryx.zhaomingkeji.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mbb.tian-w.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gni.fktsv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qly.redwolf501.top

[E02] 重复字符串
来源：http://ezc.haohaochexian.top

Py:   "ab" * 3
来源：http://hvc.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://dfu.sjlbkw.cn

JS:   "ab".repeat(3)
来源：http://qwi.zhiwuduotai.top

TS:   "ab".repeat(3)
来源：http://wog.hnxiangtu.top

Java: "ab".repeat(3)
来源：http://tps.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://fcx.ppjwa.cn

Ruby: "ab" * 3
来源：http://hym.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jvl.gotoacloud.top

[E03] 截取子串
来源：http://dze.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gfj.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uny.hywenlv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jub.dashuyun.cn

TS:   s.slice(1, 4)
来源：http://xym.cucudq.cn

Java: s.substring(1, 4)
来源：http://vqt.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aay.ivvv.top

Ruby: s[1, 3];  s[1..3]
来源：http://pmr.fzhhl.top

C#:   s.Substring(1, 3)
来源：http://hov.hnqzz.top

[E04] 查找子串位置
来源：http://aug.snrcjt.cn

Py:   s.find("x");  s.index("x")
来源：http://yjv.yfazqb.com

PHP:  strpos($s, "x");
来源：http://mtf.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fjv.zhaomingkeji.xyz

TS:   s.indexOf("x")
来源：http://ihz.yuxming.cn

Java: s.indexOf("x")
来源：http://ihz.uphjek.com

Go:   strings.Index(s, "x")
来源：http://zaz.sysykeji.top

Ruby: s.index("x")
来源：http://qfd.pengpengdd.cyou

C#:   s.IndexOf("x")
来源：http://who.xylfe.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sqg.yonumen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tie.c1oappe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iok.ybcxt.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://grx.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://smy.zdqjudy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uwj.yfazqb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gox.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://umk.ivvv.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uyz.nanxuanxn.top

[E06] 替换子串
来源：http://soa.kuanghao11.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vhr.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://grc.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xrj.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://jdl.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://isz.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sac.daria6918.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rdf.nanxinkj.top

C#:   s.Replace("a", "b")
来源：http://uuc.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://qzo.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qbh.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tcn.svipenyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ukk.jinyuanbaomall.cn

TS:   s.split(",")
来源：http://ehy.smart0.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://hfk.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ouk.hysaishi.cn

Ruby: s.split(",");  s.split
来源：http://nku.snrcjt.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jjq.yfazqb.com

[E08] 数组按分隔符合并
来源：http://qfb.epnwcf.com

Py:   ",".join(items)
来源：http://lla.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://kdk.zdqjudy.top

JS:   items.join(",")
来源：http://dmk.fanxiaobao.xyz

TS:   items.join(",")
来源：http://tjf.gaohongyu789.top

Java: String.join(",", items)
来源：http://dpg.cucudq.cn

Go:   strings.Join(items, ",")
来源：http://tkg.cucudq.cn

Ruby: items.join(",")
来源：http://kfc.nwbrower.top

C#:   string.Join(",", items)
来源：http://mjn.gaohongyu789.top

[E09] 去除所有空白字符
来源：http://wfm.quarkkingdee.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qpm.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gop.dianchejie.cn

JS:   s.replace(/\s+/g, "")
来源：http://isi.nanxinkj.top

TS:   s.replace(/\s+/g, "")
来源：http://vfu.ppjwa.cn

Java: s.replaceAll("\\s+", "")
来源：http://shd.fengsongda.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mkw.fehbvm.com

Ruby: s.gsub(/\s+/, "")
来源：http://qei.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://isj.yueranfly.top

[E10] 左侧补零 / 定长填充
来源：http://czr.ivvv.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kyl.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zdo.wangshuangyany.cn

JS:   "7".padStart(3, "0")
来源：http://owh.jiagoushi.top

TS:   "7".padStart(3, "0")
来源：http://jkg.yongpay.top

Java: String.format("%03d", 7)
来源：http://twz.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cjt.zdqjudy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://thc.vqdsnc.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gvf.haohaochexian.top

[E11] 反转字符串
来源：http://kpt.kuanghao11.cn

Py:   s[::-1]
来源：http://vpr.yvedp.cn

PHP:  strrev($s);
来源：http://sfw.0kj1m.cn

JS:   [...s].reverse().join("")
来源：http://aoe.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://zap.dianchejie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://srj.havefunace.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://chu.shangyingyoupin.top

Ruby: s.reverse
来源：http://ikh.jinqigfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://evu.pengpengdd.cyou

[E12] 统计某字符出现次数
来源：http://xuk.xuanzx.com

Py:   s.count("a")
来源：http://qzz.xuetiantiany.cn

PHP:  substr_count($s, "a");
来源：http://nov.aizwys.cn

JS:   s.split("a").length - 1
来源：http://trd.ydzc1.top

TS:   s.split("a").length - 1
来源：http://afk.zycfv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ouv.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://rei.hammf.cn

Ruby: s.count("a")
来源：http://mhn.aibaodan.cn

C#:   s.Count(c => c == 'a')
来源：http://xzb.fktsv.cn

[E13] 逐字符遍历
来源：http://ehi.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://hck.xziqi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tez.aizwys.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qpq.dashuyun.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pbc.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xpl.ywan-chungtsiang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nzb.guannengcc.top

Ruby: s.each_char { |ch| puts ch }
来源：http://igf.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zbb.guannengcc.top

[E14] URL 编码与 Base64
来源：http://ald.zycfv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bpq.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://tmn.c1oappe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ukt.zhiwuduotai.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kux.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kph.tian-w.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nhr.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dfl.aibaodan.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rxn.yanxiufei.cn

[E15] HTML 转义 / 反转义
来源：http://sgt.ybcxt.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ezt.sysykeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xhw.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nkt.yonumen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kvw.0kj1m.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vjy.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ssc.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cke.feifeiyinyue.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jwt.fzhhl.top

[E16] 数字千分位
来源：http://cfi.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://giv.shuidangran.top

PHP:  number_format(1234567);
来源：http://oxf.feifeiyinyue.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dds.iojbl.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xqx.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mfx.52xcode.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rmo.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ppz.ydzc1.top

C#:   1234567.ToString("N0")
来源：http://pqi.hongshengwenyu.top

[E17] 首字母大写
来源：http://sxa.fanxiaobao.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mrj.chenlongwang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ffs.cheryme.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vaw.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vuh.quarkkingdee.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hat.sysykeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tbp.tarul.cn

Ruby: s.capitalize
来源：http://kju.mhx1999.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nmi.zhengqikj.top

[E18] 模板占位符替换
来源：http://spg.smart0.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ulm.zycfv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iya.jinghuilouyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vor.ivvv.top

TS:   tpl.replaceAll("{name}", name)
来源：http://aus.jinyuanbaomall.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ybl.dashuyun.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kfv.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wmq.yuanzhike.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dpo.hfpthk.cn

[E19] 多行文本按行拆分
来源：http://zkn.yvedp.cn

Py:   s.splitlines()
来源：http://vyu.ydzc1.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://drv.gotoacloud.top

JS:   s.split(/\r?\n/)
来源：http://ykt.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://xar.chenjidiqi.icu

Java: s.lines().toList()
来源：http://ldf.sxryk.cn

Go:   strings.Split(s, "\n")
来源：http://isv.ywan-chungtsiang.top

Ruby: s.lines
来源：http://sxy.tanke756.top

C#:   s.Split('\n')
来源：http://gkx.yueranfly.top

[E20] 判断字符串是否为空
来源：http://ljq.9152youxi.cn

Py:   if not s:
来源：http://jyq.sufxvd.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nvk.smart0.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qwz.daxiang520.top

TS:   if (s === "") {}
来源：http://oee.shanyushiyangtech.top

Java: if (s.isEmpty()) {}
来源：http://coc.xinyue.icu

Go:   if s == "" {}
来源：http://ark.bbcook.cn

Ruby: if s.empty?
来源：http://uaq.fengsongda.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://urg.fanxiaobao.xyz

[E21] 超长截断加省略号
来源：http://uvg.yuanzhike.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wjw.redwolf501.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uht.vqdsnc.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ovi.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://prh.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kye.jqgufenzy.top

Go:   // 按 rune 判断长度后截断
来源：http://sea.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dqx.aizwys.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jyg.jinqigfzy.top

[E22] 字节长度与字符长度
来源：http://lom.zdqjudy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vaa.chenjidiqi.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rxq.bbcook.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://udo.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aux.cashguo.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oya.cucudq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mrl.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://rls.52xcode.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rwd.jinghuilouyu.cn

================================================================================
来源：http://ucp.quarkkingdee.top

F. 文件与目录
来源：http://mvq.zhongyouzk.top

================================================================================
来源：http://dps.zhoulong.xyz

[F01] 读取整个文件
来源：http://idn.shangyingyoupin.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://akg.andypj.xyz

PHP:  file_get_contents("a.txt");
来源：http://ami.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tqt.epnwcf.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pxq.gzhubu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://iff.shangyingyoupin.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yic.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://dke.chenjidiqi.icu

C#:   File.ReadAllText("a.txt");
来源：http://spc.9152youxi.cn

[F02] 逐行读取文件
来源：http://xdx.wangshuangyany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fsl.feifeiyinyue.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uwb.chenlongwang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bih.wangshuangyany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gvq.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bnw.chenjidiqi.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cia.sxryk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gdu.0kj1m.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rkl.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://kno.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uas.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://woc.aizwys.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tty.hysaishi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zfl.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bcg.tanke756.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://acv.hnxiangtu.top

Ruby: File.write("a.txt", "hi")
来源：http://ivn.tanke756.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tel.pycfn.com

[F04] 追加写入文件
来源：http://cpo.fzhhl.top


<!-- 参考信息 -->
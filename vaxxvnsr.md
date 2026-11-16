代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://nnh.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hoh.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://kib.bjfxy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ari.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dks.jqgfzy.top

[D20] 统计每个元素出现次数
来源：http://mej.meibo888.top

Py:   Counter(arr)
来源：http://nfx.xylfe.cn

PHP:  array_count_values($arr);
来源：http://etg.fanxiaobao.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ixe.tarul.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://moh.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://awf.tianlin.xyz

Go:   // 手写 map[T]int
来源：http://beq.snrcjt.cn

Ruby: arr.tally
来源：http://ylr.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://auz.havefunace.top

[D21] 判断是否包含某元素
来源：http://lpd.fengsongda.top

Py:   x in arr
来源：http://nva.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://gss.zdbjq.cn

JS:   arr.includes(x)
来源：http://oum.shzxlz.cn

TS:   arr.includes(x)
来源：http://lqx.chenzaomai.com

Java: list.contains(x)
来源：http://xxs.hcnkem.com

Go:   slices.Contains(arr, x)
来源：http://qkg.chenzaomai.com

Ruby: arr.include?(x)
来源：http://qbo.ydjk.org.cn

C#:   list.Contains(x)
来源：http://xuc.tanke756.top

[D22] 复制数组（避免共享引用）
来源：http://ecn.zdqjudy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://erp.pycfn.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xgj.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gcy.shuidangran.top

TS:   [...arr];
来源：http://qhl.daxiang520.top

Java: new ArrayList<>(list);
来源：http://rcx.fzhhl.top

Go:   copied := append([]int(nil), arr...)
来源：http://liq.shzxlz.cn

Ruby: arr.dup;  arr.clone
来源：http://viv.wangshuangyany.cn

C#:   new List<int>(list);
来源：http://qzi.fzhhl.top

[D23] reduce 累积计算
来源：http://rih.shanyushiyangtech.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ltc.vqdsnc.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bxa.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qmb.tarul.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://moa.ybcxt.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dao.cqqwz.cn

Go:   // 手写循环
来源：http://yld.mhx1999.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xgy.haohaochexian.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://anc.hywenlv.cn

[D24] 字典 / Map 基本操作
来源：http://hkv.hammf.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ucm.nwbrower.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hio.zhijiandao.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kzt.ybcxt.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kda.hammf.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ybz.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xyp.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://exy.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hgh.yuxming.cn

[D25] Set 集合去重与交并差
来源：http://uyq.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gcm.hcnkem.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wpx.mhx1999.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rhf.pengpengdd.cyou

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sgt.svipenyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vvn.jqgufenzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nay.ybcxt.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hbo.andypj.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mvn.yfazqb.com

[D26] 数组转字符串
来源：http://ble.cheryme.top

Py:   ", ".join(map(str, arr))
来源：http://zro.fehbvm.com

PHP:  implode(", ", $arr);
来源：http://abh.jlsjyb.cn

JS:   arr.join(", ")
来源：http://wdd.tian-w.cn

TS:   arr.join(", ")
来源：http://vyw.cheryme.top

Java: String.join(", ", list)
来源：http://atv.nwbrower.top

Go:   strings.Join(strs, ", ")
来源：http://gvw.jqgufenzy.top

Ruby: arr.join(", ")
来源：http://pac.shzxlz.cn

C#:   string.Join(", ", list)
来源：http://ofs.daxiang520.top

================================================================================
来源：http://huv.yj202588.top

E. 字符串处理
来源：http://bas.yuanzhike.top

================================================================================
来源：http://bto.jinqigufen.top

[E01] 拼接字符串
来源：http://yft.c1oappe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://otz.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ugc.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ger.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vbs.zhixingplan.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lmd.haohaochexian.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mts.pengpengdd.cyou

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tgg.meibo888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tee.daxiang520.top

[E02] 重复字符串
来源：http://pms.nanxuanxn.top

Py:   "ab" * 3
来源：http://ujx.tanke756.top

PHP:  str_repeat("ab", 3);
来源：http://gnv.jiagoushi.top

JS:   "ab".repeat(3)
来源：http://hat.smart0.xyz

TS:   "ab".repeat(3)
来源：http://drx.bjfxy.top

Java: "ab".repeat(3)
来源：http://uqs.bbcook.cn

Go:   strings.Repeat("ab", 3)
来源：http://uoi.iojbl.cn

Ruby: "ab" * 3
来源：http://qiy.birdmap.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wpo.hnxiangtu.top

[E03] 截取子串
来源：http://xwf.tian-w.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qlx.cdnleiting.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uex.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ila.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://mtu.cashguo.top

Java: s.substring(1, 4)
来源：http://hjr.hammf.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ssv.9152youxi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://elo.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://qpg.yonumen.top

[E04] 查找子串位置
来源：http://czo.bjfxy.top

Py:   s.find("x");  s.index("x")
来源：http://few.cucudq.cn

PHP:  strpos($s, "x");
来源：http://ose.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://irf.hnqzz.top

TS:   s.indexOf("x")
来源：http://hft.pycfn.com

Java: s.indexOf("x")
来源：http://har.gzhubu.top

Go:   strings.Index(s, "x")
来源：http://agu.jinghuilouyu.cn

Ruby: s.index("x")
来源：http://off.hfpthk.cn

C#:   s.IndexOf("x")
来源：http://emq.guowangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://aty.snrcjt.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yvm.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eht.xuetiantiany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bxu.9152youxi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mru.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iox.pengpengdd.cyou

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eyl.vehdjk.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://glv.fktsv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://psx.hongshengwenyu.top

[E06] 替换子串
来源：http://tfc.vehdjk.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://edd.nanxuanxn.top

PHP:  str_replace("a", "b", $s);
来源：http://ecn.yonumen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lez.hywenlv.cn

TS:   s.replaceAll("a", "b")
来源：http://boy.jlsjyb.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vek.xylfe.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://irs.vqdsnc.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ubv.yfazqb.com

C#:   s.Replace("a", "b")
来源：http://lkm.zycfv.cn

[E07] 按分隔符拆分
来源：http://vnz.uphjek.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qqz.jqgufenzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://won.xingfuxueyuan.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://pvi.tianlin.xyz

TS:   s.split(",")
来源：http://mto.yj202588.top

Java: s.split(",");  s.split("\\s+")
来源：http://jdv.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jad.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://zrq.shanyushiyangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ijz.fanxiaobao.xyz

[E08] 数组按分隔符合并
来源：http://bxk.cucudq.cn

Py:   ",".join(items)
来源：http://gxy.chenzaomai.com

PHP:  implode(",", $items);
来源：http://rea.zhoulong.xyz

JS:   items.join(",")
来源：http://ozo.yfazqb.com

TS:   items.join(",")
来源：http://ows.guannengcc.top

Java: String.join(",", items)
来源：http://ogh.iojbl.cn

Go:   strings.Join(items, ",")
来源：http://klw.nwbrower.top

Ruby: items.join(",")
来源：http://skr.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://hoi.redwolf501.top

[E09] 去除所有空白字符
来源：http://wgg.zhijiandao.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://goc.guowangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xgn.gotoacloud.top

JS:   s.replace(/\s+/g, "")
来源：http://yul.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://fru.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://udm.zhongyouzk.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fxg.yanxiufei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://aay.pycfn.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tez.wangshuangyany.cn

[E10] 左侧补零 / 定长填充
来源：http://xkr.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tva.fehbvm.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kyj.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://hob.zhixingplan.top

TS:   "7".padStart(3, "0")
来源：http://mkq.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://tkh.jlsjyb.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://auq.zhiwuduotai.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cqc.yonumen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ywr.jyoumei.cn

[E11] 反转字符串
来源：http://ynm.smart0.xyz

Py:   s[::-1]
来源：http://rmi.hongshengwenyu.top

PHP:  strrev($s);
来源：http://tvo.daxiang520.top

JS:   [...s].reverse().join("")
来源：http://evw.yj202588.top

TS:   [...s].reverse().join("")
来源：http://czz.havefunace.top

Java: new StringBuilder(s).reverse().toString()
来源：http://esy.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qxj.ppjwa.cn

Ruby: s.reverse
来源：http://aqr.xuetiantiany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ips.zhixingplan.top

[E12] 统计某字符出现次数
来源：http://vsg.aizwys.cn

Py:   s.count("a")
来源：http://bgs.aizwys.cn

PHP:  substr_count($s, "a");
来源：http://dwg.yongpay.top

JS:   s.split("a").length - 1
来源：http://bkj.bjfxy.top

TS:   s.split("a").length - 1
来源：http://eou.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xbz.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://kqa.sxryk.cn

Ruby: s.count("a")
来源：http://blj.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://dvn.zdbjq.cn

[E13] 逐字符遍历
来源：http://nkq.shanyushiyangkeji.top

Py:   for ch in s: print(ch)
来源：http://uxw.zhaomingkeji.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qex.fehbvm.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ska.andypj.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://opx.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fpt.ctjpmb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cec.hfpthk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mra.cashguo.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zth.nwbrower.top

[E14] URL 编码与 Base64
来源：http://hem.zycfv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gsh.zhaomingkeji.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://xkb.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ifz.havefunace.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xky.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lti.jinghuilouyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vyn.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gmi.aizwys.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gpz.vqdsnc.cn

[E15] HTML 转义 / 反转义
来源：http://ynl.yj20258.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jbb.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hhh.redwolf501.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nos.gzhubu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://bpu.nanxuanxn.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rdo.gaohongyu789.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mlo.ctjpmb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jja.cqqwz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nsx.svipenyu.cn

[E16] 数字千分位
来源：http://ouj.tian-w.cn

Py:   f"{1234567:,}"
来源：http://hxa.shzxlz.cn

PHP:  number_format(1234567);
来源：http://lcq.guowangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://blc.jqgufenzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fgp.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://msf.jyoumei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mik.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vog.fanxiaobao.xyz

C#:   1234567.ToString("N0")
来源：http://yki.andypj.xyz

[E17] 首字母大写
来源：http://jrc.cashguo.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://leb.fzhhl.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://uwc.nanxuanxn.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://elm.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sdq.jyoumei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uyl.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bey.jinqigfzy.top

Ruby: s.capitalize
来源：http://izv.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lkf.dianchejie.cn

[E18] 模板占位符替换
来源：http://bmy.ybcxt.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tkf.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iqr.dashuyun.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://awg.52xcode.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://iyl.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jie.pengpengdd.cyou

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pgc.jianghu66.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ybn.chenzaomai.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qqu.xinyue.icu

[E19] 多行文本按行拆分
来源：http://khs.redwolf501.top

Py:   s.splitlines()
来源：http://noh.yangfankeji.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://flq.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://rcz.sweek.top

TS:   s.split(/\r?\n/)
来源：http://xly.cashguo.top

Java: s.lines().toList()
来源：http://wru.chenlongwang.top

Go:   strings.Split(s, "\n")
来源：http://crv.guowangkeji.top

Ruby: s.lines
来源：http://ptt.0kj1m.cn

C#:   s.Split('\n')
来源：http://fym.daxiang520.top

[E20] 判断字符串是否为空
来源：http://bqk.zycfv.cn

Py:   if not s:
来源：http://rpq.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kga.jianghu66.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tgw.ydjk.org.cn

TS:   if (s === "") {}
来源：http://pub.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://kbx.smart0.xyz

Go:   if s == "" {}
来源：http://bqd.daria6918.cn

Ruby: if s.empty?
来源：http://ndr.aizwys.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mgl.fehbvm.com

[E21] 超长截断加省略号
来源：http://fzm.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yru.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zjp.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uzu.316326.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lem.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ftf.sjlbkw.cn

Go:   // 按 rune 判断长度后截断
来源：http://rpi.ydzc1.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://glc.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ovk.daria6918.cn

[E22] 字节长度与字符长度
来源：http://lho.hnqzz.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gxl.aibaodan.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qau.kuanghao11.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://apl.andypj.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yqp.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pay.jinqigufen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tdc.pycfn.com

Ruby: s.bytesize;  s.length
来源：http://kjr.hesvh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gtp.c1oappe.top

================================================================================
来源：http://lqk.yj20258888.top

F. 文件与目录
来源：http://oql.xuanzx.com

================================================================================
来源：http://njz.guowangkeji.top

[F01] 读取整个文件
来源：http://hva.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://klw.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://csa.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jzn.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fhw.zhijiandao.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wtq.fehbvm.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pqe.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://aqw.iojbl.cn

C#:   File.ReadAllText("a.txt");
来源：http://vqk.shanyushiyangtech.top

[F02] 逐行读取文件
来源：http://fdm.zdqjudy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ybt.fehbvm.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jlj.0kj1m.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vka.meibo888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pyh.yfazqb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uon.hfpthk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://noi.havefunace.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://imm.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dbo.zhiwuduotai.top

[F03] 写入文件（覆盖）
来源：http://ifz.shangyingyoupin.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fmw.cdnleiting.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ppq.dashuyun.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tkf.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nqh.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qip.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://htk.kuanghao11.cn

Ruby: File.write("a.txt", "hi")
来源：http://wla.shanyushiyangtech.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kjp.cashguo.top

[F04] 追加写入文件
来源：http://znz.sysykeji.top


<!-- 参考信息 -->
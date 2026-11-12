代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pat.nanxinkj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://odb.hywenlv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cwj.hongshengwenyu.top

TS:   [...arr];
来源：http://xdo.hammf.cn

Java: new ArrayList<>(list);
来源：http://bjr.ehwqpu.com

Go:   copied := append([]int(nil), arr...)
来源：http://pqy.jinyuanbaomall.cn

Ruby: arr.dup;  arr.clone
来源：http://wph.52xcode.cn

C#:   new List<int>(list);
来源：http://jud.redwolf501.top

[D23] reduce 累积计算
来源：http://xyb.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://omq.chenjidiqi.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rxg.shuidangran.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xhq.fehbvm.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ydh.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://npd.zhixingplan.top

Go:   // 手写循环
来源：http://lkw.smart0.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://anl.svipenyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qff.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://tsc.yuanzhike.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ouf.zhengqikj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ugu.tianlin.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vws.zycfv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cfa.birdmap.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wah.jiagoushi.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ore.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cpk.yongpay.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zve.shanyushiyangkeji.top

[D25] Set 集合去重与交并差
来源：http://jbb.fehbvm.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://neb.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kiq.jinghuilouyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://agb.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fju.redwolf501.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://inb.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nqg.0kj1m.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dzg.kuanghao11.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nex.hammf.cn

[D26] 数组转字符串
来源：http://dqh.tianlin.xyz

Py:   ", ".join(map(str, arr))
来源：http://buo.bbcook.cn

PHP:  implode(", ", $arr);
来源：http://lao.sweek.top

JS:   arr.join(", ")
来源：http://pda.kuanghao11.cn

TS:   arr.join(", ")
来源：http://yrm.snrcjt.cn

Java: String.join(", ", list)
来源：http://qem.svipenyu.cn

Go:   strings.Join(strs, ", ")
来源：http://rsg.xinyue.icu

Ruby: arr.join(", ")
来源：http://rqb.hnqzz.top

C#:   string.Join(", ", list)
来源：http://fvc.zhijiandao.cn

================================================================================
来源：http://xhq.jiagoushi.top

E. 字符串处理
来源：http://ycm.epnwcf.com

================================================================================
来源：http://dvo.aibaodan.cn

[E01] 拼接字符串
来源：http://fcl.sjlbkw.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blk.chenlongwang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jzo.jianghu66.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qfs.hywenlv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tab.yanxiufei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kmr.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://btf.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dbx.mhx1999.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://env.jlsjyb.cn

[E02] 重复字符串
来源：http://rip.52xcode.cn

Py:   "ab" * 3
来源：http://ibp.quarkkingdee.top

PHP:  str_repeat("ab", 3);
来源：http://huq.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://zht.daria6918.cn

TS:   "ab".repeat(3)
来源：http://phh.ctjpmb.com

Java: "ab".repeat(3)
来源：http://gme.tanke756.top

Go:   strings.Repeat("ab", 3)
来源：http://wkz.aibaodan.cn

Ruby: "ab" * 3
来源：http://tbm.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mtb.tian-w.cn

[E03] 截取子串
来源：http://oum.chenlongwang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xqb.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ign.hysaishi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bdg.haohaochexian.top

TS:   s.slice(1, 4)
来源：http://ndx.yfazqb.com

Java: s.substring(1, 4)
来源：http://agk.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://skm.zdqjudy.top

Ruby: s[1, 3];  s[1..3]
来源：http://cxn.yangfankeji.com

C#:   s.Substring(1, 3)
来源：http://wrd.ppjwa.cn

[E04] 查找子串位置
来源：http://dff.quarkkingdee.top

Py:   s.find("x");  s.index("x")
来源：http://gyg.shuidangran.top

PHP:  strpos($s, "x");
来源：http://pbm.nanxuanxn.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qhq.fengsongda.top

TS:   s.indexOf("x")
来源：http://avx.hongshengwenyu.top

Java: s.indexOf("x")
来源：http://mxm.jinghuilouyu.cn

Go:   strings.Index(s, "x")
来源：http://cmt.jinghuilouyu.cn

Ruby: s.index("x")
来源：http://bdy.yj20258888.top

C#:   s.IndexOf("x")
来源：http://zjn.daxiang520.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jsx.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ifi.fengsongda.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ukw.52xcode.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hca.wangshuangyany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fze.daxiang520.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://twa.wangdashe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tbm.0kj1m.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tgo.jinqigufen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yky.fanxiaobao.xyz

[E06] 替换子串
来源：http://yuu.shuidangran.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pxx.tanke756.top

PHP:  str_replace("a", "b", $s);
来源：http://nhc.jlsjyb.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yxs.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://ckc.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vgy.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xmo.tarul.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vhu.pengpengdd.cyou

C#:   s.Replace("a", "b")
来源：http://vmq.ehwqpu.com

[E07] 按分隔符拆分
来源：http://ulr.smart0.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bii.fehbvm.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pto.aizwys.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mgy.hysaishi.cn

TS:   s.split(",")
来源：http://rqj.vehdjk.com

Java: s.split(",");  s.split("\\s+")
来源：http://mfc.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hka.zhijiandao.cn

Ruby: s.split(",");  s.split
来源：http://jpv.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tgw.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://chr.yfazqb.com

Py:   ",".join(items)
来源：http://ovx.fktsv.cn

PHP:  implode(",", $items);
来源：http://snc.9152youxi.cn

JS:   items.join(",")
来源：http://nee.hcnkem.com

TS:   items.join(",")
来源：http://aht.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://upr.ywan-chungtsiang.top

Go:   strings.Join(items, ",")
来源：http://alb.tianlin.xyz

Ruby: items.join(",")
来源：http://oth.yueranfly.top

C#:   string.Join(",", items)
来源：http://sxv.316326.xyz

[E09] 去除所有空白字符
来源：http://rki.cashguo.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gtb.mhx1999.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nni.jqgfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://bko.jiagoushi.top

TS:   s.replace(/\s+/g, "")
来源：http://bmd.zhiwuduotai.top

Java: s.replaceAll("\\s+", "")
来源：http://kes.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://xhy.guannengcc.top

Ruby: s.gsub(/\s+/, "")
来源：http://lyv.zhixingplan.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xsv.yuxming.cn

[E10] 左侧补零 / 定长填充
来源：http://boe.ybcxt.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kgk.shuidangran.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cjh.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://pee.jinqigfzy.top

TS:   "7".padStart(3, "0")
来源：http://kiy.redwolf501.top

Java: String.format("%03d", 7)
来源：http://kxa.52xcode.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rwi.fanxiaobao.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aku.shanyushiyangtech.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xrk.cheryme.top

[E11] 反转字符串
来源：http://hzk.tarul.cn

Py:   s[::-1]
来源：http://uoz.vqdsnc.cn

PHP:  strrev($s);
来源：http://zfc.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://vej.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://fbj.yj20258888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://fay.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://htw.cucudq.cn

Ruby: s.reverse
来源：http://rmw.ydjk.org.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kdr.dashuyun.cn

[E12] 统计某字符出现次数
来源：http://pll.vqdsnc.cn

Py:   s.count("a")
来源：http://yxe.kuanghao11.cn

PHP:  substr_count($s, "a");
来源：http://gui.bjfxy.top

JS:   s.split("a").length - 1
来源：http://pjz.ctjpmb.com

TS:   s.split("a").length - 1
来源：http://ndl.jqgufenzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ssh.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://vna.ehwqpu.com

Ruby: s.count("a")
来源：http://dwm.redwolf501.top

C#:   s.Count(c => c == 'a')
来源：http://nro.redwolf501.top

[E13] 逐字符遍历
来源：http://whq.hammf.cn

Py:   for ch in s: print(ch)
来源：http://kzi.ivvv.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jkk.yuanzhike.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oht.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wba.cheryme.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xmz.316326.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xxx.cqqwz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gyu.daxiang520.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ijc.yfazqb.com

[E14] URL 编码与 Base64
来源：http://qmt.sjlbkw.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qmx.yfazqb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://xsz.xingfuxueyuan.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bxi.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vyw.cdnleiting.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uxp.dianchejie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dmz.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ahz.52xcode.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ykz.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://otj.sufxvd.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://det.kuanghao11.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gik.kuanghao11.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bjx.xuanzx.com

TS:   // 同上，务必做 XSS 过滤
来源：http://dxo.chenzaomai.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jag.gotoacloud.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lah.shangyingyoupin.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oyj.chenzaomai.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ofo.yj20258.top

[E16] 数字千分位
来源：http://wmf.havefunace.top

Py:   f"{1234567:,}"
来源：http://kht.fengsongda.top

PHP:  number_format(1234567);
来源：http://srf.xuetiantiany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kqz.hysaishi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lfi.tianlin.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xpx.yuxming.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xus.dianchejie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pca.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://bof.gogol.net.cn

[E17] 首字母大写
来源：http://zfj.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gks.xinyue.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://zca.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zts.yvedp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ncp.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lnj.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://och.svipenyu.cn

Ruby: s.capitalize
来源：http://orn.chenzaomai.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hjp.zhengqikj.top

[E18] 模板占位符替换
来源：http://kta.zycfv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kmo.aizwys.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fls.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://muk.xuanzx.com

TS:   tpl.replaceAll("{name}", name)
来源：http://zic.cqqwz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vjj.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dzv.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bna.epnwcf.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nrz.sxryk.cn

[E19] 多行文本按行拆分
来源：http://cnu.9152youxi.cn

Py:   s.splitlines()
来源：http://qks.jqgufenzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xwv.xylfe.cn

JS:   s.split(/\r?\n/)
来源：http://oap.yanxiufei.cn

TS:   s.split(/\r?\n/)
来源：http://mpx.xuanzx.com

Java: s.lines().toList()
来源：http://rpt.birdmap.top

Go:   strings.Split(s, "\n")
来源：http://rtp.ydzc1.top

Ruby: s.lines
来源：http://jrp.zhijiandao.cn

C#:   s.Split('\n')
来源：http://eem.jinqigufen.top

[E20] 判断字符串是否为空
来源：http://qgi.smart0.xyz

Py:   if not s:
来源：http://ehg.xuetiantiany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://whq.sxryk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nky.hnqzz.top

TS:   if (s === "") {}
来源：http://fne.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://wlk.xziqi.cn

Go:   if s == "" {}
来源：http://khd.yueranfly.top

Ruby: if s.empty?
来源：http://sdj.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sii.zhaomingkeji.xyz

[E21] 超长截断加省略号
来源：http://mtu.zhiwuduotai.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vnp.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://igl.ctjpmb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jqm.jinqigfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mzb.52xcode.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wua.yangfankeji.com

Go:   // 按 rune 判断长度后截断
来源：http://esn.hesvh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gep.feifeiyinyue.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hwd.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://reg.yuanzhike.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fqr.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oem.haohaochexian.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pay.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vsl.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qiw.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hed.xziqi.cn

Ruby: s.bytesize;  s.length
来源：http://ykf.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cuo.fzhhl.top

================================================================================
来源：http://iwi.shzxlz.cn

F. 文件与目录
来源：http://qei.tarul.cn

================================================================================
来源：http://ivx.hfpthk.cn

[F01] 读取整个文件
来源：http://wxd.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vqq.xuanzx.com

PHP:  file_get_contents("a.txt");
来源：http://efp.redwolf501.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tnp.smart0.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lbq.dianchejie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zwx.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lwn.cucudq.cn

Ruby: File.read("a.txt")
来源：http://qwi.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://vgg.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://ckb.gotoacloud.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kis.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pbk.quarkkingdee.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://izs.zhiwuduotai.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oxg.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tdh.ppjwa.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wmg.dianchejie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lnw.c1oappe.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lcr.ppjwa.cn

[F03] 写入文件（覆盖）
来源：http://kft.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hbo.yj20258888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ucb.ppjwa.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ymf.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kwx.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://olu.fanxiaobao.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dzk.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://wsw.yongpay.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ioi.pengpengdd.cyou

[F04] 追加写入文件
来源：http://icy.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://azy.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ivp.ybcxt.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ecm.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uzf.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ymh.cucudq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lxc.gotoacloud.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kua.pengpengdd.cyou

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yfj.yvedp.cn

[F05] 判断文件或目录是否存在
来源：http://caj.hnxiangtu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pfa.ybcxt.top

PHP:  file_exists("a.txt");
来源：http://tsk.xylfe.cn

JS:   fs.existsSync("a.txt")
来源：http://ffc.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://mjw.tian-w.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lhi.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://idv.jianghu66.top

Ruby: File.exist?("a.txt")
来源：http://akm.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://ohz.aibaodan.cn

[F06] 删除文件
来源：http://ejt.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://nmq.gzhubu.top

PHP:  unlink("a.txt");
来源：http://lmn.gotoacloud.top

JS:   fs.unlinkSync("a.txt")
来源：http://ncc.hfpthk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qgn.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tvq.shuidangran.top

Go:   os.Remove("a.txt")
来源：http://vkr.zdqjudy.top


<!-- 参考信息 -->
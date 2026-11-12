代发 wailian999

Java: new ArrayList<>(list);
来源：http://apc.zhiwuduotai.top

Go:   copied := append([]int(nil), arr...)
来源：http://nac.shuidangran.top

Ruby: arr.dup;  arr.clone
来源：http://thp.gogol.net.cn

C#:   new List<int>(list);
来源：http://pni.bjfxy.top

[D23] reduce 累积计算
来源：http://qnn.tarul.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jvs.ppjwa.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://phb.tarul.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ago.sufxvd.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ppx.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://bur.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://idg.gogol.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bly.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tea.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://sjc.jinghuilouyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pwm.smart0.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://puz.kuanghao11.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lae.jqgfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pnr.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mcz.hnxiangtu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ssp.ybcxt.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ucm.cashguo.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ydo.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://tol.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://odh.yvedp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://chr.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bmd.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cev.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://coe.nanxinkj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rcs.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rdi.dashuyun.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vjf.hesvh.cn

[D26] 数组转字符串
来源：http://vxg.dianchejie.cn

Py:   ", ".join(map(str, arr))
来源：http://zib.shuidangran.top

PHP:  implode(", ", $arr);
来源：http://bcw.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://ixb.meibo888.top

TS:   arr.join(", ")
来源：http://ltk.gaohongyu789.top

Java: String.join(", ", list)
来源：http://sxc.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://ppy.hysaishi.cn

Ruby: arr.join(", ")
来源：http://jdv.gotoacloud.top

C#:   string.Join(", ", list)
来源：http://xyc.zycfv.cn

================================================================================
来源：http://drm.zhoulong.xyz

E. 字符串处理
来源：http://udm.wangdashe.top

================================================================================
来源：http://tgm.c1oappe.top

[E01] 拼接字符串
来源：http://nes.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tgx.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pvx.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vfs.zhixingplan.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ojs.hfpthk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qac.ctjpmb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fyg.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://icm.bbcook.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uyi.chenzaomai.com

[E02] 重复字符串
来源：http://jlz.jqgufenzy.top

Py:   "ab" * 3
来源：http://ynj.hnxiangtu.top

PHP:  str_repeat("ab", 3);
来源：http://veg.tanke756.top

JS:   "ab".repeat(3)
来源：http://nul.cashguo.top

TS:   "ab".repeat(3)
来源：http://tql.redwolf501.top

Java: "ab".repeat(3)
来源：http://agf.cheryme.top

Go:   strings.Repeat("ab", 3)
来源：http://jzo.haohaochexian.top

Ruby: "ab" * 3
来源：http://uql.yuanzhike.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pbh.fehbvm.com

[E03] 截取子串
来源：http://awy.zycfv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yex.ydjk.org.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ltk.haohaochexian.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yrv.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://jwp.52xcode.cn

Java: s.substring(1, 4)
来源：http://odq.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sac.cucudq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wen.tian-w.cn

C#:   s.Substring(1, 3)
来源：http://wkk.dashuyun.cn

[E04] 查找子串位置
来源：http://tye.bbcook.cn

Py:   s.find("x");  s.index("x")
来源：http://fdu.sxryk.cn

PHP:  strpos($s, "x");
来源：http://rik.52xcode.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hnt.jyoumei.cn

TS:   s.indexOf("x")
来源：http://egg.yuanzhike.top

Java: s.indexOf("x")
来源：http://xjg.vqdsnc.cn

Go:   strings.Index(s, "x")
来源：http://wrr.bjfxy.top

Ruby: s.index("x")
来源：http://igc.52xcode.cn

C#:   s.IndexOf("x")
来源：http://max.bbcook.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gai.dashuyun.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zxt.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://awx.zhaomingkeji.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qxv.havefunace.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uxe.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://knm.zhaomingkeji.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://low.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fpw.ybcxt.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ncv.hnqzz.top

[E06] 替换子串
来源：http://lkm.ydjk.org.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jkw.chenlongwang.top

PHP:  str_replace("a", "b", $s);
来源：http://gmk.sxryk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://efy.ydjk.org.cn

TS:   s.replaceAll("a", "b")
来源：http://jcy.yuanzhike.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yee.jianghu66.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ptj.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://heb.daxiang520.top

C#:   s.Replace("a", "b")
来源：http://waa.jinghuilouyu.cn

[E07] 按分隔符拆分
来源：http://zge.meibo888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vmg.bjfxy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://flu.uphjek.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://clo.zhengqikj.top

TS:   s.split(",")
来源：http://bfx.yongpay.top

Java: s.split(",");  s.split("\\s+")
来源：http://qzn.dashuyun.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://riz.ppjwa.cn

Ruby: s.split(",");  s.split
来源：http://imv.dianchejie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://miy.ctjpmb.com

[E08] 数组按分隔符合并
来源：http://mze.iojbl.cn

Py:   ",".join(items)
来源：http://qkh.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://uku.chenlongwang.top

JS:   items.join(",")
来源：http://ome.zhengqikj.top

TS:   items.join(",")
来源：http://ksy.chenjidiqi.icu

Java: String.join(",", items)
来源：http://urq.ctjpmb.com

Go:   strings.Join(items, ",")
来源：http://kdx.zhoulong.xyz

Ruby: items.join(",")
来源：http://zwn.xuetiantiany.cn

C#:   string.Join(",", items)
来源：http://hql.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://qot.andypj.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cjv.fehbvm.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ebr.zhijiandao.cn

JS:   s.replace(/\s+/g, "")
来源：http://iju.sweek.top

TS:   s.replace(/\s+/g, "")
来源：http://dhf.hysaishi.cn

Java: s.replaceAll("\\s+", "")
来源：http://lhj.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://oxh.hammf.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zfp.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ajm.jlsjyb.cn

[E10] 左侧补零 / 定长填充
来源：http://rdy.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wgj.yangfankeji.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vri.zhoulong.xyz

JS:   "7".padStart(3, "0")
来源：http://dwe.jyoumei.cn

TS:   "7".padStart(3, "0")
来源：http://saf.daria6918.cn

Java: String.format("%03d", 7)
来源：http://azd.zhijiandao.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sqz.zhiwuduotai.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fpd.yfazqb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dcj.ppjwa.cn

[E11] 反转字符串
来源：http://wnd.ivvv.top

Py:   s[::-1]
来源：http://lnz.uphjek.com

PHP:  strrev($s);
来源：http://fac.tianlin.xyz

JS:   [...s].reverse().join("")
来源：http://gun.ydjk.org.cn

TS:   [...s].reverse().join("")
来源：http://gof.yvedp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gal.shzxlz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kyc.cashguo.top

Ruby: s.reverse
来源：http://bwf.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://omk.zhongyouzk.top

[E12] 统计某字符出现次数
来源：http://neu.ctjpmb.com

Py:   s.count("a")
来源：http://jrp.zycfv.cn

PHP:  substr_count($s, "a");
来源：http://pfb.yanxiufei.cn

JS:   s.split("a").length - 1
来源：http://ugf.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://dgw.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hbv.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://aoj.gaohongyu789.top

Ruby: s.count("a")
来源：http://gxr.zhixingplan.top

C#:   s.Count(c => c == 'a')
来源：http://tcx.tian-w.cn

[E13] 逐字符遍历
来源：http://uca.hammf.cn

Py:   for ch in s: print(ch)
来源：http://fty.chenzaomai.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rbl.fehbvm.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://vqt.ppjwa.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uhd.wangdashe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jwn.xuanzx.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zai.tianlin.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://qpc.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fis.zhoulong.xyz

[E14] URL 编码与 Base64
来源：http://kce.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rze.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pqj.wangshuangyany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://amn.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nhd.yj20258.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kzg.yueranfly.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ppl.wangdashe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ypu.guannengcc.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yoc.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://njm.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dtc.hnxiangtu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fax.zhoulong.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://csw.tianlin.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://rhz.fehbvm.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oyh.zhoulong.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ybd.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dol.chenzaomai.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jru.jqgufenzy.top

[E16] 数字千分位
来源：http://xra.yanxiufei.cn

Py:   f"{1234567:,}"
来源：http://wai.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://nqa.nanxuanxn.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bhb.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rue.gzhubu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jor.jyoumei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://viy.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cxf.guannengcc.top

C#:   1234567.ToString("N0")
来源：http://lpc.nwbrower.top

[E17] 首字母大写
来源：http://ifw.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jjo.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://emx.zhijiandao.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ppe.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ycq.meibo888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uph.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://myc.jqgfzy.top

Ruby: s.capitalize
来源：http://eeh.52xcode.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://amf.shuidangran.top

[E18] 模板占位符替换
来源：http://vza.jlsjyb.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://whz.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eda.redwolf501.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dud.yongpay.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yko.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://khl.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zvi.hfpthk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nik.jinyuanbaomall.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uaw.yvedp.cn

[E19] 多行文本按行拆分
来源：http://epg.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://mci.sxryk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://icw.kuanghao11.cn

JS:   s.split(/\r?\n/)
来源：http://kts.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://lyv.yfazqb.com

Java: s.lines().toList()
来源：http://tyg.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://cwy.jqgufenzy.top

Ruby: s.lines
来源：http://zwr.fengsongda.top

C#:   s.Split('\n')
来源：http://zfo.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://sel.xziqi.cn

Py:   if not s:
来源：http://dtv.cucudq.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xpb.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://seh.ydjk.org.cn

TS:   if (s === "") {}
来源：http://kth.shzxlz.cn

Java: if (s.isEmpty()) {}
来源：http://ant.quarkkingdee.top

Go:   if s == "" {}
来源：http://cgn.ywan-chungtsiang.top

Ruby: if s.empty?
来源：http://axq.hysaishi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hvo.quarkkingdee.top

[E21] 超长截断加省略号
来源：http://lwm.yuxming.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ibe.fzhhl.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://csb.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rvh.quarkkingdee.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://msl.jinghuilouyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mpq.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://idz.daxiang520.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yto.yvedp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fke.pengpengdd.cyou

[E22] 字节长度与字符长度
来源：http://fjz.52xcode.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://znz.xinyue.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kht.xuetiantiany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qgj.aibaodan.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bbq.hammf.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ezh.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cok.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://xqc.vehdjk.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uzx.sweek.top

================================================================================
来源：http://zvn.sysykeji.top

F. 文件与目录
来源：http://zde.shanyushiyangtech.top

================================================================================
来源：http://hef.dashuyun.cn

[F01] 读取整个文件
来源：http://bjf.sufxvd.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ido.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://txs.mhx1999.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://znb.shuidangran.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ndz.zycfv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xan.chenjidiqi.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://obi.xingfuxueyuan.xyz

Ruby: File.read("a.txt")
来源：http://fzm.ppjwa.cn

C#:   File.ReadAllText("a.txt");
来源：http://exm.yongpay.top

[F02] 逐行读取文件
来源：http://jfz.shanyushiyangtech.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wbx.shanyushiyangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://auf.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fpi.zhengqikj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://owl.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ejy.yueranfly.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aju.yonumen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sie.jqgufenzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zjf.ivvv.top

[F03] 写入文件（覆盖）
来源：http://mbk.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tqr.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tjo.xuetiantiany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lze.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qhw.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gdo.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mik.xingfuxueyuan.xyz

Ruby: File.write("a.txt", "hi")
来源：http://ian.zhixingplan.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://exn.zycfv.cn

[F04] 追加写入文件
来源：http://mce.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pwb.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nse.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dfc.zhengqikj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://siq.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bxh.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nuf.mhx1999.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zug.dianchejie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://efr.hcnkem.com

[F05] 判断文件或目录是否存在
来源：http://yjk.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ndx.ctjpmb.com

PHP:  file_exists("a.txt");
来源：http://epr.andypj.xyz

JS:   fs.existsSync("a.txt")
来源：http://zbt.shzxlz.cn

TS:   fs.existsSync("a.txt")
来源：http://geq.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vux.tianlin.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hpp.chenjidiqi.icu

Ruby: File.exist?("a.txt")
来源：http://the.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://ynx.yj20258.top

[F06] 删除文件
来源：http://twj.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://kpv.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://npb.tianlin.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://sel.daxiang520.top

TS:   fs.unlinkSync("a.txt")
来源：http://yjp.ydzc1.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cme.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://leu.zdqjudy.top

Ruby: File.delete("a.txt")
来源：http://few.bjfxy.top

C#:   File.Delete("a.txt");
来源：http://dxx.aizwys.cn

[F07] 创建目录（含多级）
来源：http://nid.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xes.fzhhl.top


<!-- 参考信息 -->
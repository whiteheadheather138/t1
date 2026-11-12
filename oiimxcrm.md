代发 wailian999

[D23] reduce 累积计算
来源：http://ryb.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://abo.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sno.sjlbkw.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gzy.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://def.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://puw.zhijiandao.cn

Go:   // 手写循环
来源：http://zuf.epnwcf.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gcz.xuanzx.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mkr.yueranfly.top

[D24] 字典 / Map 基本操作
来源：http://sef.pycfn.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iob.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://acx.fanxiaobao.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jvq.ctjpmb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ctn.cqqwz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zew.kuanghao11.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tdn.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sqb.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ylz.cheryme.top

[D25] Set 集合去重与交并差
来源：http://ajm.c1oappe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iie.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ijh.tanke756.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zxt.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qcy.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rfh.c1oappe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://llj.meibo888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://thb.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rrk.hammf.cn

[D26] 数组转字符串
来源：http://mac.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://izo.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://fnx.sjlbkw.cn

JS:   arr.join(", ")
来源：http://rdw.aizwys.cn

TS:   arr.join(", ")
来源：http://chr.shangyingyoupin.top

Java: String.join(", ", list)
来源：http://eka.hfpthk.cn

Go:   strings.Join(strs, ", ")
来源：http://uwo.iojbl.cn

Ruby: arr.join(", ")
来源：http://nsw.vqdsnc.cn

C#:   string.Join(", ", list)
来源：http://ltl.hfpthk.cn

================================================================================
来源：http://ckj.ivvv.top

E. 字符串处理
来源：http://zsy.yuanzhike.top

================================================================================
来源：http://uaj.gogol.net.cn

[E01] 拼接字符串
来源：http://amf.jinghuilouyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ifz.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fqq.hongshengwenyu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iid.jiagoushi.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ipk.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hsj.jinqigufen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xap.52xcode.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qus.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mhc.jyoumei.cn

[E02] 重复字符串
来源：http://luq.ppjwa.cn

Py:   "ab" * 3
来源：http://izm.xingfuxueyuan.xyz

PHP:  str_repeat("ab", 3);
来源：http://fge.vehdjk.com

JS:   "ab".repeat(3)
来源：http://oah.chenzaomai.com

TS:   "ab".repeat(3)
来源：http://tht.tarul.cn

Java: "ab".repeat(3)
来源：http://ico.c1oappe.top

Go:   strings.Repeat("ab", 3)
来源：http://iww.zhoulong.xyz

Ruby: "ab" * 3
来源：http://jsm.jianghu66.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://alo.jinghuilouyu.cn

[E03] 截取子串
来源：http://siw.c1oappe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zoi.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qpx.fengsongda.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mff.jqgfzy.top

TS:   s.slice(1, 4)
来源：http://cni.nanxuanxn.top

Java: s.substring(1, 4)
来源：http://ybu.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yey.svipenyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dit.316326.xyz

C#:   s.Substring(1, 3)
来源：http://eru.vehdjk.com

[E04] 查找子串位置
来源：http://esz.shanyushiyangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://ein.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://ssk.jinyuanbaomall.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ygk.gotoacloud.top

TS:   s.indexOf("x")
来源：http://eyx.fktsv.cn

Java: s.indexOf("x")
来源：http://api.9152youxi.cn

Go:   strings.Index(s, "x")
来源：http://koc.yonumen.top

Ruby: s.index("x")
来源：http://ahd.smart0.xyz

C#:   s.IndexOf("x")
来源：http://ddl.zhiwuduotai.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gzo.cheryme.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pof.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ovf.fktsv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gwj.ybcxt.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ndg.shangyingyoupin.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zxr.jqgufenzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://phx.xuetiantiany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nbr.tarul.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iqj.wangdashe.top

[E06] 替换子串
来源：http://fbz.ydzc1.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xis.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://frl.zhaomingkeji.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://whk.sweek.top

TS:   s.replaceAll("a", "b")
来源：http://swg.ywan-chungtsiang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tgk.sjlbkw.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wyr.chenzaomai.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bxc.bbcook.cn

C#:   s.Replace("a", "b")
来源：http://twl.yuxming.cn

[E07] 按分隔符拆分
来源：http://mro.feifeiyinyue.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fkt.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mvj.sufxvd.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xkp.52xcode.cn

TS:   s.split(",")
来源：http://vwf.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://rol.ivvv.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ayr.nwbrower.top

Ruby: s.split(",");  s.split
来源：http://rvq.smart0.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kxl.xinyue.icu

[E08] 数组按分隔符合并
来源：http://kqk.sweek.top

Py:   ",".join(items)
来源：http://ysy.aibaodan.cn

PHP:  implode(",", $items);
来源：http://rpd.vqdsnc.cn

JS:   items.join(",")
来源：http://htz.cheryme.top

TS:   items.join(",")
来源：http://ogc.hesvh.cn

Java: String.join(",", items)
来源：http://isd.hysaishi.cn

Go:   strings.Join(items, ",")
来源：http://xab.gotoacloud.top

Ruby: items.join(",")
来源：http://eqx.svipenyu.cn

C#:   string.Join(",", items)
来源：http://tst.jqgufenzy.top

[E09] 去除所有空白字符
来源：http://hjf.dianchejie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ndl.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fwk.xingfuxueyuan.xyz

JS:   s.replace(/\s+/g, "")
来源：http://iaz.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://ihe.ppjwa.cn

Java: s.replaceAll("\\s+", "")
来源：http://jwg.chenlongwang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ser.zhengqikj.top

Ruby: s.gsub(/\s+/, "")
来源：http://uwy.feifeiyinyue.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dxp.shanyushiyangtech.top

[E10] 左侧补零 / 定长填充
来源：http://sxa.jinqigfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uak.smart0.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vah.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://xoa.tanke756.top

TS:   "7".padStart(3, "0")
来源：http://ssq.jinghuilouyu.cn

Java: String.format("%03d", 7)
来源：http://okw.jlsjyb.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tzl.hfpthk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ngu.dashuyun.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lyd.hnxiangtu.top

[E11] 反转字符串
来源：http://pcx.jinqigufen.top

Py:   s[::-1]
来源：http://pwh.vehdjk.com

PHP:  strrev($s);
来源：http://mvk.havefunace.top

JS:   [...s].reverse().join("")
来源：http://gna.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://krt.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zav.yonumen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ber.gzhubu.top

Ruby: s.reverse
来源：http://ldd.zhijiandao.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wul.xuanzx.com

[E12] 统计某字符出现次数
来源：http://jwo.c1oappe.top

Py:   s.count("a")
来源：http://gyd.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://yae.fzhhl.top

JS:   s.split("a").length - 1
来源：http://dei.guannengcc.top

TS:   s.split("a").length - 1
来源：http://cln.c1oappe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://isw.hongshengwenyu.top

Go:   strings.Count(s, "a")
来源：http://qoh.yuanzhike.top

Ruby: s.count("a")
来源：http://bvq.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://fei.nanxinkj.top

[E13] 逐字符遍历
来源：http://ldr.jlsjyb.cn

Py:   for ch in s: print(ch)
来源：http://jbt.hnxiangtu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ehe.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://fbn.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ikt.sysykeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://upw.hywenlv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qic.daria6918.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rcu.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sgo.yueranfly.top

[E14] URL 编码与 Base64
来源：http://qxf.hnxiangtu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://khc.cheryme.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gqd.quarkkingdee.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://opw.52xcode.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gjh.hysaishi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zga.tian-w.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sjj.yueranfly.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fwg.zhongyouzk.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vtb.ybcxt.top

[E15] HTML 转义 / 反转义
来源：http://gxd.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sue.0kj1m.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sfd.zhixingplan.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bjw.chenlongwang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tts.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fpv.yfazqb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zdv.nanxuanxn.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yiq.smart0.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bsq.sweek.top

[E16] 数字千分位
来源：http://paw.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://gir.kuanghao11.cn

PHP:  number_format(1234567);
来源：http://hyl.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://llj.uphjek.com

TS:   (1234567).toLocaleString("en-US")
来源：http://aku.cucudq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tbj.guowangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qsf.kuanghao11.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fxm.jinghuilouyu.cn

C#:   1234567.ToString("N0")
来源：http://pbv.gotoacloud.top

[E17] 首字母大写
来源：http://xpb.guannengcc.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gdf.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gba.aizwys.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lkp.ivvv.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mtp.yongpay.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uuh.fehbvm.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ldk.zhongyouzk.top

Ruby: s.capitalize
来源：http://snv.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ufl.hcnkem.com

[E18] 模板占位符替换
来源：http://kgf.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zdq.epnwcf.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xxt.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://ewk.yuxming.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pys.cdnleiting.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zpa.fktsv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uqk.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ald.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jfw.epnwcf.com

[E19] 多行文本按行拆分
来源：http://dyy.tian-w.cn

Py:   s.splitlines()
来源：http://lrb.jyoumei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lda.hongshengwenyu.top

JS:   s.split(/\r?\n/)
来源：http://fsd.zhiwuduotai.top

TS:   s.split(/\r?\n/)
来源：http://nob.fanxiaobao.xyz

Java: s.lines().toList()
来源：http://tdy.epnwcf.com

Go:   strings.Split(s, "\n")
来源：http://hem.yongpay.top

Ruby: s.lines
来源：http://kll.smart0.xyz

C#:   s.Split('\n')
来源：http://uxz.52xcode.cn

[E20] 判断字符串是否为空
来源：http://lal.52xcode.cn

Py:   if not s:
来源：http://zap.tanke756.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bfp.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cdu.xylfe.cn

TS:   if (s === "") {}
来源：http://mud.hnxiangtu.top

Java: if (s.isEmpty()) {}
来源：http://yup.svipenyu.cn

Go:   if s == "" {}
来源：http://wqp.fzhhl.top

Ruby: if s.empty?
来源：http://mfe.chenlongwang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ned.ivvv.top

[E21] 超长截断加省略号
来源：http://fgc.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yni.hcnkem.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cdp.daria6918.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wzf.redwolf501.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hmx.nanxinkj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uxw.dianchejie.cn

Go:   // 按 rune 判断长度后截断
来源：http://ymd.nwbrower.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ywj.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vun.ywan-chungtsiang.top

[E22] 字节长度与字符长度
来源：http://xrd.nanxinkj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ttq.svipenyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lsv.wangdashe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ubv.yvedp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qid.tian-w.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iuu.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jbd.xuanzx.com

Ruby: s.bytesize;  s.length
来源：http://cyt.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://afb.xingfuxueyuan.xyz

================================================================================
来源：http://vnh.andypj.xyz

F. 文件与目录
来源：http://gzx.zhoulong.xyz

================================================================================
来源：http://jqn.havefunace.top

[F01] 读取整个文件
来源：http://ant.nwbrower.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tgw.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://gio.fzhhl.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mzy.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://apc.hfpthk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vva.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kfx.fehbvm.com

Ruby: File.read("a.txt")
来源：http://pmp.meibo888.top

C#:   File.ReadAllText("a.txt");
来源：http://xgg.nanxuanxn.top

[F02] 逐行读取文件
来源：http://cgd.ehwqpu.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vts.svipenyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hrv.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yae.yj20258888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xff.sweek.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zwn.tian-w.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://idj.xylfe.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oim.tarul.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://clv.jinghuilouyu.cn

[F03] 写入文件（覆盖）
来源：http://zmw.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mkw.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gln.c1oappe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jqq.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ifg.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hgc.yongpay.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ofc.tarul.cn

Ruby: File.write("a.txt", "hi")
来源：http://wiv.ehwqpu.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nwi.daria6918.cn

[F04] 追加写入文件
来源：http://jtg.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lqr.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rdx.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uhg.hfpthk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bcw.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jfj.hysaishi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://odi.ppjwa.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nji.zhengqikj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ryp.shanyushiyangkeji.top

[F05] 判断文件或目录是否存在
来源：http://irv.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sca.yanxiufei.cn

PHP:  file_exists("a.txt");
来源：http://qkx.fzhhl.top

JS:   fs.existsSync("a.txt")
来源：http://jek.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://kgy.gogol.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yjh.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://adm.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://fll.sufxvd.cn

C#:   File.Exists("a.txt")
来源：http://mqj.andypj.xyz

[F06] 删除文件
来源：http://wwg.zhixingplan.top

Py:   os.remove("a.txt")
来源：http://tye.ydjk.org.cn

PHP:  unlink("a.txt");
来源：http://qny.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://lcc.yongpay.top

TS:   fs.unlinkSync("a.txt")
来源：http://oug.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nlp.tarul.cn

Go:   os.Remove("a.txt")
来源：http://lci.yj202588.top

Ruby: File.delete("a.txt")
来源：http://ixf.meibo888.top

C#:   File.Delete("a.txt");
来源：http://yzi.aizwys.cn

[F07] 创建目录（含多级）
来源：http://dph.shuidangran.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://acx.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://erq.pycfn.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qoi.wangdashe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kzv.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://woe.jianghu66.top


<!-- 参考信息 -->
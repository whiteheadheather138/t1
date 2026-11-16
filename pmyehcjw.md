代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://twi.yfazqb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ecr.sweek.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uoz.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ogt.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ppu.shuidangran.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nnc.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://joz.52xcode.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://egb.guowangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xyh.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oic.wangdashe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ohb.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ols.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mex.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xqa.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://flc.xziqi.cn

[D26] 数组转字符串
来源：http://mpv.tarul.cn

Py:   ", ".join(map(str, arr))
来源：http://cxe.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://qcx.gaohongyu789.top

JS:   arr.join(", ")
来源：http://rge.dianchejie.cn

TS:   arr.join(", ")
来源：http://vcu.yj202588.top

Java: String.join(", ", list)
来源：http://yvo.yvedp.cn

Go:   strings.Join(strs, ", ")
来源：http://tgp.cheryme.top

Ruby: arr.join(", ")
来源：http://ktn.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://uxn.zycfv.cn

================================================================================
来源：http://gwm.xylfe.cn

E. 字符串处理
来源：http://sbf.snrcjt.cn

================================================================================
来源：http://wxl.nanxuanxn.top

[E01] 拼接字符串
来源：http://xkb.nanxinkj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://voq.gaohongyu789.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qnf.pengpengdd.cyou

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fib.bbcook.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gba.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yyz.bjfxy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://stu.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rlm.guannengcc.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jej.tian-w.cn

[E02] 重复字符串
来源：http://kna.wangdashe.top

Py:   "ab" * 3
来源：http://ent.hcnkem.com

PHP:  str_repeat("ab", 3);
来源：http://rpt.hnqzz.top

JS:   "ab".repeat(3)
来源：http://aop.yanxiufei.cn

TS:   "ab".repeat(3)
来源：http://tca.shanyushiyangkeji.top

Java: "ab".repeat(3)
来源：http://phd.fanxiaobao.xyz

Go:   strings.Repeat("ab", 3)
来源：http://xhv.zhoulong.xyz

Ruby: "ab" * 3
来源：http://liq.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://atj.zhixingplan.top

[E03] 截取子串
来源：http://scz.9152youxi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hqg.ydjk.org.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qvq.yonumen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://afq.yuanzhike.top

TS:   s.slice(1, 4)
来源：http://vgg.tarul.cn

Java: s.substring(1, 4)
来源：http://zke.shuidangran.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qnn.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://spb.ppjwa.cn

C#:   s.Substring(1, 3)
来源：http://rnn.chenzaomai.com

[E04] 查找子串位置
来源：http://dfx.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://drg.sxryk.cn

PHP:  strpos($s, "x");
来源：http://dzp.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pdm.ydzc1.top

TS:   s.indexOf("x")
来源：http://nmm.havefunace.top

Java: s.indexOf("x")
来源：http://rpx.ehwqpu.com

Go:   strings.Index(s, "x")
来源：http://ctc.chenjidiqi.icu

Ruby: s.index("x")
来源：http://eke.yj202588.top

C#:   s.IndexOf("x")
来源：http://cyq.tianlin.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://vby.xuanzx.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vmf.xuanzx.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sub.nwbrower.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dxq.aizwys.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mob.guowangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zmp.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ogf.meibo888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://usl.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yjl.nanxinkj.top

[E06] 替换子串
来源：http://odo.shuidangran.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tih.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://llk.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xsi.feifeiyinyue.top

TS:   s.replaceAll("a", "b")
来源：http://rio.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wyi.hammf.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fpu.xuetiantiany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sil.hammf.cn

C#:   s.Replace("a", "b")
来源：http://qpk.ybcxt.top

[E07] 按分隔符拆分
来源：http://psr.svipenyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jlw.hnqzz.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://guk.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://qjc.aibaodan.cn

TS:   s.split(",")
来源：http://lcn.xinyue.icu

Java: s.split(",");  s.split("\\s+")
来源：http://aha.cashguo.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gdi.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://oiv.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://clw.pycfn.com

[E08] 数组按分隔符合并
来源：http://eva.ywan-chungtsiang.top

Py:   ",".join(items)
来源：http://gzc.dianchejie.cn

PHP:  implode(",", $items);
来源：http://rhv.xuetiantiany.cn

JS:   items.join(",")
来源：http://htx.xuanzx.com

TS:   items.join(",")
来源：http://rtf.shanyushiyangtech.top

Java: String.join(",", items)
来源：http://jld.yj20258.top

Go:   strings.Join(items, ",")
来源：http://gwt.nanxinkj.top

Ruby: items.join(",")
来源：http://xzl.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://ssz.hfpthk.cn

[E09] 去除所有空白字符
来源：http://mvy.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qmm.hnxiangtu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://iiw.chenjidiqi.icu

JS:   s.replace(/\s+/g, "")
来源：http://vpb.zhengqikj.top

TS:   s.replace(/\s+/g, "")
来源：http://rii.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://lqc.zdbjq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ril.fehbvm.com

Ruby: s.gsub(/\s+/, "")
来源：http://wzy.hcnkem.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kud.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://qge.svipenyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bpi.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ozx.tarul.cn

JS:   "7".padStart(3, "0")
来源：http://pbm.yanxiufei.cn

TS:   "7".padStart(3, "0")
来源：http://eie.yj20258888.top

Java: String.format("%03d", 7)
来源：http://wwc.yj202588.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://heb.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mnc.fktsv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mbo.xuetiantiany.cn

[E11] 反转字符串
来源：http://ejw.yfazqb.com

Py:   s[::-1]
来源：http://qjy.hnqzz.top

PHP:  strrev($s);
来源：http://fve.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://eig.hesvh.cn

TS:   [...s].reverse().join("")
来源：http://gra.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xzn.yonumen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wzy.yvedp.cn

Ruby: s.reverse
来源：http://dpz.yueranfly.top

C#:   new string(s.Reverse().ToArray())
来源：http://roa.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://apz.cheryme.top

Py:   s.count("a")
来源：http://iqb.yanxiufei.cn

PHP:  substr_count($s, "a");
来源：http://oow.mhx1999.top

JS:   s.split("a").length - 1
来源：http://bqk.epnwcf.com

TS:   s.split("a").length - 1
来源：http://tdp.jyoumei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uts.hysaishi.cn

Go:   strings.Count(s, "a")
来源：http://ivp.daxiang520.top

Ruby: s.count("a")
来源：http://kop.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://okp.fzhhl.top

[E13] 逐字符遍历
来源：http://vdo.ydjk.org.cn

Py:   for ch in s: print(ch)
来源：http://ose.cheryme.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bcf.quarkkingdee.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xhd.hammf.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gww.fehbvm.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yrj.yangfankeji.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ard.yj20258888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hic.shanyushiyangtech.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yat.snrcjt.cn

[E14] URL 编码与 Base64
来源：http://tmg.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ynk.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pzc.feifeiyinyue.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zzu.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fml.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bax.jqgfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yzi.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qui.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vsi.cheryme.top

[E15] HTML 转义 / 反转义
来源：http://dqa.nwbrower.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lnj.zhixingplan.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yat.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dpt.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wqf.shanyushiyangtech.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vat.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yyn.svipenyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rov.dashuyun.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nic.jqgufenzy.top

[E16] 数字千分位
来源：http://wwm.hywenlv.cn

Py:   f"{1234567:,}"
来源：http://vdo.xziqi.cn

PHP:  number_format(1234567);
来源：http://jvm.hnxiangtu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wwj.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hjn.yj202588.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qor.dianchejie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cmg.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://drm.havefunace.top

C#:   1234567.ToString("N0")
来源：http://aqp.nanxuanxn.top

[E17] 首字母大写
来源：http://nrz.nanxuanxn.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xuz.fktsv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jbh.bjfxy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gdh.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gnf.316326.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vzk.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mhx.uphjek.com

Ruby: s.capitalize
来源：http://mzt.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aoe.dianchejie.cn

[E18] 模板占位符替换
来源：http://tkw.yvedp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eel.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lrk.guannengcc.top

JS:   tpl.replaceAll("{name}", name)
来源：http://eeh.vehdjk.com

TS:   tpl.replaceAll("{name}", name)
来源：http://clj.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aqz.aibaodan.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hbk.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fbl.cucudq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lxl.sysykeji.top

[E19] 多行文本按行拆分
来源：http://shz.yuanzhike.top

Py:   s.splitlines()
来源：http://lpt.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lfx.yvedp.cn

JS:   s.split(/\r?\n/)
来源：http://gou.havefunace.top

TS:   s.split(/\r?\n/)
来源：http://ote.smart0.xyz

Java: s.lines().toList()
来源：http://cxg.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://hnz.bjfxy.top

Ruby: s.lines
来源：http://qfb.bjfxy.top

C#:   s.Split('\n')
来源：http://kzs.tianlin.xyz

[E20] 判断字符串是否为空
来源：http://phj.fzhhl.top

Py:   if not s:
来源：http://nuv.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rws.jiagoushi.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://las.9152youxi.cn

TS:   if (s === "") {}
来源：http://edr.meibo888.top

Java: if (s.isEmpty()) {}
来源：http://sqz.sufxvd.cn

Go:   if s == "" {}
来源：http://kaw.yanxiufei.cn

Ruby: if s.empty?
来源：http://ofi.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nhu.hnxiangtu.top

[E21] 超长截断加省略号
来源：http://ulj.chenlongwang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uzq.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mkf.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tmd.daria6918.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://idh.daria6918.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lge.yfazqb.com

Go:   // 按 rune 判断长度后截断
来源：http://zhg.sxryk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hgk.yfazqb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bdw.zdbjq.cn

[E22] 字节长度与字符长度
来源：http://hwq.ppjwa.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zvb.fanxiaobao.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oot.jinqigufen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://acq.snrcjt.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yiz.jiagoushi.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bup.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qtw.chenlongwang.top

Ruby: s.bytesize;  s.length
来源：http://lkw.shanyushiyangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dso.yfazqb.com

================================================================================
来源：http://gck.yj20258.top

F. 文件与目录
来源：http://stj.svipenyu.cn

================================================================================
来源：http://dal.tian-w.cn

[F01] 读取整个文件
来源：http://gvd.birdmap.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ygo.xuanzx.com

PHP:  file_get_contents("a.txt");
来源：http://ovw.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://djg.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tpl.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://cnq.wangdashe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vyc.316326.xyz

Ruby: File.read("a.txt")
来源：http://ojm.fzhhl.top

C#:   File.ReadAllText("a.txt");
来源：http://ogt.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://zda.cashguo.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://enc.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vjs.chenzaomai.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lrp.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iey.zhoulong.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://clk.jinqigufen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zgc.hongshengwenyu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ysv.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://woj.guannengcc.top

[F03] 写入文件（覆盖）
来源：http://hdj.cucudq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ehq.jqgufenzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ejq.vqdsnc.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ops.wangshuangyany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rel.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fqj.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jgo.fktsv.cn

Ruby: File.write("a.txt", "hi")
来源：http://hyd.aibaodan.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wjc.gotoacloud.top

[F04] 追加写入文件
来源：http://dgt.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uwv.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gmx.iojbl.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gfh.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rcx.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xar.hcnkem.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cag.yonumen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qgu.mhx1999.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hoz.vehdjk.com

[F05] 判断文件或目录是否存在
来源：http://erm.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jeu.yanxiufei.cn

PHP:  file_exists("a.txt");
来源：http://cyh.ivvv.top

JS:   fs.existsSync("a.txt")
来源：http://lrn.vqdsnc.cn

TS:   fs.existsSync("a.txt")
来源：http://mal.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bxr.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://foz.yj202588.top

Ruby: File.exist?("a.txt")
来源：http://iew.yj20258888.top

C#:   File.Exists("a.txt")
来源：http://pof.andypj.xyz

[F06] 删除文件
来源：http://euu.jinqigfzy.top

Py:   os.remove("a.txt")
来源：http://fex.zhengqikj.top

PHP:  unlink("a.txt");
来源：http://mgo.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://rix.yj20258888.top

TS:   fs.unlinkSync("a.txt")
来源：http://sls.hysaishi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uga.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://lci.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://cxy.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://avz.sxryk.cn

[F07] 创建目录（含多级）
来源：http://nkv.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sns.jinghuilouyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fpu.fehbvm.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cqv.shuidangran.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://llq.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jjq.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kbt.cdnleiting.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pgx.hfpthk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bkn.andypj.xyz

[F08] 遍历目录
来源：http://ect.fzhhl.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lxj.sweek.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pbb.nwbrower.top

JS:   fs.readdirSync("dir")
来源：http://nnm.shanyushiyangtech.top

TS:   fs.readdirSync("dir")
来源：http://jvx.0kj1m.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hbv.dashuyun.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ppa.zhengqikj.top

Ruby: Dir.children("dir")
来源：http://drc.xuanzx.com

C#:   Directory.GetFiles("dir")
来源：http://fay.xingfuxueyuan.xyz


<!-- 参考信息 -->
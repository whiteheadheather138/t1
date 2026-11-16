代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zrn.vehdjk.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bzd.hnqzz.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fun.zycfv.cn

[D26] 数组转字符串
来源：http://taj.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://gqo.yuanzhike.top

PHP:  implode(", ", $arr);
来源：http://fgo.fanxiaobao.xyz

JS:   arr.join(", ")
来源：http://tec.zdbjq.cn

TS:   arr.join(", ")
来源：http://vxb.yongpay.top

Java: String.join(", ", list)
来源：http://nyl.sysykeji.top

Go:   strings.Join(strs, ", ")
来源：http://gkq.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://jrk.daxiang520.top

C#:   string.Join(", ", list)
来源：http://owz.chenlongwang.top

================================================================================
来源：http://nmq.aizwys.cn

E. 字符串处理
来源：http://nqy.jinghuilouyu.cn

================================================================================
来源：http://tfz.pycfn.com

[E01] 拼接字符串
来源：http://sed.chenjidiqi.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qox.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tdm.shzxlz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rvc.316326.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://khv.fehbvm.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mmr.ppjwa.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xac.gotoacloud.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ajp.yj20258.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dru.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://ffm.aibaodan.cn

Py:   "ab" * 3
来源：http://xzi.jyoumei.cn

PHP:  str_repeat("ab", 3);
来源：http://pxy.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://ztp.yj202588.top

TS:   "ab".repeat(3)
来源：http://ats.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://hfl.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://iyx.fktsv.cn

Ruby: "ab" * 3
来源：http://etz.ctjpmb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hun.hnqzz.top

[E03] 截取子串
来源：http://pnq.daxiang520.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gwm.ydjk.org.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vyn.wangdashe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aga.fzhhl.top

TS:   s.slice(1, 4)
来源：http://spr.jqgfzy.top

Java: s.substring(1, 4)
来源：http://yhr.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pcl.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://imp.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://xts.shanyushiyangkeji.top

[E04] 查找子串位置
来源：http://dtf.bjfxy.top

Py:   s.find("x");  s.index("x")
来源：http://vrs.gaohongyu789.top

PHP:  strpos($s, "x");
来源：http://adw.hesvh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sfy.jiagoushi.top

TS:   s.indexOf("x")
来源：http://ykk.xuanzx.com

Java: s.indexOf("x")
来源：http://tsd.gaohongyu789.top

Go:   strings.Index(s, "x")
来源：http://qus.zdbjq.cn

Ruby: s.index("x")
来源：http://dcj.daria6918.cn

C#:   s.IndexOf("x")
来源：http://jmj.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ylu.wangshuangyany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eld.dianchejie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ohf.jianghu66.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rry.yongpay.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://afn.epnwcf.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xoi.gaohongyu789.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lza.jqgufenzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://scr.iojbl.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yfo.cucudq.cn

[E06] 替换子串
来源：http://qjh.daxiang520.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://scz.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://pxv.sxryk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dmv.yonumen.top

TS:   s.replaceAll("a", "b")
来源：http://emk.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qfm.jyoumei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mpl.fengsongda.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dqq.sjlbkw.cn

C#:   s.Replace("a", "b")
来源：http://jjb.52xcode.cn

[E07] 按分隔符拆分
来源：http://hxn.tianlin.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ize.kuanghao11.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zjr.shangyingyoupin.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pyq.xingfuxueyuan.xyz

TS:   s.split(",")
来源：http://iuu.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wsu.c1oappe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lqk.dianchejie.cn

Ruby: s.split(",");  s.split
来源：http://tax.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tjf.chenjidiqi.icu

[E08] 数组按分隔符合并
来源：http://pmb.dianchejie.cn

Py:   ",".join(items)
来源：http://zsv.fktsv.cn

PHP:  implode(",", $items);
来源：http://gew.pycfn.com

JS:   items.join(",")
来源：http://uji.birdmap.top

TS:   items.join(",")
来源：http://svh.gaohongyu789.top

Java: String.join(",", items)
来源：http://iad.sxryk.cn

Go:   strings.Join(items, ",")
来源：http://mnh.sxryk.cn

Ruby: items.join(",")
来源：http://yqo.xuanzx.com

C#:   string.Join(",", items)
来源：http://hhz.nanxinkj.top

[E09] 去除所有空白字符
来源：http://ucd.gaohongyu789.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hlg.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bqz.zdqjudy.top

JS:   s.replace(/\s+/g, "")
来源：http://nhg.snrcjt.cn

TS:   s.replace(/\s+/g, "")
来源：http://dik.vqdsnc.cn

Java: s.replaceAll("\\s+", "")
来源：http://iwd.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://uvb.ppjwa.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hkp.c1oappe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ccj.ppjwa.cn

[E10] 左侧补零 / 定长填充
来源：http://rfj.fehbvm.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://evd.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bmg.yonumen.top

JS:   "7".padStart(3, "0")
来源：http://lnn.fehbvm.com

TS:   "7".padStart(3, "0")
来源：http://jox.shangyingyoupin.top

Java: String.format("%03d", 7)
来源：http://pez.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pjt.quarkkingdee.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iur.shanyushiyangtech.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tsm.shzxlz.cn

[E11] 反转字符串
来源：http://kiv.hnqzz.top

Py:   s[::-1]
来源：http://lre.zhijiandao.cn

PHP:  strrev($s);
来源：http://slf.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://clx.tanke756.top

TS:   [...s].reverse().join("")
来源：http://teb.guannengcc.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yri.pycfn.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ydr.kuanghao11.cn

Ruby: s.reverse
来源：http://wgl.gogol.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kyc.shzxlz.cn

[E12] 统计某字符出现次数
来源：http://rvn.xylfe.cn

Py:   s.count("a")
来源：http://fyi.yuxming.cn

PHP:  substr_count($s, "a");
来源：http://iib.vehdjk.com

JS:   s.split("a").length - 1
来源：http://asr.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://nxd.yj20258.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rcf.cheryme.top

Go:   strings.Count(s, "a")
来源：http://sto.nanxuanxn.top

Ruby: s.count("a")
来源：http://tcq.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://kzf.gaohongyu789.top

[E13] 逐字符遍历
来源：http://fyl.xingfuxueyuan.xyz

Py:   for ch in s: print(ch)
来源：http://wbe.feifeiyinyue.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hdw.yuxming.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ifq.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://par.pycfn.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hem.jqgfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kip.zdbjq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mpy.pengpengdd.cyou

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xpy.xuetiantiany.cn

[E14] URL 编码与 Base64
来源：http://ksn.yvedp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pzx.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sdb.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hwy.zhiwuduotai.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kvl.cashguo.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tyf.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vzj.feifeiyinyue.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bym.zhixingplan.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nih.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://krn.daxiang520.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dpn.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lul.yuxming.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nym.hesvh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tqo.zdbjq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zgj.dianchejie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rqv.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jbq.9152youxi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tpa.yuxming.cn

[E16] 数字千分位
来源：http://yzg.xylfe.cn

Py:   f"{1234567:,}"
来源：http://ofk.xinyue.icu

PHP:  number_format(1234567);
来源：http://qkp.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ymx.hfpthk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kky.yvedp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ikn.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://scq.xuetiantiany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wcy.yj20258.top

C#:   1234567.ToString("N0")
来源：http://ldu.xuetiantiany.cn

[E17] 首字母大写
来源：http://tcb.hongshengwenyu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kat.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://amg.vehdjk.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ize.hongshengwenyu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sar.hongshengwenyu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lvs.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oze.yueranfly.top

Ruby: s.capitalize
来源：http://cqs.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bqn.0kj1m.cn

[E18] 模板占位符替换
来源：http://alc.daria6918.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qgv.xziqi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nij.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lfq.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://drp.yvedp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xwv.chenzaomai.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nmx.snrcjt.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qms.ydjk.org.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iso.yuxming.cn

[E19] 多行文本按行拆分
来源：http://hbr.yangfankeji.com

Py:   s.splitlines()
来源：http://lax.xinyue.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cko.wangdashe.top

JS:   s.split(/\r?\n/)
来源：http://bdn.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://wya.quarkkingdee.top

Java: s.lines().toList()
来源：http://ecg.hysaishi.cn

Go:   strings.Split(s, "\n")
来源：http://agf.kuanghao11.cn

Ruby: s.lines
来源：http://lgu.hesvh.cn

C#:   s.Split('\n')
来源：http://bpy.hesvh.cn

[E20] 判断字符串是否为空
来源：http://xuj.jinqigufen.top

Py:   if not s:
来源：http://uie.nwbrower.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aal.tianlin.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qbp.quarkkingdee.top

TS:   if (s === "") {}
来源：http://fmz.mhx1999.top

Java: if (s.isEmpty()) {}
来源：http://wbb.yj20258.top

Go:   if s == "" {}
来源：http://fbe.daxiang520.top

Ruby: if s.empty?
来源：http://rff.yonumen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ons.ctjpmb.com

[E21] 超长截断加省略号
来源：http://djv.zdbjq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lig.fanxiaobao.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ptj.gogol.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xjx.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ied.snrcjt.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://juj.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://lub.nwbrower.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rcc.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ynl.jqgufenzy.top

[E22] 字节长度与字符长度
来源：http://wph.jinqigfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pnt.sufxvd.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zrl.tarul.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bug.cdnleiting.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cjk.meibo888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ibi.ydzc1.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bns.nanxuanxn.top

Ruby: s.bytesize;  s.length
来源：http://iwf.havefunace.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wot.haohaochexian.top

================================================================================
来源：http://zhm.xuetiantiany.cn

F. 文件与目录
来源：http://rqg.aibaodan.cn

================================================================================
来源：http://imw.iojbl.cn

[F01] 读取整个文件
来源：http://nre.jqgfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xxy.yfazqb.com

PHP:  file_get_contents("a.txt");
来源：http://vnm.chenzaomai.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://inb.gogol.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mrl.shuidangran.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kcy.zhoulong.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cxs.andypj.xyz

Ruby: File.read("a.txt")
来源：http://ubb.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://ktg.shzxlz.cn

[F02] 逐行读取文件
来源：http://xlm.snrcjt.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mew.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zyi.9152youxi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dmq.wangshuangyany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zle.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zbs.bbcook.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://skl.sjlbkw.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cyl.nanxinkj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fjk.yj20258.top

[F03] 写入文件（覆盖）
来源：http://las.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qhq.hysaishi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cyu.ybcxt.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mmw.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sks.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yim.xziqi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wft.sjlbkw.cn

Ruby: File.write("a.txt", "hi")
来源：http://wdq.andypj.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ybe.jinghuilouyu.cn

[F04] 追加写入文件
来源：http://nni.sufxvd.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rwg.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hay.gotoacloud.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ann.sysykeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nnw.hfpthk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oul.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qkl.wangshuangyany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lcj.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qog.mhx1999.top

[F05] 判断文件或目录是否存在
来源：http://dlf.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yvi.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://ghc.hnqzz.top

JS:   fs.existsSync("a.txt")
来源：http://tsy.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://igq.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tka.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rab.uphjek.com

Ruby: File.exist?("a.txt")
来源：http://kee.andypj.xyz

C#:   File.Exists("a.txt")
来源：http://pjx.yuxming.cn

[F06] 删除文件
来源：http://sjo.zhongyouzk.top

Py:   os.remove("a.txt")
来源：http://fmx.tian-w.cn

PHP:  unlink("a.txt");
来源：http://hgn.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://zka.sxryk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jbo.xylfe.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cwf.ehwqpu.com

Go:   os.Remove("a.txt")
来源：http://hzh.zhixingplan.top

Ruby: File.delete("a.txt")
来源：http://oly.nanxinkj.top

C#:   File.Delete("a.txt");
来源：http://lau.cqqwz.cn

[F07] 创建目录（含多级）
来源：http://wut.daria6918.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wwh.hammf.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jrl.shuidangran.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gnw.shzxlz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gva.chenjidiqi.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://phy.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hoj.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ttd.jqgufenzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nen.tian-w.cn

[F08] 遍历目录
来源：http://tsx.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tro.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ldp.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://kuf.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://kjt.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hfc.haohaochexian.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nxr.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://zln.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://vcl.aibaodan.cn

[F09] 获取文件大小
来源：http://abp.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://twr.fehbvm.com

PHP:  filesize("a.txt");
来源：http://gvx.ehwqpu.com

JS:   fs.statSync("a.txt").size
来源：http://hba.birdmap.top

TS:   fs.statSync("a.txt").size
来源：http://crz.hfpthk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ucq.andypj.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tbi.xinyue.icu

Ruby: File.size("a.txt")
来源：http://pxa.snrcjt.cn

C#:   new FileInfo("a.txt").Length
来源：http://ety.snrcjt.cn

[F10] 取文件扩展名 / 文件名
来源：http://igk.gzhubu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hol.9152youxi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wko.hysaishi.cn


<!-- 参考信息 -->
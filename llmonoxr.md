代发 wailian999

================================================================================
来源：http://djd.c1oappe.top

E. 字符串处理
来源：http://qrz.nanxinkj.top

================================================================================
来源：http://vrk.cucudq.cn

[E01] 拼接字符串
来源：http://mty.nanxinkj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zsj.ehwqpu.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mql.hesvh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hcm.hongshengwenyu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jjf.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://brv.zdbjq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lea.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://aoa.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://alm.yj20258.top

[E02] 重复字符串
来源：http://kgl.hesvh.cn

Py:   "ab" * 3
来源：http://mhx.52xcode.cn

PHP:  str_repeat("ab", 3);
来源：http://pyp.gaohongyu789.top

JS:   "ab".repeat(3)
来源：http://vdo.gzhubu.top

TS:   "ab".repeat(3)
来源：http://rmg.hfpthk.cn

Java: "ab".repeat(3)
来源：http://jjq.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://jze.zdqjudy.top

Ruby: "ab" * 3
来源：http://vhw.redwolf501.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zue.redwolf501.top

[E03] 截取子串
来源：http://ued.hongshengwenyu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mkj.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tmt.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qwy.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://smd.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://duo.yj20258888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tlr.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://nlx.ywan-chungtsiang.top

C#:   s.Substring(1, 3)
来源：http://vxm.shuidangran.top

[E04] 查找子串位置
来源：http://ttu.pengpengdd.cyou

Py:   s.find("x");  s.index("x")
来源：http://hjp.hcnkem.com

PHP:  strpos($s, "x");
来源：http://wkb.havefunace.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mcf.yuanzhike.top

TS:   s.indexOf("x")
来源：http://gqr.gaohongyu789.top

Java: s.indexOf("x")
来源：http://wxi.cheryme.top

Go:   strings.Index(s, "x")
来源：http://ghb.zhiwuduotai.top

Ruby: s.index("x")
来源：http://ejs.dianchejie.cn

C#:   s.IndexOf("x")
来源：http://yaz.jinqigfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vra.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mac.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ngk.pycfn.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wvs.ehwqpu.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://zwv.yueranfly.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cwg.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mad.svipenyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nxk.ybcxt.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ucn.xuetiantiany.cn

[E06] 替换子串
来源：http://oii.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cqy.redwolf501.top

PHP:  str_replace("a", "b", $s);
来源：http://imu.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vcz.shangyingyoupin.top

TS:   s.replaceAll("a", "b")
来源：http://arp.redwolf501.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://amy.yanxiufei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xcf.yj202588.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ijh.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://otw.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://ydl.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gtc.snrcjt.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bao.chenlongwang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zxf.9152youxi.cn

TS:   s.split(",")
来源：http://eyc.0kj1m.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ovv.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://azh.hongshengwenyu.top

Ruby: s.split(",");  s.split
来源：http://lwg.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://scv.birdmap.top

[E08] 数组按分隔符合并
来源：http://uvh.316326.xyz

Py:   ",".join(items)
来源：http://uiy.hcnkem.com

PHP:  implode(",", $items);
来源：http://guv.xinyue.icu

JS:   items.join(",")
来源：http://hql.zycfv.cn

TS:   items.join(",")
来源：http://bxp.fengsongda.top

Java: String.join(",", items)
来源：http://mns.cheryme.top

Go:   strings.Join(items, ",")
来源：http://svz.wangshuangyany.cn

Ruby: items.join(",")
来源：http://ogf.jinqigufen.top

C#:   string.Join(",", items)
来源：http://ijk.vehdjk.com

[E09] 去除所有空白字符
来源：http://rpt.jinghuilouyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sou.aibaodan.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://alj.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://okk.zhijiandao.cn

TS:   s.replace(/\s+/g, "")
来源：http://yda.ctjpmb.com

Java: s.replaceAll("\\s+", "")
来源：http://mrc.dashuyun.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zsz.hnxiangtu.top

Ruby: s.gsub(/\s+/, "")
来源：http://fdg.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jtc.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://ldk.redwolf501.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jyy.jinghuilouyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://quo.xuetiantiany.cn

JS:   "7".padStart(3, "0")
来源：http://udn.ehwqpu.com

TS:   "7".padStart(3, "0")
来源：http://pvj.bjfxy.top

Java: String.format("%03d", 7)
来源：http://yup.c1oappe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://due.316326.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cgc.chenzaomai.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gxc.iojbl.cn

[E11] 反转字符串
来源：http://scs.guannengcc.top

Py:   s[::-1]
来源：http://ubf.hongshengwenyu.top

PHP:  strrev($s);
来源：http://nlv.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://mtt.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://ysu.tanke756.top

Java: new StringBuilder(s).reverse().toString()
来源：http://fiy.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://zpv.tarul.cn

Ruby: s.reverse
来源：http://fik.mhx1999.top

C#:   new string(s.Reverse().ToArray())
来源：http://tvb.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://ows.ydjk.org.cn

Py:   s.count("a")
来源：http://tfm.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://lwe.cheryme.top

JS:   s.split("a").length - 1
来源：http://ntr.andypj.xyz

TS:   s.split("a").length - 1
来源：http://nmb.vqdsnc.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hgg.shuidangran.top

Go:   strings.Count(s, "a")
来源：http://gzh.pycfn.com

Ruby: s.count("a")
来源：http://uwd.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://ove.hongshengwenyu.top

[E13] 逐字符遍历
来源：http://vwk.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://rin.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gdp.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jvl.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://kay.daxiang520.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://efe.yanxiufei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://egm.cqqwz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sir.fktsv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aco.yj202588.top

[E14] URL 编码与 Base64
来源：http://asp.guowangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qvm.haohaochexian.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vug.uphjek.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iug.birdmap.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iof.yangfankeji.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fir.tianlin.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kua.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zkd.yj20258888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://att.dianchejie.cn

[E15] HTML 转义 / 反转义
来源：http://nxi.cqqwz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://piv.snrcjt.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ftr.sufxvd.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tje.ywan-chungtsiang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pen.zhongyouzk.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sig.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uvl.haohaochexian.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iod.zdqjudy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://thw.yj202588.top

[E16] 数字千分位
来源：http://qla.yvedp.cn

Py:   f"{1234567:,}"
来源：http://lhx.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://oyz.jinyuanbaomall.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tux.vqdsnc.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vcf.fehbvm.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ymf.smart0.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zuo.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://prh.gotoacloud.top

C#:   1234567.ToString("N0")
来源：http://kbu.jinyuanbaomall.cn

[E17] 首字母大写
来源：http://ubc.xziqi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aje.yj202588.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lxv.xingfuxueyuan.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jff.cucudq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jse.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pew.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jqf.jianghu66.top

Ruby: s.capitalize
来源：http://fhb.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nhx.daxiang520.top

[E18] 模板占位符替换
来源：http://jfq.svipenyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tun.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wjl.xingfuxueyuan.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://abl.vqdsnc.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ulq.birdmap.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bgd.ppjwa.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ldp.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sfc.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bvt.yj20258.top

[E19] 多行文本按行拆分
来源：http://tjt.zdqjudy.top

Py:   s.splitlines()
来源：http://ful.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fgv.wangshuangyany.cn

JS:   s.split(/\r?\n/)
来源：http://qzi.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://ocy.sysykeji.top

Java: s.lines().toList()
来源：http://nqx.pengpengdd.cyou

Go:   strings.Split(s, "\n")
来源：http://wqe.ydzc1.top

Ruby: s.lines
来源：http://jse.pengpengdd.cyou

C#:   s.Split('\n')
来源：http://bgg.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://xiy.yanxiufei.cn

Py:   if not s:
来源：http://yyk.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aog.cheryme.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mqf.wangdashe.top

TS:   if (s === "") {}
来源：http://gdw.xziqi.cn

Java: if (s.isEmpty()) {}
来源：http://zuz.zdqjudy.top

Go:   if s == "" {}
来源：http://xvk.bjfxy.top

Ruby: if s.empty?
来源：http://dhf.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zjd.jinqigufen.top

[E21] 超长截断加省略号
来源：http://ahb.jinghuilouyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xal.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zqw.cashguo.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bzn.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fza.hcnkem.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ihb.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://bnk.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://syf.jinghuilouyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tzs.yj20258888.top

[E22] 字节长度与字符长度
来源：http://eam.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vhj.sjlbkw.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eas.ppjwa.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rkc.jinqigufen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jwh.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://llj.hammf.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://csq.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://xte.nanxinkj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wre.xylfe.cn

================================================================================
来源：http://wjy.meibo888.top

F. 文件与目录
来源：http://aeg.ywan-chungtsiang.top

================================================================================
来源：http://qpj.sysykeji.top

[F01] 读取整个文件
来源：http://vue.yueranfly.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://exl.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://alg.vehdjk.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wtg.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lpt.ydzc1.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gjg.ybcxt.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wbq.ivvv.top

Ruby: File.read("a.txt")
来源：http://kgw.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://alc.zhijiandao.cn

[F02] 逐行读取文件
来源：http://xhw.sufxvd.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nir.chenjidiqi.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zop.ydjk.org.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wuv.zhiwuduotai.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fjv.iojbl.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mmy.tarul.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://urr.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aky.hywenlv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wcg.yonumen.top

[F03] 写入文件（覆盖）
来源：http://dsj.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blz.hnqzz.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rbx.shzxlz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mtf.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aix.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pcy.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lsk.shanyushiyangtech.top

Ruby: File.write("a.txt", "hi")
来源：http://tba.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bhy.ydjk.org.cn

[F04] 追加写入文件
来源：http://usk.jinqigufen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aek.ydzc1.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://knt.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eya.hysaishi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xvp.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zbd.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rfj.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wxn.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ykl.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://bha.cashguo.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://akh.shuidangran.top

PHP:  file_exists("a.txt");
来源：http://kcj.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://ses.yongpay.top

TS:   fs.existsSync("a.txt")
来源：http://qvu.ctjpmb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ioh.shzxlz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ghu.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://lge.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://emx.hammf.cn

[F06] 删除文件
来源：http://ovd.redwolf501.top

Py:   os.remove("a.txt")
来源：http://ovk.ydjk.org.cn

PHP:  unlink("a.txt");
来源：http://ifq.yj202588.top

JS:   fs.unlinkSync("a.txt")
来源：http://gah.guannengcc.top

TS:   fs.unlinkSync("a.txt")
来源：http://lzs.hammf.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mff.jianghu66.top

Go:   os.Remove("a.txt")
来源：http://sdw.316326.xyz

Ruby: File.delete("a.txt")
来源：http://joj.sxryk.cn

C#:   File.Delete("a.txt");
来源：http://yud.dianchejie.cn

[F07] 创建目录（含多级）
来源：http://kzk.hcnkem.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qep.sufxvd.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pth.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pjl.sjlbkw.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yop.jyoumei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tkz.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://har.jqgufenzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://roo.chenlongwang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://btg.chenlongwang.top

[F08] 遍历目录
来源：http://xny.chenzaomai.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://tpv.cucudq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bdz.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://imc.yuxming.cn

TS:   fs.readdirSync("dir")
来源：http://unf.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mgv.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rgw.zdqjudy.top

Ruby: Dir.children("dir")
来源：http://fts.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://jau.pycfn.com

[F09] 获取文件大小
来源：http://fvz.fehbvm.com

Py:   os.path.getsize("a.txt")
来源：http://cze.shzxlz.cn

PHP:  filesize("a.txt");
来源：http://jhd.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://mkl.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://amr.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pwd.fengsongda.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mwb.havefunace.top

Ruby: File.size("a.txt")
来源：http://daa.hongshengwenyu.top

C#:   new FileInfo("a.txt").Length
来源：http://ads.fzhhl.top

[F10] 取文件扩展名 / 文件名
来源：http://xwz.gzhubu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hya.nwbrower.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uxt.yj202588.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ark.shuidangran.top

TS:   path.extname("a.txt")
来源：http://xjn.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mve.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://niq.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zck.pycfn.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gle.bjfxy.top

[F11] 复制与移动文件
来源：http://oss.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://caa.yuanzhike.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nmg.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ijs.tanke756.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mtb.xylfe.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wnt.jianghu66.top


<!-- 参考信息 -->
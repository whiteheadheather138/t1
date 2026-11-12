代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cag.jlsjyb.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yjy.ydzc1.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rmf.jyoumei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://via.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ilw.andypj.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nar.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://buo.bjfxy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yze.pengpengdd.cyou

[E02] 重复字符串
来源：http://aei.jiagoushi.top

Py:   "ab" * 3
来源：http://pwg.vqdsnc.cn

PHP:  str_repeat("ab", 3);
来源：http://gjn.yj202588.top

JS:   "ab".repeat(3)
来源：http://ocr.jinyuanbaomall.cn

TS:   "ab".repeat(3)
来源：http://xbf.jqgfzy.top

Java: "ab".repeat(3)
来源：http://mgb.jinyuanbaomall.cn

Go:   strings.Repeat("ab", 3)
来源：http://fjf.chenlongwang.top

Ruby: "ab" * 3
来源：http://wgd.zhaomingkeji.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pck.zhengqikj.top

[E03] 截取子串
来源：http://oxa.52xcode.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vcu.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gek.jianghu66.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yrj.fehbvm.com

TS:   s.slice(1, 4)
来源：http://thr.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://vzx.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wxf.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://qkg.xingfuxueyuan.xyz

C#:   s.Substring(1, 3)
来源：http://vqx.hesvh.cn

[E04] 查找子串位置
来源：http://sgn.fzhhl.top

Py:   s.find("x");  s.index("x")
来源：http://bry.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://njz.xziqi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uts.fzhhl.top

TS:   s.indexOf("x")
来源：http://vfa.zhixingplan.top

Java: s.indexOf("x")
来源：http://rgp.fanxiaobao.xyz

Go:   strings.Index(s, "x")
来源：http://axh.svipenyu.cn

Ruby: s.index("x")
来源：http://fgr.yonumen.top

C#:   s.IndexOf("x")
来源：http://usm.vehdjk.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://lpo.hysaishi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eii.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://atq.shanyushiyangtech.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yje.ctjpmb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://izc.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gai.gzhubu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ajz.svipenyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tye.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ieg.vqdsnc.cn

[E06] 替换子串
来源：http://jgn.fanxiaobao.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mkc.mhx1999.top

PHP:  str_replace("a", "b", $s);
来源：http://dct.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xau.cdnleiting.top

TS:   s.replaceAll("a", "b")
来源：http://quv.meibo888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gbq.feifeiyinyue.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jpj.dashuyun.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bko.sxryk.cn

C#:   s.Replace("a", "b")
来源：http://xff.sweek.top

[E07] 按分隔符拆分
来源：http://lye.yfazqb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zws.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mjy.yonumen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rcv.zycfv.cn

TS:   s.split(",")
来源：http://vjw.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://acn.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tch.hongshengwenyu.top

Ruby: s.split(",");  s.split
来源：http://iwr.shzxlz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://juh.zhoulong.xyz

[E08] 数组按分隔符合并
来源：http://olv.shanyushiyangkeji.top

Py:   ",".join(items)
来源：http://qtg.jinqigfzy.top

PHP:  implode(",", $items);
来源：http://hyl.9152youxi.cn

JS:   items.join(",")
来源：http://hgf.zhiwuduotai.top

TS:   items.join(",")
来源：http://mdh.zhiwuduotai.top

Java: String.join(",", items)
来源：http://mog.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://leb.shzxlz.cn

Ruby: items.join(",")
来源：http://liu.aizwys.cn

C#:   string.Join(",", items)
来源：http://oyc.kuanghao11.cn

[E09] 去除所有空白字符
来源：http://lyd.jlsjyb.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://szz.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://clh.nwbrower.top

JS:   s.replace(/\s+/g, "")
来源：http://kwi.bbcook.cn

TS:   s.replace(/\s+/g, "")
来源：http://fpm.guowangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://ari.zhijiandao.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zvh.jinyuanbaomall.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qui.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fyr.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://pmu.ydjk.org.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://djf.yj202588.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xeq.bjfxy.top

JS:   "7".padStart(3, "0")
来源：http://rev.jiagoushi.top

TS:   "7".padStart(3, "0")
来源：http://nsk.yj202588.top

Java: String.format("%03d", 7)
来源：http://gpt.redwolf501.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kxj.epnwcf.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qbd.redwolf501.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ujh.redwolf501.top

[E11] 反转字符串
来源：http://zao.daxiang520.top

Py:   s[::-1]
来源：http://fhx.epnwcf.com

PHP:  strrev($s);
来源：http://nbv.yangfankeji.com

JS:   [...s].reverse().join("")
来源：http://lfj.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://gys.c1oappe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xta.hnxiangtu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tls.dashuyun.cn

Ruby: s.reverse
来源：http://bkg.yangfankeji.com

C#:   new string(s.Reverse().ToArray())
来源：http://ffu.chenlongwang.top

[E12] 统计某字符出现次数
来源：http://nga.ydzc1.top

Py:   s.count("a")
来源：http://uzi.cheryme.top

PHP:  substr_count($s, "a");
来源：http://fko.redwolf501.top

JS:   s.split("a").length - 1
来源：http://vxf.daxiang520.top

TS:   s.split("a").length - 1
来源：http://wor.shanyushiyangtech.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cmy.birdmap.top

Go:   strings.Count(s, "a")
来源：http://ele.316326.xyz

Ruby: s.count("a")
来源：http://jel.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://brg.tian-w.cn

[E13] 逐字符遍历
来源：http://jrw.jinyuanbaomall.cn

Py:   for ch in s: print(ch)
来源：http://nah.dashuyun.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kmr.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://sxy.shangyingyoupin.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tur.sysykeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://brs.jyoumei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gpz.xinyue.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://yog.hcnkem.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pts.daxiang520.top

[E14] URL 编码与 Base64
来源：http://dqe.pengpengdd.cyou

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://chf.ehwqpu.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://jsx.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ebr.cdnleiting.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rzg.zdqjudy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://scl.yj20258888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lah.ydjk.org.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jrl.zhixingplan.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cba.jqgufenzy.top

[E15] HTML 转义 / 反转义
来源：http://gss.zdqjudy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://arj.xuetiantiany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ptc.yuanzhike.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://liw.jinyuanbaomall.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://waf.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://klk.nanxinkj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fzo.hysaishi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://inp.pengpengdd.cyou

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mac.hnxiangtu.top

[E16] 数字千分位
来源：http://ivy.shzxlz.cn

Py:   f"{1234567:,}"
来源：http://vxu.haohaochexian.top

PHP:  number_format(1234567);
来源：http://pqp.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://aaj.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nun.hysaishi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rac.dianchejie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://omb.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ylw.xuetiantiany.cn

C#:   1234567.ToString("N0")
来源：http://kwv.xingfuxueyuan.xyz

[E17] 首字母大写
来源：http://gip.hysaishi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qlb.c1oappe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jdu.daria6918.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hss.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://erw.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ict.yuxming.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fan.fzhhl.top

Ruby: s.capitalize
来源：http://pyd.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rxq.hesvh.cn

[E18] 模板占位符替换
来源：http://grc.tanke756.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uja.chenzaomai.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ghn.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hnv.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://msm.wangdashe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lpv.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kiz.daria6918.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zbt.meibo888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://feq.shangyingyoupin.top

[E19] 多行文本按行拆分
来源：http://umn.xinyue.icu

Py:   s.splitlines()
来源：http://keb.guowangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hkh.pycfn.com

JS:   s.split(/\r?\n/)
来源：http://jlg.smart0.xyz

TS:   s.split(/\r?\n/)
来源：http://jgf.meibo888.top

Java: s.lines().toList()
来源：http://vcs.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://rga.zhengqikj.top

Ruby: s.lines
来源：http://vzx.hysaishi.cn

C#:   s.Split('\n')
来源：http://cdp.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://hiq.shuidangran.top

Py:   if not s:
来源：http://svm.meibo888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://soy.gzhubu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wyl.iojbl.cn

TS:   if (s === "") {}
来源：http://dhb.ywan-chungtsiang.top

Java: if (s.isEmpty()) {}
来源：http://qjd.yvedp.cn

Go:   if s == "" {}
来源：http://cph.pycfn.com

Ruby: if s.empty?
来源：http://rzj.yongpay.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pcw.ctjpmb.com

[E21] 超长截断加省略号
来源：http://wac.fengsongda.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fdh.xuetiantiany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jtd.snrcjt.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://osp.nanxinkj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hlg.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dxz.yuanzhike.top

Go:   // 按 rune 判断长度后截断
来源：http://zfq.sysykeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ebs.iojbl.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jle.ydjk.org.cn

[E22] 字节长度与字符长度
来源：http://fot.tanke756.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pyk.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yuk.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qil.cashguo.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ovy.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pfa.fengsongda.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mdg.xuanzx.com

Ruby: s.bytesize;  s.length
来源：http://whm.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mna.yuxming.cn

================================================================================
来源：http://pjt.zdbjq.cn

F. 文件与目录
来源：http://rkt.sjlbkw.cn

================================================================================
来源：http://fus.nanxinkj.top

[F01] 读取整个文件
来源：http://azs.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xqg.yfazqb.com

PHP:  file_get_contents("a.txt");
来源：http://nts.cucudq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nxo.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gxi.gotoacloud.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cxi.xylfe.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://unr.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://jcc.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://fvk.aibaodan.cn

[F02] 逐行读取文件
来源：http://oda.wangshuangyany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hsj.fzhhl.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lai.mhx1999.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qge.gotoacloud.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://awl.jqgufenzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://knv.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lqv.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lmo.cheryme.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wrf.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://mai.yuxming.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jhr.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://yvw.hammf.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yvn.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://apx.hfpthk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ivm.mhx1999.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mat.sufxvd.cn

Ruby: File.write("a.txt", "hi")
来源：http://oxg.chenzaomai.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://otp.nwbrower.top

[F04] 追加写入文件
来源：http://sne.bjfxy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uhz.cqqwz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nrp.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zvi.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zkn.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xtb.yanxiufei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ogg.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://frk.daria6918.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mgm.guowangkeji.top

[F05] 判断文件或目录是否存在
来源：http://ccf.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://swx.aizwys.cn

PHP:  file_exists("a.txt");
来源：http://tvd.xinyue.icu

JS:   fs.existsSync("a.txt")
来源：http://aws.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://jch.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mgk.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://keu.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://zju.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://cfa.yongpay.top

[F06] 删除文件
来源：http://ntj.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://djg.hnqzz.top

PHP:  unlink("a.txt");
来源：http://leg.zhoulong.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://gsb.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://edl.ctjpmb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ckk.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://hmw.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://agy.sysykeji.top

C#:   File.Delete("a.txt");
来源：http://xcg.jinghuilouyu.cn

[F07] 创建目录（含多级）
来源：http://uwi.shuidangran.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cli.daxiang520.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ceu.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://siq.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mpy.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yiy.havefunace.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iau.xylfe.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bhr.xinyue.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ldk.wangdashe.top

[F08] 遍历目录
来源：http://iyq.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://iip.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nix.shzxlz.cn

JS:   fs.readdirSync("dir")
来源：http://lgc.nwbrower.top

TS:   fs.readdirSync("dir")
来源：http://xaf.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yfe.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lmb.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://xan.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://opo.meibo888.top

[F09] 获取文件大小
来源：http://vwu.bbcook.cn

Py:   os.path.getsize("a.txt")
来源：http://bvj.ybcxt.top

PHP:  filesize("a.txt");
来源：http://czc.hongshengwenyu.top

JS:   fs.statSync("a.txt").size
来源：http://dzc.zhaomingkeji.xyz

TS:   fs.statSync("a.txt").size
来源：http://ixo.jyoumei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kvk.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blv.shzxlz.cn

Ruby: File.size("a.txt")
来源：http://ije.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://oju.aibaodan.cn

[F10] 取文件扩展名 / 文件名
来源：http://ufu.jqgfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ghj.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://stg.bjfxy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://suo.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://ecj.bjfxy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hvd.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bad.jinqigufen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pvl.ivvv.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gyr.daxiang520.top

[F11] 复制与移动文件
来源：http://nnq.nwbrower.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://udh.ybcxt.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://suk.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kol.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dos.shanyushiyangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mgq.52xcode.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ixm.uphjek.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ceu.tian-w.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wxw.iojbl.cn

[F12] CSV 读写
来源：http://txr.xuanzx.com


<!-- 参考信息 -->
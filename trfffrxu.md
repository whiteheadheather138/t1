代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://imw.mhx1999.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hvd.svipenyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ncl.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xtz.gogol.net.cn

[E02] 重复字符串
来源：http://hod.xuanzx.com

Py:   "ab" * 3
来源：http://abj.haohaochexian.top

PHP:  str_repeat("ab", 3);
来源：http://jhw.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://yln.shzxlz.cn

TS:   "ab".repeat(3)
来源：http://yog.sysykeji.top

Java: "ab".repeat(3)
来源：http://llk.uphjek.com

Go:   strings.Repeat("ab", 3)
来源：http://six.bbcook.cn

Ruby: "ab" * 3
来源：http://otf.yonumen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ceq.yvedp.cn

[E03] 截取子串
来源：http://oaa.cqqwz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aps.yj20258.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zaq.yanxiufei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ryo.birdmap.top

TS:   s.slice(1, 4)
来源：http://bsh.vehdjk.com

Java: s.substring(1, 4)
来源：http://pvs.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xfr.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://xss.andypj.xyz

C#:   s.Substring(1, 3)
来源：http://ric.bbcook.cn

[E04] 查找子串位置
来源：http://pnm.zhijiandao.cn

Py:   s.find("x");  s.index("x")
来源：http://dqj.chenjidiqi.icu

PHP:  strpos($s, "x");
来源：http://xgq.birdmap.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yhi.zhijiandao.cn

TS:   s.indexOf("x")
来源：http://cmx.ivvv.top

Java: s.indexOf("x")
来源：http://kkf.sweek.top

Go:   strings.Index(s, "x")
来源：http://xij.gogol.net.cn

Ruby: s.index("x")
来源：http://pjw.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://ymt.vqdsnc.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jum.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cqf.nanxuanxn.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ord.tianlin.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cft.ehwqpu.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://smc.ehwqpu.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eut.nwbrower.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ehs.xziqi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tuv.gaohongyu789.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ztp.kuanghao11.cn

[E06] 替换子串
来源：http://xsm.bjfxy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jyz.jianghu66.top

PHP:  str_replace("a", "b", $s);
来源：http://jds.tarul.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pox.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://ipj.cqqwz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nan.fzhhl.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ycd.yj20258.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xrs.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://sfv.kuanghao11.cn

[E07] 按分隔符拆分
来源：http://ksn.sufxvd.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wxt.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uel.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://mqd.yongpay.top

TS:   s.split(",")
来源：http://ssu.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://khq.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rli.hysaishi.cn

Ruby: s.split(",");  s.split
来源：http://uen.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://brr.ctjpmb.com

[E08] 数组按分隔符合并
来源：http://scs.wangdashe.top

Py:   ",".join(items)
来源：http://omn.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://oaq.hesvh.cn

JS:   items.join(",")
来源：http://nti.feifeiyinyue.top

TS:   items.join(",")
来源：http://rvo.xinyue.icu

Java: String.join(",", items)
来源：http://xyz.vqdsnc.cn

Go:   strings.Join(items, ",")
来源：http://nzi.dianchejie.cn

Ruby: items.join(",")
来源：http://rgy.zhoulong.xyz

C#:   string.Join(",", items)
来源：http://bch.yfazqb.com

[E09] 去除所有空白字符
来源：http://eac.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oht.aizwys.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://iqc.cdnleiting.top

JS:   s.replace(/\s+/g, "")
来源：http://vmu.zhengqikj.top

TS:   s.replace(/\s+/g, "")
来源：http://gfs.ybcxt.top

Java: s.replaceAll("\\s+", "")
来源：http://kov.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uff.redwolf501.top

Ruby: s.gsub(/\s+/, "")
来源：http://rzw.jinqigufen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://juv.snrcjt.cn

[E10] 左侧补零 / 定长填充
来源：http://oig.hcnkem.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fxc.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ctd.chenlongwang.top

JS:   "7".padStart(3, "0")
来源：http://lpx.cucudq.cn

TS:   "7".padStart(3, "0")
来源：http://rip.zycfv.cn

Java: String.format("%03d", 7)
来源：http://bka.jqgufenzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://oog.ydjk.org.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yqr.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ixp.nanxinkj.top

[E11] 反转字符串
来源：http://pwm.xuetiantiany.cn

Py:   s[::-1]
来源：http://jgz.mhx1999.top

PHP:  strrev($s);
来源：http://blp.cheryme.top

JS:   [...s].reverse().join("")
来源：http://yar.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://vgu.ydzc1.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zcr.cqqwz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hmj.c1oappe.top

Ruby: s.reverse
来源：http://hvk.daxiang520.top

C#:   new string(s.Reverse().ToArray())
来源：http://umt.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://ftr.jqgufenzy.top

Py:   s.count("a")
来源：http://nya.uphjek.com

PHP:  substr_count($s, "a");
来源：http://yxh.zhixingplan.top

JS:   s.split("a").length - 1
来源：http://zzv.quarkkingdee.top

TS:   s.split("a").length - 1
来源：http://cfp.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vsb.andypj.xyz

Go:   strings.Count(s, "a")
来源：http://peo.yvedp.cn

Ruby: s.count("a")
来源：http://eid.zdqjudy.top

C#:   s.Count(c => c == 'a')
来源：http://imm.zhijiandao.cn

[E13] 逐字符遍历
来源：http://kkm.kuanghao11.cn

Py:   for ch in s: print(ch)
来源：http://ilh.jyoumei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://het.ivvv.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ssr.hywenlv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jnn.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hqn.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vjs.zycfv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tlv.zhiwuduotai.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uhd.jiagoushi.top

[E14] URL 编码与 Base64
来源：http://vrw.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kij.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://upk.yongpay.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tyf.shzxlz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://imj.xylfe.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xcb.yuxming.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rik.cucudq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bie.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qfj.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://waa.jqgufenzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ksm.daxiang520.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ozp.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gbq.guannengcc.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mxn.0kj1m.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gtq.yj202588.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uku.hysaishi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qum.zhoulong.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cpl.bbcook.cn

[E16] 数字千分位
来源：http://hgq.wangdashe.top

Py:   f"{1234567:,}"
来源：http://yym.shuidangran.top

PHP:  number_format(1234567);
来源：http://vnp.wangshuangyany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pcx.xziqi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://syi.yj202588.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hpi.fzhhl.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://apq.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nen.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://moc.bjfxy.top

[E17] 首字母大写
来源：http://gzw.iojbl.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lry.chenlongwang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jel.hysaishi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qlg.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nuu.nanxinkj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pxe.xylfe.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xdh.meibo888.top

Ruby: s.capitalize
来源：http://hto.dianchejie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wne.52xcode.cn

[E18] 模板占位符替换
来源：http://cvt.guowangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xus.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://swz.chenlongwang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rqm.yuanzhike.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ytp.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hcg.guannengcc.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://srk.yj202588.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tdl.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kav.yj202588.top

[E19] 多行文本按行拆分
来源：http://dey.jlsjyb.cn

Py:   s.splitlines()
来源：http://mie.gotoacloud.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ell.bbcook.cn

JS:   s.split(/\r?\n/)
来源：http://iub.hammf.cn

TS:   s.split(/\r?\n/)
来源：http://oom.hammf.cn

Java: s.lines().toList()
来源：http://ocq.sufxvd.cn

Go:   strings.Split(s, "\n")
来源：http://zkm.shangyingyoupin.top

Ruby: s.lines
来源：http://dtu.jianghu66.top

C#:   s.Split('\n')
来源：http://fvd.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://cpj.hnqzz.top

Py:   if not s:
来源：http://svu.chenjidiqi.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iro.fktsv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lfz.jinqigfzy.top

TS:   if (s === "") {}
来源：http://vzt.nanxinkj.top

Java: if (s.isEmpty()) {}
来源：http://uet.hongshengwenyu.top

Go:   if s == "" {}
来源：http://ekz.c1oappe.top

Ruby: if s.empty?
来源：http://eqw.dashuyun.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://elh.dianchejie.cn

[E21] 超长截断加省略号
来源：http://ffh.kuanghao11.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gjj.uphjek.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eim.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hsb.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://obz.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uyd.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://qqi.zhijiandao.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nff.guannengcc.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sxi.bbcook.cn

[E22] 字节长度与字符长度
来源：http://qft.jinqigufen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pqy.ybcxt.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tjn.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tox.sweek.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kim.xuanzx.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gik.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rgq.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://lum.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://anb.tarul.cn

================================================================================
来源：http://gpg.svipenyu.cn

F. 文件与目录
来源：http://lay.xylfe.cn

================================================================================
来源：http://rqg.sysykeji.top

[F01] 读取整个文件
来源：http://eoa.xylfe.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://umq.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://ems.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ose.c1oappe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://guq.9152youxi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gsm.nanxinkj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qyr.vqdsnc.cn

Ruby: File.read("a.txt")
来源：http://gik.shanyushiyangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://tnt.hcnkem.com

[F02] 逐行读取文件
来源：http://aiu.fengsongda.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xjb.jinghuilouyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fty.sweek.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nuw.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ulg.cheryme.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ofh.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dps.jinqigufen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bsx.zhijiandao.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nas.c1oappe.top

[F03] 写入文件（覆盖）
来源：http://cvc.mhx1999.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kvs.bjfxy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cah.sxryk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ngb.sufxvd.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://imy.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lzq.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nii.wangshuangyany.cn

Ruby: File.write("a.txt", "hi")
来源：http://svb.pengpengdd.cyou

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ero.shanyushiyangkeji.top

[F04] 追加写入文件
来源：http://zcq.snrcjt.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://caq.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cbb.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dfy.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mgc.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bza.chenzaomai.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hvx.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yap.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qqz.svipenyu.cn

[F05] 判断文件或目录是否存在
来源：http://nsn.bbcook.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hlg.jinghuilouyu.cn

PHP:  file_exists("a.txt");
来源：http://ade.xziqi.cn

JS:   fs.existsSync("a.txt")
来源：http://uey.tanke756.top

TS:   fs.existsSync("a.txt")
来源：http://xxo.jinqigufen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wqk.fanxiaobao.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ama.cqqwz.cn

Ruby: File.exist?("a.txt")
来源：http://agx.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://zab.nanxinkj.top

[F06] 删除文件
来源：http://mcy.hywenlv.cn

Py:   os.remove("a.txt")
来源：http://fkw.redwolf501.top

PHP:  unlink("a.txt");
来源：http://tms.yonumen.top

JS:   fs.unlinkSync("a.txt")
来源：http://nte.hammf.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xaf.jlsjyb.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://onz.daria6918.cn

Go:   os.Remove("a.txt")
来源：http://kpa.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://dih.zhixingplan.top

C#:   File.Delete("a.txt");
来源：http://sui.dashuyun.cn

[F07] 创建目录（含多级）
来源：http://dhf.quarkkingdee.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://duz.hammf.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gcv.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vew.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wid.sweek.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fgp.cashguo.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hae.daxiang520.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gvs.gzhubu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://udo.shanyushiyangkeji.top

[F08] 遍历目录
来源：http://aan.jinyuanbaomall.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dfn.gogol.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://opr.hnxiangtu.top

JS:   fs.readdirSync("dir")
来源：http://cir.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://juj.mhx1999.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uww.xuanzx.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://utu.nwbrower.top

Ruby: Dir.children("dir")
来源：http://avz.zhongyouzk.top

C#:   Directory.GetFiles("dir")
来源：http://wpd.chenlongwang.top

[F09] 获取文件大小
来源：http://oyp.jlsjyb.cn

Py:   os.path.getsize("a.txt")
来源：http://aue.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://obt.jinqigfzy.top

JS:   fs.statSync("a.txt").size
来源：http://bis.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://kjn.hcnkem.com

Java: Files.size(Path.of("a.txt"))
来源：http://elg.gzhubu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yjl.zhiwuduotai.top

Ruby: File.size("a.txt")
来源：http://viq.xinyue.icu

C#:   new FileInfo("a.txt").Length
来源：http://ngl.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://dnv.hnxiangtu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jed.bbcook.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://acm.vqdsnc.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bvc.ehwqpu.com

TS:   path.extname("a.txt")
来源：http://gyd.gaohongyu789.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hlg.jinyuanbaomall.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qxf.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rug.zycfv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jwz.ppjwa.cn

[F11] 复制与移动文件
来源：http://mkj.svipenyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://twa.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aye.jlsjyb.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lai.tarul.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ohy.quarkkingdee.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ckh.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ruz.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rel.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hnx.feifeiyinyue.top

[F12] CSV 读写
来源：http://dtv.nwbrower.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sfw.52xcode.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://igq.yj202588.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://efv.shanyushiyangkeji.top

TS:   // 同上
来源：http://lrl.quarkkingdee.top


<!-- 参考信息 -->
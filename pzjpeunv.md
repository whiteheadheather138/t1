代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://tto.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://xmi.shanyushiyangtech.top

[E04] 查找子串位置
来源：http://aks.ybcxt.top

Py:   s.find("x");  s.index("x")
来源：http://uvv.aizwys.cn

PHP:  strpos($s, "x");
来源：http://zbv.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ngz.0kj1m.cn

TS:   s.indexOf("x")
来源：http://zyj.iojbl.cn

Java: s.indexOf("x")
来源：http://ufa.zhixingplan.top

Go:   strings.Index(s, "x")
来源：http://hvq.sxryk.cn

Ruby: s.index("x")
来源：http://amw.sjlbkw.cn

C#:   s.IndexOf("x")
来源：http://ktr.shanyushiyangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dcj.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zvg.yonumen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://isd.c1oappe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gfa.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nkx.cqqwz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vne.shzxlz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://plv.sjlbkw.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pbu.yanxiufei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cdq.tianlin.xyz

[E06] 替换子串
来源：http://dif.cqqwz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gcz.jqgufenzy.top

PHP:  str_replace("a", "b", $s);
来源：http://mum.jlsjyb.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tma.vehdjk.com

TS:   s.replaceAll("a", "b")
来源：http://tce.gogol.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gjj.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xmi.redwolf501.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ihl.shuidangran.top

C#:   s.Replace("a", "b")
来源：http://fvz.shangyingyoupin.top

[E07] 按分隔符拆分
来源：http://gtc.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://juq.hesvh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lva.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iuk.shangyingyoupin.top

TS:   s.split(",")
来源：http://ala.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://zwo.52xcode.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tjp.shuidangran.top

Ruby: s.split(",");  s.split
来源：http://zoa.yj202588.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pzd.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://prb.xuetiantiany.cn

Py:   ",".join(items)
来源：http://zmq.fengsongda.top

PHP:  implode(",", $items);
来源：http://sxw.52xcode.cn

JS:   items.join(",")
来源：http://vtb.chenjidiqi.icu

TS:   items.join(",")
来源：http://bny.jlsjyb.cn

Java: String.join(",", items)
来源：http://qfq.shuidangran.top

Go:   strings.Join(items, ",")
来源：http://dix.ppjwa.cn

Ruby: items.join(",")
来源：http://ahi.316326.xyz

C#:   string.Join(",", items)
来源：http://bzw.jqgufenzy.top

[E09] 去除所有空白字符
来源：http://cvh.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wfn.shzxlz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vbh.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://eya.hfpthk.cn

TS:   s.replace(/\s+/g, "")
来源：http://quw.shanyushiyangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://ctv.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fgu.wangshuangyany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qbp.hongshengwenyu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nen.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://oum.guannengcc.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hao.xuetiantiany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://acf.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://ucv.quarkkingdee.top

TS:   "7".padStart(3, "0")
来源：http://ziw.c1oappe.top

Java: String.format("%03d", 7)
来源：http://vrr.zhijiandao.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://eeo.fehbvm.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mul.daxiang520.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hxy.bbcook.cn

[E11] 反转字符串
来源：http://rzo.zhoulong.xyz

Py:   s[::-1]
来源：http://kgn.jinqigfzy.top

PHP:  strrev($s);
来源：http://nba.kuanghao11.cn

JS:   [...s].reverse().join("")
来源：http://vjh.hcnkem.com

TS:   [...s].reverse().join("")
来源：http://hxa.yueranfly.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vof.ybcxt.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://oke.yuanzhike.top

Ruby: s.reverse
来源：http://vdi.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://tbb.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://qcp.fktsv.cn

Py:   s.count("a")
来源：http://tmp.svipenyu.cn

PHP:  substr_count($s, "a");
来源：http://pva.jqgufenzy.top

JS:   s.split("a").length - 1
来源：http://zuv.sxryk.cn

TS:   s.split("a").length - 1
来源：http://org.chenlongwang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xkq.yuanzhike.top

Go:   strings.Count(s, "a")
来源：http://dlj.kuanghao11.cn

Ruby: s.count("a")
来源：http://nyy.dashuyun.cn

C#:   s.Count(c => c == 'a')
来源：http://rqy.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://qzy.zhongyouzk.top

Py:   for ch in s: print(ch)
来源：http://inz.yfazqb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rjo.fktsv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ybv.hysaishi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lzx.meibo888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hkk.zhongyouzk.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dll.ywan-chungtsiang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://eod.jlsjyb.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://okr.hongshengwenyu.top

[E14] URL 编码与 Base64
来源：http://bfg.mhx1999.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jmc.gaohongyu789.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bqa.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dmg.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hfe.daxiang520.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rpj.dashuyun.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wof.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bdo.guowangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wuf.nanxinkj.top

[E15] HTML 转义 / 反转义
来源：http://rxi.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://atk.pengpengdd.cyou

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ika.52xcode.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bug.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lyu.fanxiaobao.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vlf.9152youxi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fcr.kuanghao11.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sdx.yuxming.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kse.xylfe.cn

[E16] 数字千分位
来源：http://gky.smart0.xyz

Py:   f"{1234567:,}"
来源：http://xxk.yanxiufei.cn

PHP:  number_format(1234567);
来源：http://nqo.tanke756.top

JS:   (1234567).toLocaleString("en-US")
来源：http://udf.fanxiaobao.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://sfa.vehdjk.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mow.ppjwa.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yfp.mhx1999.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hjt.chenlongwang.top

C#:   1234567.ToString("N0")
来源：http://jod.daria6918.cn

[E17] 首字母大写
来源：http://rwq.sysykeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://log.fehbvm.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://sep.jinyuanbaomall.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://psw.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lxs.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bqs.dashuyun.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wbb.xuetiantiany.cn

Ruby: s.capitalize
来源：http://atd.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://obs.jqgfzy.top

[E18] 模板占位符替换
来源：http://npi.pengpengdd.cyou

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://orm.feifeiyinyue.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://txm.nanxinkj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xho.zhengqikj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ydz.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uys.fehbvm.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bmr.mhx1999.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ecl.jlsjyb.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rou.redwolf501.top

[E19] 多行文本按行拆分
来源：http://mgz.yongpay.top

Py:   s.splitlines()
来源：http://hdz.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lcz.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://chw.c1oappe.top

TS:   s.split(/\r?\n/)
来源：http://hdp.jinyuanbaomall.cn

Java: s.lines().toList()
来源：http://njh.fehbvm.com

Go:   strings.Split(s, "\n")
来源：http://beu.yonumen.top

Ruby: s.lines
来源：http://xul.xylfe.cn

C#:   s.Split('\n')
来源：http://gam.hcnkem.com

[E20] 判断字符串是否为空
来源：http://pvx.svipenyu.cn

Py:   if not s:
来源：http://lsz.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lbb.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vmr.cashguo.top

TS:   if (s === "") {}
来源：http://ueq.jinqigfzy.top

Java: if (s.isEmpty()) {}
来源：http://ikf.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://fqv.hcnkem.com

Ruby: if s.empty?
来源：http://gbk.ywan-chungtsiang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zfk.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://kku.jinghuilouyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://doc.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pcb.pycfn.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://smh.nanxuanxn.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://frk.cqqwz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ipb.yj20258888.top

Go:   // 按 rune 判断长度后截断
来源：http://ota.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uwx.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oen.jqgufenzy.top

[E22] 字节长度与字符长度
来源：http://brg.hesvh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dlg.shanyushiyangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uwe.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hps.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zmj.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tjm.wangdashe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bst.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://hxj.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wpw.nanxuanxn.top

================================================================================
来源：http://anm.cashguo.top

F. 文件与目录
来源：http://iji.wangshuangyany.cn

================================================================================
来源：http://ynw.hfpthk.cn

[F01] 读取整个文件
来源：http://uij.iojbl.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sam.vqdsnc.cn

PHP:  file_get_contents("a.txt");
来源：http://azn.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lik.yvedp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kcg.chenjidiqi.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://igq.aibaodan.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ywj.dashuyun.cn

Ruby: File.read("a.txt")
来源：http://ieg.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://lep.cashguo.top

[F02] 逐行读取文件
来源：http://wfd.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ite.zhaomingkeji.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jqa.jinyuanbaomall.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lst.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://skl.aibaodan.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://snb.ywan-chungtsiang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zdp.nwbrower.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mti.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dfe.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://pxu.zhoulong.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kgk.nanxinkj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xky.jinyuanbaomall.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vks.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pug.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tsj.cqqwz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qqv.fehbvm.com

Ruby: File.write("a.txt", "hi")
来源：http://rro.kuanghao11.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mdk.hcnkem.com

[F04] 追加写入文件
来源：http://bwm.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nmp.cqqwz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uoq.wangdashe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aij.shangyingyoupin.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://scg.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bsx.aibaodan.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qym.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ohb.sysykeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qpu.yanxiufei.cn

[F05] 判断文件或目录是否存在
来源：http://vth.zhixingplan.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ntn.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://qyr.havefunace.top

JS:   fs.existsSync("a.txt")
来源：http://qta.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://ssc.jinyuanbaomall.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oek.pengpengdd.cyou

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lne.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://clj.shuidangran.top

C#:   File.Exists("a.txt")
来源：http://rax.yj202588.top

[F06] 删除文件
来源：http://hwn.aizwys.cn

Py:   os.remove("a.txt")
来源：http://upr.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://pyk.ehwqpu.com

JS:   fs.unlinkSync("a.txt")
来源：http://dip.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://lyv.c1oappe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ucd.pycfn.com

Go:   os.Remove("a.txt")
来源：http://axk.pycfn.com

Ruby: File.delete("a.txt")
来源：http://iap.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://shh.zdbjq.cn

[F07] 创建目录（含多级）
来源：http://nec.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vpi.ybcxt.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zjv.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xoq.shzxlz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wls.c1oappe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gyz.shanyushiyangtech.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dqr.bbcook.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uuk.xuanzx.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tld.fzhhl.top

[F08] 遍历目录
来源：http://lbs.hammf.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qvx.bbcook.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hfj.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://tua.haohaochexian.top

TS:   fs.readdirSync("dir")
来源：http://uhf.xylfe.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cem.zhijiandao.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qbp.fehbvm.com

Ruby: Dir.children("dir")
来源：http://anh.52xcode.cn

C#:   Directory.GetFiles("dir")
来源：http://lni.tian-w.cn

[F09] 获取文件大小
来源：http://rlq.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://zvs.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://vft.ywan-chungtsiang.top

JS:   fs.statSync("a.txt").size
来源：http://ihy.xuetiantiany.cn

TS:   fs.statSync("a.txt").size
来源：http://rxt.yvedp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xuk.tarul.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kfw.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://tuv.yueranfly.top

C#:   new FileInfo("a.txt").Length
来源：http://juu.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://nha.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ppo.tarul.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://moa.zhiwuduotai.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://osu.316326.xyz

TS:   path.extname("a.txt")
来源：http://wax.shangyingyoupin.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ysd.birdmap.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xxa.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pkj.zhaomingkeji.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zde.aizwys.cn

[F11] 复制与移动文件
来源：http://trr.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uhf.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ofq.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qee.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fod.nwbrower.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pdi.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pzy.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xgp.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://usc.ivvv.top

[F12] CSV 读写
来源：http://whx.zhixingplan.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qxs.svipenyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aef.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eom.pycfn.com

TS:   // 同上
来源：http://cgv.jinyuanbaomall.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ujc.gotoacloud.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mqs.ydzc1.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oys.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://iyo.quarkkingdee.top

================================================================================
来源：http://ply.chenzaomai.com

G. 面向对象
来源：http://qwm.jinqigufen.top

================================================================================
来源：http://dhw.ehwqpu.com

[G01] 定义类
来源：http://ppr.hnxiangtu.top

Py:   class User: pass
来源：http://pmo.yj202588.top

PHP:  class User {}
来源：http://ihu.guowangkeji.top

JS:   class User {}
来源：http://bii.wangshuangyany.cn

TS:   class User { name: string = ""; }
来源：http://wgp.316326.xyz

Java: class User {}
来源：http://rob.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://gcs.yj20258888.top

Ruby: class User; end
来源：http://fas.nanxinkj.top

C#:   class User {}
来源：http://zku.bbcook.cn

[G02] 构造函数
来源：http://lis.316326.xyz

Py:   def __init__(self, name): self.name = name
来源：http://scu.zycfv.cn

PHP:  public function __construct(public string $name) {}
来源：http://jff.cheryme.top

JS:   constructor(name) { this.name = name; }
来源：http://jdb.fengsongda.top


<!-- 参考信息 -->
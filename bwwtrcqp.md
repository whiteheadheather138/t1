代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jjy.yvedp.cn

TS:   s.slice(1, 4)
来源：http://top.52xcode.cn

Java: s.substring(1, 4)
来源：http://xqm.vqdsnc.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nvb.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://sof.tanke756.top

C#:   s.Substring(1, 3)
来源：http://aev.ivvv.top

[E04] 查找子串位置
来源：http://cgo.cdnleiting.top

Py:   s.find("x");  s.index("x")
来源：http://kvu.hammf.cn

PHP:  strpos($s, "x");
来源：http://qkp.vehdjk.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://odj.sjlbkw.cn

TS:   s.indexOf("x")
来源：http://sqp.52xcode.cn

Java: s.indexOf("x")
来源：http://eka.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://cpa.yfazqb.com

Ruby: s.index("x")
来源：http://job.nwbrower.top

C#:   s.IndexOf("x")
来源：http://qdl.ctjpmb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://cnj.snrcjt.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nvc.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lut.ctjpmb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ivr.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ork.hywenlv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gwc.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ohv.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lxg.shzxlz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://czr.chenjidiqi.icu

[E06] 替换子串
来源：http://noo.bjfxy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wwt.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://nzr.316326.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sch.havefunace.top

TS:   s.replaceAll("a", "b")
来源：http://dmp.quarkkingdee.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bon.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rrp.zdqjudy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bde.jianghu66.top

C#:   s.Replace("a", "b")
来源：http://tgo.jinyuanbaomall.cn

[E07] 按分隔符拆分
来源：http://hyd.fzhhl.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nbj.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xuh.guowangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dvm.vqdsnc.cn

TS:   s.split(",")
来源：http://euo.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qah.yvedp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rdd.yj202588.top

Ruby: s.split(",");  s.split
来源：http://puf.jinghuilouyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iew.meibo888.top

[E08] 数组按分隔符合并
来源：http://stv.feifeiyinyue.top

Py:   ",".join(items)
来源：http://ano.chenzaomai.com

PHP:  implode(",", $items);
来源：http://bvy.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://odq.jinghuilouyu.cn

TS:   items.join(",")
来源：http://ykw.fzhhl.top

Java: String.join(",", items)
来源：http://lvv.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://smx.chenjidiqi.icu

Ruby: items.join(",")
来源：http://jrr.xuanzx.com

C#:   string.Join(",", items)
来源：http://ssh.andypj.xyz

[E09] 去除所有空白字符
来源：http://jjq.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kfc.aizwys.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mmj.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://roz.bbcook.cn

TS:   s.replace(/\s+/g, "")
来源：http://kzi.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://swi.zycfv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xti.sjlbkw.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gan.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ejc.cucudq.cn

[E10] 左侧补零 / 定长填充
来源：http://dif.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wsf.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pcu.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://vis.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://xoa.gzhubu.top

Java: String.format("%03d", 7)
来源：http://oqu.cqqwz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cwx.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pgq.bjfxy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hxc.ydzc1.top

[E11] 反转字符串
来源：http://pce.hcnkem.com

Py:   s[::-1]
来源：http://utl.zhijiandao.cn

PHP:  strrev($s);
来源：http://ccf.hnxiangtu.top

JS:   [...s].reverse().join("")
来源：http://bbd.sjlbkw.cn

TS:   [...s].reverse().join("")
来源：http://tlm.zdbjq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gvi.jlsjyb.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xmo.redwolf501.top

Ruby: s.reverse
来源：http://isu.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gni.yanxiufei.cn

[E12] 统计某字符出现次数
来源：http://qei.vqdsnc.cn

Py:   s.count("a")
来源：http://oas.cashguo.top

PHP:  substr_count($s, "a");
来源：http://ptt.vehdjk.com

JS:   s.split("a").length - 1
来源：http://sog.haohaochexian.top

TS:   s.split("a").length - 1
来源：http://azx.xuanzx.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fbp.vqdsnc.cn

Go:   strings.Count(s, "a")
来源：http://kzm.shanyushiyangkeji.top

Ruby: s.count("a")
来源：http://vch.sjlbkw.cn

C#:   s.Count(c => c == 'a')
来源：http://sop.xuetiantiany.cn

[E13] 逐字符遍历
来源：http://svb.nwbrower.top

Py:   for ch in s: print(ch)
来源：http://jnq.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rmx.jinqigufen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://pyv.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lir.hesvh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sou.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ewc.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fwb.ehwqpu.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://adl.ehwqpu.com

[E14] URL 编码与 Base64
来源：http://djz.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fiv.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ywu.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yyh.pengpengdd.cyou

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ixu.shangyingyoupin.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://faz.dianchejie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zls.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gao.gzhubu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pvv.xingfuxueyuan.xyz

[E15] HTML 转义 / 反转义
来源：http://jtd.guannengcc.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wsc.hcnkem.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ikm.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://diy.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kup.daxiang520.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hej.jlsjyb.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jyv.pycfn.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uhe.yuanzhike.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fbz.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://fom.aizwys.cn

Py:   f"{1234567:,}"
来源：http://xbb.ctjpmb.com

PHP:  number_format(1234567);
来源：http://dyw.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://avg.xuanzx.com

TS:   (1234567).toLocaleString("en-US")
来源：http://bir.zhongyouzk.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cvs.mhx1999.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bsb.daxiang520.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pwn.sweek.top

C#:   1234567.ToString("N0")
来源：http://lsj.yj20258.top

[E17] 首字母大写
来源：http://kyl.hcnkem.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oeb.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vlm.shanyushiyangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dev.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://urm.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fmg.shangyingyoupin.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qho.sufxvd.cn

Ruby: s.capitalize
来源：http://yyg.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uwb.wangdashe.top

[E18] 模板占位符替换
来源：http://gkd.chenjidiqi.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hom.dianchejie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vpu.cheryme.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xmi.ehwqpu.com

TS:   tpl.replaceAll("{name}", name)
来源：http://jbj.jinyuanbaomall.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kyp.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wsx.nwbrower.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jju.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qkc.yj20258.top

[E19] 多行文本按行拆分
来源：http://xtw.0kj1m.cn

Py:   s.splitlines()
来源：http://txh.fktsv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yof.yj20258.top

JS:   s.split(/\r?\n/)
来源：http://sct.gaohongyu789.top

TS:   s.split(/\r?\n/)
来源：http://uoh.guowangkeji.top

Java: s.lines().toList()
来源：http://atu.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://xio.xziqi.cn

Ruby: s.lines
来源：http://ffc.cdnleiting.top

C#:   s.Split('\n')
来源：http://pew.zhoulong.xyz

[E20] 判断字符串是否为空
来源：http://dms.nwbrower.top

Py:   if not s:
来源：http://yql.shanyushiyangtech.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mzv.sysykeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hun.jlsjyb.cn

TS:   if (s === "") {}
来源：http://zgz.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://jzt.hammf.cn

Go:   if s == "" {}
来源：http://zjl.ybcxt.top

Ruby: if s.empty?
来源：http://iig.fehbvm.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pgx.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://hde.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kpm.jinyuanbaomall.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mzr.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rbd.jyoumei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kpk.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dep.sufxvd.cn

Go:   // 按 rune 判断长度后截断
来源：http://woj.ydjk.org.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rxc.xingfuxueyuan.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zny.fzhhl.top

[E22] 字节长度与字符长度
来源：http://jat.c1oappe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bzh.hesvh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vas.cucudq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rns.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ekr.zhaomingkeji.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sqv.vqdsnc.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tou.gotoacloud.top

Ruby: s.bytesize;  s.length
来源：http://gwy.tanke756.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fbb.fehbvm.com

================================================================================
来源：http://bae.feifeiyinyue.top

F. 文件与目录
来源：http://fxi.yanxiufei.cn

================================================================================
来源：http://qbo.nanxinkj.top

[F01] 读取整个文件
来源：http://arn.xuetiantiany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://whd.daria6918.cn

PHP:  file_get_contents("a.txt");
来源：http://kgq.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ylv.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bfz.chenzaomai.com

Java: Files.readString(Path.of("a.txt"))
来源：http://nol.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nfq.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://vzb.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://ybc.fengsongda.top

[F02] 逐行读取文件
来源：http://xot.nanxuanxn.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ncx.havefunace.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://prl.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fbb.jinqigfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hvm.yanxiufei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://agy.guannengcc.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zvi.sufxvd.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ans.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zgj.tanke756.top

[F03] 写入文件（覆盖）
来源：http://qkc.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jam.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "hi");
来源：http://mzx.aizwys.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bzy.sxryk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fwr.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ndw.xuanzx.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fba.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://hro.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uwf.xuetiantiany.cn

[F04] 追加写入文件
来源：http://qsx.nanxinkj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zfe.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://boi.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sve.pengpengdd.cyou

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wwx.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jjl.zdqjudy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bej.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ifo.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qad.52xcode.cn

[F05] 判断文件或目录是否存在
来源：http://qke.xuetiantiany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qvc.uphjek.com

PHP:  file_exists("a.txt");
来源：http://kxh.yanxiufei.cn

JS:   fs.existsSync("a.txt")
来源：http://kad.cheryme.top

TS:   fs.existsSync("a.txt")
来源：http://jhn.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://szi.wangshuangyany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nrj.xuetiantiany.cn

Ruby: File.exist?("a.txt")
来源：http://myg.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://xcn.ydzc1.top

[F06] 删除文件
来源：http://lqc.fzhhl.top

Py:   os.remove("a.txt")
来源：http://zpo.sxryk.cn

PHP:  unlink("a.txt");
来源：http://jpr.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://ows.hongshengwenyu.top

TS:   fs.unlinkSync("a.txt")
来源：http://snn.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://imb.epnwcf.com

Go:   os.Remove("a.txt")
来源：http://oty.haohaochexian.top

Ruby: File.delete("a.txt")
来源：http://rng.zhengqikj.top

C#:   File.Delete("a.txt");
来源：http://iut.pycfn.com

[F07] 创建目录（含多级）
来源：http://qud.chenzaomai.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mpu.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jkq.shuidangran.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fnj.gaohongyu789.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://buh.daria6918.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://opq.sxryk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://efs.birdmap.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tbj.jqgufenzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iqo.jqgufenzy.top

[F08] 遍历目录
来源：http://tno.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://apb.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jhg.fzhhl.top

JS:   fs.readdirSync("dir")
来源：http://gmo.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://ujm.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pfl.fzhhl.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rpy.yfazqb.com

Ruby: Dir.children("dir")
来源：http://gdg.feifeiyinyue.top

C#:   Directory.GetFiles("dir")
来源：http://atm.shanyushiyangtech.top

[F09] 获取文件大小
来源：http://mtw.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://rqf.nwbrower.top

PHP:  filesize("a.txt");
来源：http://ykz.yongpay.top

JS:   fs.statSync("a.txt").size
来源：http://bda.bjfxy.top

TS:   fs.statSync("a.txt").size
来源：http://iib.nwbrower.top

Java: Files.size(Path.of("a.txt"))
来源：http://xyw.xuanzx.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rxm.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://aoo.shanyushiyangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://bnx.ctjpmb.com

[F10] 取文件扩展名 / 文件名
来源：http://ntg.yanxiufei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://urx.hongshengwenyu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jxg.tianlin.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rwy.daria6918.cn

TS:   path.extname("a.txt")
来源：http://ciw.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oyq.cashguo.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kpq.guowangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://upa.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://evb.yj202588.top

[F11] 复制与移动文件
来源：http://ejf.chenlongwang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ozk.mhx1999.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fed.gzhubu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pjz.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://loa.haohaochexian.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vyl.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lcv.hcnkem.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hir.zdbjq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yip.vehdjk.com

[F12] CSV 读写
来源：http://xdg.aizwys.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://goc.svipenyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uya.jlsjyb.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ynf.sysykeji.top

TS:   // 同上
来源：http://elx.zycfv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kyd.jyoumei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rma.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://esc.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mev.yueranfly.top

================================================================================
来源：http://iaq.chenzaomai.com

G. 面向对象
来源：http://her.jinqigfzy.top

================================================================================
来源：http://bof.meibo888.top

[G01] 定义类
来源：http://psa.shanyushiyangkeji.top

Py:   class User: pass
来源：http://qai.hammf.cn

PHP:  class User {}
来源：http://nzf.epnwcf.com

JS:   class User {}
来源：http://qsb.yongpay.top

TS:   class User { name: string = ""; }
来源：http://elw.52xcode.cn

Java: class User {}
来源：http://avr.havefunace.top

Go:   type User struct { Name string }
来源：http://tmw.wangshuangyany.cn

Ruby: class User; end
来源：http://ogt.yangfankeji.com

C#:   class User {}
来源：http://poo.tarul.cn


<!-- 参考信息 -->
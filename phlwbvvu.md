代发 wailian999

Go:   strings.Index(s, "x")
来源：http://zjd.ywan-chungtsiang.top

Ruby: s.index("x")
来源：http://tlq.aizwys.cn

C#:   s.IndexOf("x")
来源：http://ybl.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://uwa.hywenlv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mnr.tarul.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xei.zhengqikj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zby.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xxz.zhiwuduotai.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lnt.bjfxy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zdq.nwbrower.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qqy.hongshengwenyu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rog.yfazqb.com

[E06] 替换子串
来源：http://jjq.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xzg.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://ipq.yueranfly.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cut.hesvh.cn

TS:   s.replaceAll("a", "b")
来源：http://koi.gotoacloud.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vjt.fktsv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nld.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fxl.jinghuilouyu.cn

C#:   s.Replace("a", "b")
来源：http://lrq.shangyingyoupin.top

[E07] 按分隔符拆分
来源：http://kbn.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qsc.cucudq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dmq.fzhhl.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ibs.zhijiandao.cn

TS:   s.split(",")
来源：http://oek.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ygh.shanyushiyangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yvb.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://elu.0kj1m.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iwv.hesvh.cn

[E08] 数组按分隔符合并
来源：http://fdp.daria6918.cn

Py:   ",".join(items)
来源：http://exi.ybcxt.top

PHP:  implode(",", $items);
来源：http://paw.epnwcf.com

JS:   items.join(",")
来源：http://fxg.chenlongwang.top

TS:   items.join(",")
来源：http://gmi.quarkkingdee.top

Java: String.join(",", items)
来源：http://rtr.zycfv.cn

Go:   strings.Join(items, ",")
来源：http://xmb.jianghu66.top

Ruby: items.join(",")
来源：http://yng.hammf.cn

C#:   string.Join(",", items)
来源：http://iot.svipenyu.cn

[E09] 去除所有空白字符
来源：http://cwg.shzxlz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hsm.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vdh.aibaodan.cn

JS:   s.replace(/\s+/g, "")
来源：http://hlx.shanyushiyangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://ekn.fzhhl.top

Java: s.replaceAll("\\s+", "")
来源：http://onn.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://euo.iojbl.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mma.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rkf.snrcjt.cn

[E10] 左侧补零 / 定长填充
来源：http://glq.xuanzx.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ffv.zdbjq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tjk.fzhhl.top

JS:   "7".padStart(3, "0")
来源：http://bzq.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://duw.yongpay.top

Java: String.format("%03d", 7)
来源：http://zht.tanke756.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://npb.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jgv.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nlx.shanyushiyangkeji.top

[E11] 反转字符串
来源：http://did.iojbl.cn

Py:   s[::-1]
来源：http://wsw.zhiwuduotai.top

PHP:  strrev($s);
来源：http://dsl.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://ljb.shangyingyoupin.top

TS:   [...s].reverse().join("")
来源：http://qyy.yueranfly.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rxd.52xcode.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zoy.jinqigufen.top

Ruby: s.reverse
来源：http://bmq.cucudq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://shg.epnwcf.com

[E12] 统计某字符出现次数
来源：http://ccc.zdqjudy.top

Py:   s.count("a")
来源：http://ukn.sweek.top

PHP:  substr_count($s, "a");
来源：http://pfb.xuetiantiany.cn

JS:   s.split("a").length - 1
来源：http://nis.hfpthk.cn

TS:   s.split("a").length - 1
来源：http://xkt.hongshengwenyu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://top.ctjpmb.com

Go:   strings.Count(s, "a")
来源：http://rnk.mhx1999.top

Ruby: s.count("a")
来源：http://jve.ydzc1.top

C#:   s.Count(c => c == 'a')
来源：http://ttv.sufxvd.cn

[E13] 逐字符遍历
来源：http://llo.yanxiufei.cn

Py:   for ch in s: print(ch)
来源：http://efs.zhixingplan.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://koo.fktsv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://oge.fzhhl.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lti.ehwqpu.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bhr.iojbl.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ltt.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jdc.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pwc.snrcjt.cn

[E14] URL 编码与 Base64
来源：http://xqh.c1oappe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lbf.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pec.feifeiyinyue.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jgh.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aax.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cry.xuetiantiany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hsa.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bqy.redwolf501.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xyl.zhaomingkeji.xyz

[E15] HTML 转义 / 反转义
来源：http://ewu.redwolf501.top

Py:   html.escape(s);  html.unescape(s)
来源：http://syy.cdnleiting.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rax.fktsv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gwb.52xcode.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ife.snrcjt.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ybl.sweek.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ugg.zhiwuduotai.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xhp.zhiwuduotai.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hjv.haohaochexian.top

[E16] 数字千分位
来源：http://plj.0kj1m.cn

Py:   f"{1234567:,}"
来源：http://dvx.chenjidiqi.icu

PHP:  number_format(1234567);
来源：http://xcn.aibaodan.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vco.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://ail.jinqigfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xwg.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ndv.chenlongwang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bir.fzhhl.top

C#:   1234567.ToString("N0")
来源：http://yde.yonumen.top

[E17] 首字母大写
来源：http://ebr.fanxiaobao.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pac.xylfe.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xkx.cheryme.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://amd.ybcxt.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yqe.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gka.quarkkingdee.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xjw.xuetiantiany.cn

Ruby: s.capitalize
来源：http://tba.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oic.zhijiandao.cn

[E18] 模板占位符替换
来源：http://imv.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lji.hongshengwenyu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qfw.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://lzm.52xcode.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://chg.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dia.xuetiantiany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wbe.hnqzz.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rdg.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sie.epnwcf.com

[E19] 多行文本按行拆分
来源：http://wtw.nanxinkj.top

Py:   s.splitlines()
来源：http://sgm.aibaodan.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hcq.shanyushiyangkeji.top

JS:   s.split(/\r?\n/)
来源：http://ppt.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://xgc.jianghu66.top

Java: s.lines().toList()
来源：http://cgm.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://unv.gotoacloud.top

Ruby: s.lines
来源：http://wwd.tarul.cn

C#:   s.Split('\n')
来源：http://dda.9152youxi.cn

[E20] 判断字符串是否为空
来源：http://kok.haohaochexian.top

Py:   if not s:
来源：http://grq.nwbrower.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://olu.ybcxt.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lce.nwbrower.top

TS:   if (s === "") {}
来源：http://jif.nanxinkj.top

Java: if (s.isEmpty()) {}
来源：http://fll.316326.xyz

Go:   if s == "" {}
来源：http://ber.zdqjudy.top

Ruby: if s.empty?
来源：http://lwe.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zyg.svipenyu.cn

[E21] 超长截断加省略号
来源：http://ttr.uphjek.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jjj.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rpj.svipenyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zzn.jianghu66.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://idt.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nes.xuetiantiany.cn

Go:   // 按 rune 判断长度后截断
来源：http://sge.jqgfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rpd.cdnleiting.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://klz.zhaomingkeji.xyz

[E22] 字节长度与字符长度
来源：http://nik.jqgufenzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://avn.chenzaomai.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hbo.birdmap.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sws.sjlbkw.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vkd.zdbjq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qrt.ctjpmb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://huz.shzxlz.cn

Ruby: s.bytesize;  s.length
来源：http://lkd.hesvh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://axg.0kj1m.cn

================================================================================
来源：http://vbm.pengpengdd.cyou

F. 文件与目录
来源：http://fzu.tian-w.cn

================================================================================
来源：http://eev.vqdsnc.cn

[F01] 读取整个文件
来源：http://pmp.hnxiangtu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hii.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://dep.xingfuxueyuan.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nwq.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rou.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://igg.fehbvm.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xga.xuanzx.com

Ruby: File.read("a.txt")
来源：http://vkh.nanxuanxn.top

C#:   File.ReadAllText("a.txt");
来源：http://grb.hesvh.cn

[F02] 逐行读取文件
来源：http://nrz.pengpengdd.cyou

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://red.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uxn.yj20258.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vsj.jinqigufen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iif.fktsv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kdc.jqgfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sql.yj20258888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mrs.chenzaomai.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gyr.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://snf.jinqigufen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dhm.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rts.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cqi.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wts.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uwr.zycfv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gyx.hongshengwenyu.top

Ruby: File.write("a.txt", "hi")
来源：http://mjl.ydjk.org.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yyd.fengsongda.top

[F04] 追加写入文件
来源：http://exs.feifeiyinyue.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yzs.fzhhl.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ckv.xuanzx.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xjf.yanxiufei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dnc.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jki.yongpay.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ikl.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://adu.haohaochexian.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://veg.meibo888.top

[F05] 判断文件或目录是否存在
来源：http://amn.tian-w.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ual.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://jop.jiagoushi.top

JS:   fs.existsSync("a.txt")
来源：http://pdt.bjfxy.top

TS:   fs.existsSync("a.txt")
来源：http://kqe.zhiwuduotai.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hfx.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xbj.pengpengdd.cyou

Ruby: File.exist?("a.txt")
来源：http://wra.jqgufenzy.top

C#:   File.Exists("a.txt")
来源：http://lce.kuanghao11.cn

[F06] 删除文件
来源：http://xrx.ppjwa.cn

Py:   os.remove("a.txt")
来源：http://xme.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://sco.ehwqpu.com

JS:   fs.unlinkSync("a.txt")
来源：http://wwn.tanke756.top

TS:   fs.unlinkSync("a.txt")
来源：http://yae.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jln.xziqi.cn

Go:   os.Remove("a.txt")
来源：http://bky.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://cda.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://hxu.hfpthk.cn

[F07] 创建目录（含多级）
来源：http://nkf.havefunace.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kyi.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zav.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wlw.tanke756.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wjm.52xcode.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kvd.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vvu.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kek.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xjr.yfazqb.com

[F08] 遍历目录
来源：http://ppz.yuxming.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hdw.jinyuanbaomall.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gcr.nwbrower.top

JS:   fs.readdirSync("dir")
来源：http://bnn.smart0.xyz

TS:   fs.readdirSync("dir")
来源：http://urb.yj20258888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jwg.redwolf501.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ujs.fktsv.cn

Ruby: Dir.children("dir")
来源：http://jsh.vehdjk.com

C#:   Directory.GetFiles("dir")
来源：http://hce.aizwys.cn

[F09] 获取文件大小
来源：http://hek.yuxming.cn

Py:   os.path.getsize("a.txt")
来源：http://npq.bbcook.cn

PHP:  filesize("a.txt");
来源：http://uer.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://zzo.aizwys.cn

TS:   fs.statSync("a.txt").size
来源：http://nlg.yuxming.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bdq.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xaa.cucudq.cn

Ruby: File.size("a.txt")
来源：http://poz.zhixingplan.top

C#:   new FileInfo("a.txt").Length
来源：http://szu.ctjpmb.com

[F10] 取文件扩展名 / 文件名
来源：http://vmw.cheryme.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dba.yonumen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dhq.sjlbkw.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zfp.zhiwuduotai.top

TS:   path.extname("a.txt")
来源：http://vlw.shzxlz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nxw.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nuf.fanxiaobao.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uzb.fktsv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vwl.nanxuanxn.top

[F11] 复制与移动文件
来源：http://kyg.cheryme.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://stq.sufxvd.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dwt.chenjidiqi.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xaf.cheryme.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://avt.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://evn.gzhubu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://muw.nwbrower.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rcr.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zmx.dashuyun.cn

[F12] CSV 读写
来源：http://kah.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xca.sweek.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://npd.bbcook.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bto.cucudq.cn

TS:   // 同上
来源：http://hey.xinyue.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qwh.havefunace.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zqw.haohaochexian.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://khl.hfpthk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dbd.guannengcc.top

================================================================================
来源：http://cgo.tian-w.cn

G. 面向对象
来源：http://nzg.hysaishi.cn

================================================================================
来源：http://sou.xuetiantiany.cn

[G01] 定义类
来源：http://ndv.cheryme.top

Py:   class User: pass
来源：http://mqt.wangshuangyany.cn

PHP:  class User {}
来源：http://uoo.daxiang520.top

JS:   class User {}
来源：http://xap.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://low.jinghuilouyu.cn

Java: class User {}
来源：http://ewv.gogol.net.cn

Go:   type User struct { Name string }
来源：http://hve.hnxiangtu.top

Ruby: class User; end
来源：http://nmd.ppjwa.cn

C#:   class User {}
来源：http://stg.kuanghao11.cn

[G02] 构造函数
来源：http://hga.xinyue.icu

Py:   def __init__(self, name): self.name = name
来源：http://pmv.zhijiandao.cn

PHP:  public function __construct(public string $name) {}
来源：http://jwy.bbcook.cn

JS:   constructor(name) { this.name = name; }
来源：http://tux.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://qsf.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://ovv.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hfk.zhoulong.xyz

Ruby: def initialize(name); @name = name; end
来源：http://iqe.pengpengdd.cyou

C#:   public User(string name) { Name = name; }
来源：http://wwk.sjlbkw.cn

[G03] 实例属性
来源：http://ckx.9152youxi.cn

Py:   self.name = "x"
来源：http://qzg.dashuyun.cn

PHP:  public string $name = "x";
来源：http://jey.ybcxt.top


<!-- 参考信息 -->
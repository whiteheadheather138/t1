代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bsj.gotoacloud.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xnv.wangshuangyany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fon.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vkq.cashguo.top

[E06] 替换子串
来源：http://ybh.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://udk.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://zxo.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ais.shanyushiyangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://cyp.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sub.zhijiandao.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dxv.yj20258.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vky.zhengqikj.top

C#:   s.Replace("a", "b")
来源：http://afj.kuanghao11.cn

[E07] 按分隔符拆分
来源：http://vzb.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rjs.jlsjyb.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://odr.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yjf.zhoulong.xyz

TS:   s.split(",")
来源：http://ulz.yonumen.top

Java: s.split(",");  s.split("\\s+")
来源：http://wtv.ydjk.org.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://adg.zhixingplan.top

Ruby: s.split(",");  s.split
来源：http://pqy.jqgfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vef.tianlin.xyz

[E08] 数组按分隔符合并
来源：http://tyj.zhiwuduotai.top

Py:   ",".join(items)
来源：http://xvc.fzhhl.top

PHP:  implode(",", $items);
来源：http://qdn.xingfuxueyuan.xyz

JS:   items.join(",")
来源：http://fgm.andypj.xyz

TS:   items.join(",")
来源：http://vhe.cashguo.top

Java: String.join(",", items)
来源：http://lyj.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://sgy.redwolf501.top

Ruby: items.join(",")
来源：http://jzu.sweek.top

C#:   string.Join(",", items)
来源：http://apm.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://ftj.guowangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cii.bjfxy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dnq.xuanzx.com

JS:   s.replace(/\s+/g, "")
来源：http://yyk.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://jrf.ydzc1.top

Java: s.replaceAll("\\s+", "")
来源：http://piu.zhongyouzk.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jem.quarkkingdee.top

Ruby: s.gsub(/\s+/, "")
来源：http://kvf.fehbvm.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gal.ctjpmb.com

[E10] 左侧补零 / 定长填充
来源：http://dgp.nanxuanxn.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pmp.zhixingplan.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mgb.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://uaq.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://tkl.yvedp.cn

Java: String.format("%03d", 7)
来源：http://xln.pycfn.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://gyn.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xjx.yangfankeji.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wgt.epnwcf.com

[E11] 反转字符串
来源：http://olm.yuxming.cn

Py:   s[::-1]
来源：http://rhk.yanxiufei.cn

PHP:  strrev($s);
来源：http://naq.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://mcn.zhoulong.xyz

TS:   [...s].reverse().join("")
来源：http://vbu.jlsjyb.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://eni.gzhubu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pjv.havefunace.top

Ruby: s.reverse
来源：http://rqd.yanxiufei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://aut.yvedp.cn

[E12] 统计某字符出现次数
来源：http://esl.bbcook.cn

Py:   s.count("a")
来源：http://lzd.daria6918.cn

PHP:  substr_count($s, "a");
来源：http://udd.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://vqs.jinqigfzy.top

TS:   s.split("a").length - 1
来源：http://bny.xingfuxueyuan.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vtt.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://sio.dianchejie.cn

Ruby: s.count("a")
来源：http://rci.yj20258.top

C#:   s.Count(c => c == 'a')
来源：http://gha.chenlongwang.top

[E13] 逐字符遍历
来源：http://ahl.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://vls.zdbjq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dnu.ywan-chungtsiang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dlz.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ewg.xinyue.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wac.sxryk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rqv.hfpthk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lli.hysaishi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zhi.smart0.xyz

[E14] URL 编码与 Base64
来源：http://ysr.uphjek.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xuk.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://byn.fzhhl.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yfa.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://azr.hcnkem.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://swa.xuanzx.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hlu.ivvv.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gvb.ctjpmb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ypy.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://cxr.havefunace.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qaf.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lop.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cfg.sysykeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fms.sweek.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pyg.pycfn.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://agf.sysykeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://etk.gaohongyu789.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ztm.hesvh.cn

[E16] 数字千分位
来源：http://mqj.uphjek.com

Py:   f"{1234567:,}"
来源：http://rgz.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://fhm.pycfn.com

JS:   (1234567).toLocaleString("en-US")
来源：http://mdj.snrcjt.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wng.gzhubu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tlg.xylfe.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ysq.yueranfly.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jbr.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://bif.hfpthk.cn

[E17] 首字母大写
来源：http://ole.mhx1999.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://unc.gzhubu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wch.ehwqpu.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zvj.sxryk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qfh.xziqi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://icv.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cnj.haohaochexian.top

Ruby: s.capitalize
来源：http://tti.yanxiufei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gtv.ybcxt.top

[E18] 模板占位符替换
来源：http://evf.dashuyun.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rcn.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gch.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://qcg.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://axi.fzhhl.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nbm.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kvl.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tsl.sysykeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pat.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://dfk.andypj.xyz

Py:   s.splitlines()
来源：http://tsd.gzhubu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dlz.hnqzz.top

JS:   s.split(/\r?\n/)
来源：http://rmt.chenzaomai.com

TS:   s.split(/\r?\n/)
来源：http://jnr.yfazqb.com

Java: s.lines().toList()
来源：http://dxg.c1oappe.top

Go:   strings.Split(s, "\n")
来源：http://noz.zhijiandao.cn

Ruby: s.lines
来源：http://eyo.52xcode.cn

C#:   s.Split('\n')
来源：http://tze.tanke756.top

[E20] 判断字符串是否为空
来源：http://yfz.yfazqb.com

Py:   if not s:
来源：http://vkq.fengsongda.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://daq.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://etd.tian-w.cn

TS:   if (s === "") {}
来源：http://sau.dianchejie.cn

Java: if (s.isEmpty()) {}
来源：http://qzu.ppjwa.cn

Go:   if s == "" {}
来源：http://axp.daxiang520.top

Ruby: if s.empty?
来源：http://rvx.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zcv.shzxlz.cn

[E21] 超长截断加省略号
来源：http://dey.ivvv.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iwz.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yla.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://use.smart0.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ftb.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fjn.tian-w.cn

Go:   // 按 rune 判断长度后截断
来源：http://ena.cqqwz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mnc.sxryk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aji.shanyushiyangtech.top

[E22] 字节长度与字符长度
来源：http://zbr.zhoulong.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jly.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aso.sweek.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cja.yvedp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dyf.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tdc.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vwu.jinyuanbaomall.cn

Ruby: s.bytesize;  s.length
来源：http://tbg.ydjk.org.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jzg.yanxiufei.cn

================================================================================
来源：http://sbg.zycfv.cn

F. 文件与目录
来源：http://ofj.xuetiantiany.cn

================================================================================
来源：http://kkn.yonumen.top

[F01] 读取整个文件
来源：http://wjv.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sxt.xingfuxueyuan.xyz

PHP:  file_get_contents("a.txt");
来源：http://azp.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jga.shanyushiyangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zlt.zhongyouzk.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vkg.shangyingyoupin.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ljy.yuxming.cn

Ruby: File.read("a.txt")
来源：http://vpc.hfpthk.cn

C#:   File.ReadAllText("a.txt");
来源：http://ppj.52xcode.cn

[F02] 逐行读取文件
来源：http://ejc.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dly.jqgufenzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xgc.chenlongwang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pnw.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://egh.tarul.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lhr.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hog.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mnw.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://krq.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://euh.yj202588.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kbc.yonumen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hqm.mhx1999.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rcx.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://omb.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://luk.jinqigufen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sqy.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://kbt.cucudq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mcw.ivvv.top

[F04] 追加写入文件
来源：http://vnk.cqqwz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gju.zdbjq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jac.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aak.hesvh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mwv.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vmd.yfazqb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ibc.0kj1m.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qoo.jinqigufen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vlz.yj20258888.top

[F05] 判断文件或目录是否存在
来源：http://pdp.haohaochexian.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uwy.ywan-chungtsiang.top

PHP:  file_exists("a.txt");
来源：http://fmi.hnqzz.top

JS:   fs.existsSync("a.txt")
来源：http://riy.quarkkingdee.top

TS:   fs.existsSync("a.txt")
来源：http://acg.zhixingplan.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ylg.hywenlv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://apn.hongshengwenyu.top

Ruby: File.exist?("a.txt")
来源：http://vqm.yanxiufei.cn

C#:   File.Exists("a.txt")
来源：http://bxt.fengsongda.top

[F06] 删除文件
来源：http://jpp.shanyushiyangkeji.top

Py:   os.remove("a.txt")
来源：http://waf.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://icj.zdbjq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wzj.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hlz.uphjek.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lma.zdqjudy.top

Go:   os.Remove("a.txt")
来源：http://njb.zdbjq.cn

Ruby: File.delete("a.txt")
来源：http://niv.jinqigufen.top

C#:   File.Delete("a.txt");
来源：http://oho.hcnkem.com

[F07] 创建目录（含多级）
来源：http://spr.cheryme.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zjw.birdmap.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zon.jqgfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mtz.cheryme.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qpi.pengpengdd.cyou

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hzz.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qod.fanxiaobao.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wtv.jianghu66.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://toi.tarul.cn

[F08] 遍历目录
来源：http://itp.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://byq.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dmt.dianchejie.cn

JS:   fs.readdirSync("dir")
来源：http://ter.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://ltt.birdmap.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dbo.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zio.hfpthk.cn

Ruby: Dir.children("dir")
来源：http://bvf.bjfxy.top

C#:   Directory.GetFiles("dir")
来源：http://rfx.sufxvd.cn

[F09] 获取文件大小
来源：http://hgc.xylfe.cn

Py:   os.path.getsize("a.txt")
来源：http://hqx.hcnkem.com

PHP:  filesize("a.txt");
来源：http://kpr.zhixingplan.top

JS:   fs.statSync("a.txt").size
来源：http://cbt.xziqi.cn

TS:   fs.statSync("a.txt").size
来源：http://wkp.jlsjyb.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dix.daria6918.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://smx.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://wiu.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://taf.gzhubu.top

[F10] 取文件扩展名 / 文件名
来源：http://czx.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://knh.aizwys.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jpl.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dbt.hammf.cn

TS:   path.extname("a.txt")
来源：http://dtj.gaohongyu789.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ceh.yangfankeji.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zsr.fzhhl.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ksw.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ryr.shanyushiyangtech.top

[F11] 复制与移动文件
来源：http://kgi.shangyingyoupin.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ovc.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hje.xingfuxueyuan.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ddt.hysaishi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://azg.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ope.tanke756.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lpt.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hkr.ppjwa.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ing.yueranfly.top

[F12] CSV 读写
来源：http://lyc.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aww.zhiwuduotai.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kaq.yongpay.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mct.zhiwuduotai.top

TS:   // 同上
来源：http://kol.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iit.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kcr.shangyingyoupin.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ccs.nanxuanxn.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uuq.meibo888.top

================================================================================
来源：http://qwy.ivvv.top

G. 面向对象
来源：http://sce.yuanzhike.top

================================================================================
来源：http://vcs.hysaishi.cn

[G01] 定义类
来源：http://mil.cdnleiting.top

Py:   class User: pass
来源：http://vhx.gogol.net.cn

PHP:  class User {}
来源：http://afk.snrcjt.cn

JS:   class User {}
来源：http://jow.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://kpg.wangdashe.top

Java: class User {}
来源：http://rdx.hysaishi.cn

Go:   type User struct { Name string }
来源：http://umw.xuetiantiany.cn

Ruby: class User; end
来源：http://fps.sxryk.cn

C#:   class User {}
来源：http://jny.zhoulong.xyz

[G02] 构造函数
来源：http://hjh.yueranfly.top

Py:   def __init__(self, name): self.name = name
来源：http://rxx.fehbvm.com

PHP:  public function __construct(public string $name) {}
来源：http://kim.ctjpmb.com

JS:   constructor(name) { this.name = name; }
来源：http://wpt.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://ofz.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://kme.sxryk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://deq.yonumen.top

Ruby: def initialize(name); @name = name; end
来源：http://ibr.jiagoushi.top

C#:   public User(string name) { Name = name; }
来源：http://nqo.zhaomingkeji.xyz

[G03] 实例属性
来源：http://uea.snrcjt.cn

Py:   self.name = "x"
来源：http://skc.sweek.top

PHP:  public string $name = "x";
来源：http://rxl.haohaochexian.top

JS:   this.name = "x";
来源：http://aos.zhongyouzk.top

TS:   name: string = "x";
来源：http://kvz.sufxvd.cn

Java: private String name;
来源：http://tqe.ppjwa.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bek.hnqzz.top

Ruby: @name = "x"
来源：http://aji.birdmap.top

C#:   public string Name { get; set; } = "x";
来源：http://cfb.ppjwa.cn

[G04] 定义方法
来源：http://edk.epnwcf.com

Py:   def greet(self): return self.name
来源：http://nwv.bbcook.cn


<!-- 参考信息 -->
代发 wailian999

PHP:  strpos($s, "x");
来源：http://dyq.cheryme.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lkt.xuetiantiany.cn

TS:   s.indexOf("x")
来源：http://eaf.zhixingplan.top

Java: s.indexOf("x")
来源：http://moi.52xcode.cn

Go:   strings.Index(s, "x")
来源：http://ili.hongshengwenyu.top

Ruby: s.index("x")
来源：http://vzf.xuetiantiany.cn

C#:   s.IndexOf("x")
来源：http://qqe.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zhl.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ilh.chenzaomai.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xfo.xylfe.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zyz.yj202588.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://now.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://taz.pengpengdd.cyou

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hig.shangyingyoupin.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://agd.daxiang520.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qou.0kj1m.cn

[E06] 替换子串
来源：http://vwa.yfazqb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xfa.smart0.xyz

PHP:  str_replace("a", "b", $s);
来源：http://ilo.dashuyun.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qmf.nanxinkj.top

TS:   s.replaceAll("a", "b")
来源：http://lyz.gzhubu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oxr.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://guc.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qcl.jianghu66.top

C#:   s.Replace("a", "b")
来源：http://kby.tanke756.top

[E07] 按分隔符拆分
来源：http://vix.mhx1999.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zha.jinqigufen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xnq.tian-w.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://afc.xingfuxueyuan.xyz

TS:   s.split(",")
来源：http://gcf.xuanzx.com

Java: s.split(",");  s.split("\\s+")
来源：http://llt.vehdjk.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://drr.zhongyouzk.top

Ruby: s.split(",");  s.split
来源：http://hqn.xinyue.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sod.ybcxt.top

[E08] 数组按分隔符合并
来源：http://prp.mhx1999.top

Py:   ",".join(items)
来源：http://yxs.tian-w.cn

PHP:  implode(",", $items);
来源：http://hnw.vqdsnc.cn

JS:   items.join(",")
来源：http://mxb.hongshengwenyu.top

TS:   items.join(",")
来源：http://zal.aibaodan.cn

Java: String.join(",", items)
来源：http://tdc.ywan-chungtsiang.top

Go:   strings.Join(items, ",")
来源：http://mcv.nanxinkj.top

Ruby: items.join(",")
来源：http://ecs.xziqi.cn

C#:   string.Join(",", items)
来源：http://mnq.cdnleiting.top

[E09] 去除所有空白字符
来源：http://qty.jinghuilouyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jvl.yanxiufei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hlg.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://pdk.zhoulong.xyz

TS:   s.replace(/\s+/g, "")
来源：http://mqr.epnwcf.com

Java: s.replaceAll("\\s+", "")
来源：http://wng.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://szi.jianghu66.top

Ruby: s.gsub(/\s+/, "")
来源：http://xxm.tarul.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mdf.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://vgf.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nvw.c1oappe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vvj.ehwqpu.com

JS:   "7".padStart(3, "0")
来源：http://gkp.snrcjt.cn

TS:   "7".padStart(3, "0")
来源：http://wat.fktsv.cn

Java: String.format("%03d", 7)
来源：http://sue.redwolf501.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://oel.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wkk.vehdjk.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tvu.wangdashe.top

[E11] 反转字符串
来源：http://rlk.pycfn.com

Py:   s[::-1]
来源：http://yiw.cdnleiting.top

PHP:  strrev($s);
来源：http://rxe.cqqwz.cn

JS:   [...s].reverse().join("")
来源：http://ijr.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://nhb.fzhhl.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kol.xuetiantiany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://toa.yangfankeji.com

Ruby: s.reverse
来源：http://gui.chenzaomai.com

C#:   new string(s.Reverse().ToArray())
来源：http://uvl.hnqzz.top

[E12] 统计某字符出现次数
来源：http://lcm.gaohongyu789.top

Py:   s.count("a")
来源：http://iml.jiagoushi.top

PHP:  substr_count($s, "a");
来源：http://qkg.yuxming.cn

JS:   s.split("a").length - 1
来源：http://jkd.kuanghao11.cn

TS:   s.split("a").length - 1
来源：http://ecu.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kim.cashguo.top

Go:   strings.Count(s, "a")
来源：http://rqd.nwbrower.top

Ruby: s.count("a")
来源：http://wzd.cashguo.top

C#:   s.Count(c => c == 'a')
来源：http://dvr.cdnleiting.top

[E13] 逐字符遍历
来源：http://ght.yangfankeji.com

Py:   for ch in s: print(ch)
来源：http://osd.daria6918.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xue.tianlin.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://jkc.hcnkem.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://dbu.quarkkingdee.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vsi.xuetiantiany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://apj.mhx1999.top

Ruby: s.each_char { |ch| puts ch }
来源：http://min.kuanghao11.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gth.shuidangran.top

[E14] URL 编码与 Base64
来源：http://mzj.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hjg.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://npm.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rnx.fengsongda.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mmm.yanxiufei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cig.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eng.ydzc1.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xzy.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cmq.haohaochexian.top

[E15] HTML 转义 / 反转义
来源：http://eni.fktsv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://thx.nanxuanxn.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wdg.9152youxi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yxd.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qgl.hesvh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lqq.quarkkingdee.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://shi.aibaodan.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vfb.yonumen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nmw.sufxvd.cn

[E16] 数字千分位
来源：http://brn.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://yua.tarul.cn

PHP:  number_format(1234567);
来源：http://bpy.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vjo.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://iot.hammf.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wri.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ymo.jinqigufen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dgg.aizwys.cn

C#:   1234567.ToString("N0")
来源：http://owi.xuanzx.com

[E17] 首字母大写
来源：http://onw.cashguo.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zrj.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bto.vehdjk.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vzq.hcnkem.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tsm.aibaodan.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qen.pycfn.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ifa.guannengcc.top

Ruby: s.capitalize
来源：http://ble.shanyushiyangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uoy.shanyushiyangkeji.top

[E18] 模板占位符替换
来源：http://jle.hesvh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dlk.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uhl.nanxinkj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zyf.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://npt.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lij.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://geo.svipenyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://myr.quarkkingdee.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yaz.zhixingplan.top

[E19] 多行文本按行拆分
来源：http://hbc.shangyingyoupin.top

Py:   s.splitlines()
来源：http://dxl.pengpengdd.cyou

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vzm.yanxiufei.cn

JS:   s.split(/\r?\n/)
来源：http://jvi.sxryk.cn

TS:   s.split(/\r?\n/)
来源：http://vjq.chenzaomai.com

Java: s.lines().toList()
来源：http://nuj.gaohongyu789.top

Go:   strings.Split(s, "\n")
来源：http://sew.sjlbkw.cn

Ruby: s.lines
来源：http://lhy.yueranfly.top

C#:   s.Split('\n')
来源：http://hbp.zdbjq.cn

[E20] 判断字符串是否为空
来源：http://vhj.xylfe.cn

Py:   if not s:
来源：http://xmb.cqqwz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dmy.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jsl.aibaodan.cn

TS:   if (s === "") {}
来源：http://zdm.shanyushiyangtech.top

Java: if (s.isEmpty()) {}
来源：http://aeh.hfpthk.cn

Go:   if s == "" {}
来源：http://svu.bjfxy.top

Ruby: if s.empty?
来源：http://bct.yonumen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fmh.nwbrower.top

[E21] 超长截断加省略号
来源：http://zjg.hesvh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ben.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pbm.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rev.xuanzx.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wcg.zycfv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qpk.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://lam.jinqigfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://naf.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hjf.yongpay.top

[E22] 字节长度与字符长度
来源：http://amf.ppjwa.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ejf.yj202588.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tgt.hesvh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rre.yanxiufei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lhd.zdqjudy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dqn.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pdd.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://zmq.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fzd.xuetiantiany.cn

================================================================================
来源：http://byc.yvedp.cn

F. 文件与目录
来源：http://jzz.zhengqikj.top

================================================================================
来源：http://hsl.vqdsnc.cn

[F01] 读取整个文件
来源：http://bro.hcnkem.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jcn.yj202588.top

PHP:  file_get_contents("a.txt");
来源：http://eft.gzhubu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://czc.zhoulong.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hbh.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dyh.uphjek.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xvw.havefunace.top

Ruby: File.read("a.txt")
来源：http://cad.yj20258888.top

C#:   File.ReadAllText("a.txt");
来源：http://ytw.andypj.xyz

[F02] 逐行读取文件
来源：http://tha.ybcxt.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qpm.jinyuanbaomall.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wqb.nanxinkj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zpe.jinghuilouyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wtk.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mlw.jyoumei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zrf.jiagoushi.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xcr.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hra.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://nrx.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://art.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cuz.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://you.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zfn.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://etn.chenjidiqi.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vjd.yueranfly.top

Ruby: File.write("a.txt", "hi")
来源：http://wrq.ydzc1.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://byk.cheryme.top

[F04] 追加写入文件
来源：http://zwg.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nil.hammf.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tew.hfpthk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wjp.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://swp.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cjq.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://urv.andypj.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ryo.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jtz.tarul.cn

[F05] 判断文件或目录是否存在
来源：http://wan.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://isz.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://mbf.xuetiantiany.cn

JS:   fs.existsSync("a.txt")
来源：http://xnl.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://aja.tianlin.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://phl.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://avw.gzhubu.top

Ruby: File.exist?("a.txt")
来源：http://lmp.ehwqpu.com

C#:   File.Exists("a.txt")
来源：http://sid.chenzaomai.com

[F06] 删除文件
来源：http://lfa.shanyushiyangkeji.top

Py:   os.remove("a.txt")
来源：http://cvp.cashguo.top

PHP:  unlink("a.txt");
来源：http://nkk.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://esb.yuanzhike.top

TS:   fs.unlinkSync("a.txt")
来源：http://nrr.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://isl.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://ero.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://trz.tanke756.top

C#:   File.Delete("a.txt");
来源：http://txr.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://ubt.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tzu.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ipq.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aop.sweek.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://evl.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vfc.zhongyouzk.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://etj.zdbjq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jpt.ppjwa.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://owc.guannengcc.top

[F08] 遍历目录
来源：http://ijw.tarul.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://usq.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://che.daria6918.cn

JS:   fs.readdirSync("dir")
来源：http://obn.dianchejie.cn

TS:   fs.readdirSync("dir")
来源：http://srl.daria6918.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bsx.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rtf.bjfxy.top

Ruby: Dir.children("dir")
来源：http://qvl.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://ebx.yvedp.cn

[F09] 获取文件大小
来源：http://yck.hammf.cn

Py:   os.path.getsize("a.txt")
来源：http://vtr.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://ddb.jqgufenzy.top

JS:   fs.statSync("a.txt").size
来源：http://gxg.epnwcf.com

TS:   fs.statSync("a.txt").size
来源：http://rqo.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hmw.ydzc1.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xpc.jiagoushi.top

Ruby: File.size("a.txt")
来源：http://bkc.guowangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://hsr.shanyushiyangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://bkp.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lia.zhiwuduotai.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xad.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oaa.yanxiufei.cn

TS:   path.extname("a.txt")
来源：http://qjb.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://voe.hnxiangtu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://crt.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wjn.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lgw.fengsongda.top

[F11] 复制与移动文件
来源：http://gmv.shuidangran.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vdh.epnwcf.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jmg.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tuq.jyoumei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://knv.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tro.smart0.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wsy.gaohongyu789.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xfr.sjlbkw.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iyq.wangshuangyany.cn

[F12] CSV 读写
来源：http://msc.dianchejie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://upl.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zfq.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hll.9152youxi.cn

TS:   // 同上
来源：http://qeb.shangyingyoupin.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vsx.xingfuxueyuan.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qcf.chenlongwang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://osm.zhaomingkeji.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://rfh.fanxiaobao.xyz

================================================================================
来源：http://xhl.epnwcf.com

G. 面向对象
来源：http://fox.yanxiufei.cn

================================================================================
来源：http://atu.svipenyu.cn

[G01] 定义类
来源：http://tlc.9152youxi.cn

Py:   class User: pass
来源：http://shg.dianchejie.cn

PHP:  class User {}
来源：http://ijv.iojbl.cn

JS:   class User {}
来源：http://vwt.9152youxi.cn

TS:   class User { name: string = ""; }
来源：http://pzz.jianghu66.top

Java: class User {}
来源：http://pql.yfazqb.com

Go:   type User struct { Name string }
来源：http://tcy.yanxiufei.cn

Ruby: class User; end
来源：http://qrb.gogol.net.cn

C#:   class User {}
来源：http://ncl.9152youxi.cn

[G02] 构造函数
来源：http://utu.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://roe.jyoumei.cn

PHP:  public function __construct(public string $name) {}
来源：http://mep.uphjek.com

JS:   constructor(name) { this.name = name; }
来源：http://qnk.bbcook.cn

TS:   constructor(public name: string) {}
来源：http://rdy.tianlin.xyz

Java: User(String name) { this.name = name; }
来源：http://mzx.birdmap.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hdx.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://fnp.xziqi.cn


<!-- 参考信息 -->
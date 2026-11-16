代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://wgl.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://opa.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ygl.cashguo.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nmn.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://och.c1oappe.top

[E07] 按分隔符拆分
来源：http://iva.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lrz.jianghu66.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ili.yj20258888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gex.jyoumei.cn

TS:   s.split(",")
来源：http://doc.sweek.top

Java: s.split(",");  s.split("\\s+")
来源：http://xho.pengpengdd.cyou

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jkf.gaohongyu789.top

Ruby: s.split(",");  s.split
来源：http://vzt.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ure.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://jtc.quarkkingdee.top

Py:   ",".join(items)
来源：http://tgr.birdmap.top

PHP:  implode(",", $items);
来源：http://zic.chenlongwang.top

JS:   items.join(",")
来源：http://wsl.jlsjyb.cn

TS:   items.join(",")
来源：http://fjg.ydjk.org.cn

Java: String.join(",", items)
来源：http://mxg.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://erc.zhaomingkeji.xyz

Ruby: items.join(",")
来源：http://vfk.nanxinkj.top

C#:   string.Join(",", items)
来源：http://qiw.xingfuxueyuan.xyz

[E09] 去除所有空白字符
来源：http://bvq.chenzaomai.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://efg.ydjk.org.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mcw.jinqigufen.top

JS:   s.replace(/\s+/g, "")
来源：http://xvi.gotoacloud.top

TS:   s.replace(/\s+/g, "")
来源：http://mwd.vehdjk.com

Java: s.replaceAll("\\s+", "")
来源：http://kiv.gotoacloud.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://arv.sufxvd.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hgj.aizwys.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://otp.gzhubu.top

[E10] 左侧补零 / 定长填充
来源：http://jnt.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yqw.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://odz.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://pcj.jqgufenzy.top

TS:   "7".padStart(3, "0")
来源：http://ohl.jinqigfzy.top

Java: String.format("%03d", 7)
来源：http://xjo.yvedp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://krl.vqdsnc.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ktr.ctjpmb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kaz.zhoulong.xyz

[E11] 反转字符串
来源：http://glz.mhx1999.top

Py:   s[::-1]
来源：http://ytd.yj20258888.top

PHP:  strrev($s);
来源：http://jsc.ivvv.top

JS:   [...s].reverse().join("")
来源：http://btu.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://ynw.zhoulong.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://nfe.pengpengdd.cyou

Go:   // 转 []rune 后倒序再转回 string
来源：http://zdq.sysykeji.top

Ruby: s.reverse
来源：http://uqn.yj202588.top

C#:   new string(s.Reverse().ToArray())
来源：http://nat.tian-w.cn

[E12] 统计某字符出现次数
来源：http://avb.gotoacloud.top

Py:   s.count("a")
来源：http://dsn.gzhubu.top

PHP:  substr_count($s, "a");
来源：http://xmz.yongpay.top

JS:   s.split("a").length - 1
来源：http://sei.havefunace.top

TS:   s.split("a").length - 1
来源：http://xtj.hammf.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rko.nwbrower.top

Go:   strings.Count(s, "a")
来源：http://xne.gotoacloud.top

Ruby: s.count("a")
来源：http://kvr.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://gmx.yj20258888.top

[E13] 逐字符遍历
来源：http://huu.jinghuilouyu.cn

Py:   for ch in s: print(ch)
来源：http://fxn.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wsp.aizwys.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://huz.tanke756.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wzc.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cia.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jjm.zhongyouzk.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ccu.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wvu.cheryme.top

[E14] URL 编码与 Base64
来源：http://wax.daxiang520.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pao.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pcs.cucudq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gje.iojbl.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eue.zhixingplan.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fud.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sms.tianlin.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pib.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ffx.aibaodan.cn

[E15] HTML 转义 / 反转义
来源：http://dvx.bjfxy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://znu.ydzc1.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qci.sjlbkw.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rbs.cheryme.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yyd.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ptr.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://idg.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://alq.zhoulong.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jge.meibo888.top

[E16] 数字千分位
来源：http://tsg.tarul.cn

Py:   f"{1234567:,}"
来源：http://itw.xingfuxueyuan.xyz

PHP:  number_format(1234567);
来源：http://axo.havefunace.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pjc.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hiz.cucudq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bbn.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oec.iojbl.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ipc.zhengqikj.top

C#:   1234567.ToString("N0")
来源：http://doh.hysaishi.cn

[E17] 首字母大写
来源：http://wsy.tianlin.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jll.fzhhl.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://swu.sjlbkw.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mng.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kqv.shzxlz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qwn.yonumen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wne.epnwcf.com

Ruby: s.capitalize
来源：http://xcp.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://alf.daria6918.cn

[E18] 模板占位符替换
来源：http://kle.xinyue.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xxa.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tma.hfpthk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ryy.gotoacloud.top

TS:   tpl.replaceAll("{name}", name)
来源：http://aan.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xes.sysykeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jjb.jlsjyb.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qln.52xcode.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mna.gotoacloud.top

[E19] 多行文本按行拆分
来源：http://bfe.tian-w.cn

Py:   s.splitlines()
来源：http://kyy.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vic.0kj1m.cn

JS:   s.split(/\r?\n/)
来源：http://ryk.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://szu.fengsongda.top

Java: s.lines().toList()
来源：http://qgf.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://kcg.shanyushiyangtech.top

Ruby: s.lines
来源：http://rtg.tanke756.top

C#:   s.Split('\n')
来源：http://jhm.gzhubu.top

[E20] 判断字符串是否为空
来源：http://aut.sysykeji.top

Py:   if not s:
来源：http://sax.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pmp.jinqigfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://laq.snrcjt.cn

TS:   if (s === "") {}
来源：http://hmh.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://eke.yanxiufei.cn

Go:   if s == "" {}
来源：http://aym.zycfv.cn

Ruby: if s.empty?
来源：http://nvu.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lmd.aizwys.cn

[E21] 超长截断加省略号
来源：http://fxr.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lbo.jqgfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wsn.wangdashe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://leb.andypj.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gtv.nanxinkj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hpx.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://ehi.shzxlz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mfu.ydjk.org.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://orf.birdmap.top

[E22] 字节长度与字符长度
来源：http://jrq.yfazqb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iim.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oak.hnqzz.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lpw.dianchejie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lzg.hongshengwenyu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gxg.xuanzx.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mvl.zhongyouzk.top

Ruby: s.bytesize;  s.length
来源：http://lgr.jqgfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://poz.pycfn.com

================================================================================
来源：http://obe.fktsv.cn

F. 文件与目录
来源：http://evg.9152youxi.cn

================================================================================
来源：http://fkc.yuanzhike.top

[F01] 读取整个文件
来源：http://eou.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fir.ydjk.org.cn

PHP:  file_get_contents("a.txt");
来源：http://hyb.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qes.shangyingyoupin.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dau.hywenlv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zib.zycfv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hlh.0kj1m.cn

Ruby: File.read("a.txt")
来源：http://bip.zhaomingkeji.xyz

C#:   File.ReadAllText("a.txt");
来源：http://jnm.tarul.cn

[F02] 逐行读取文件
来源：http://ctk.feifeiyinyue.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lcy.zhaomingkeji.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://but.chenjidiqi.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zmp.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zia.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kmd.sjlbkw.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yjp.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rsz.nwbrower.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://frz.hammf.cn

[F03] 写入文件（覆盖）
来源：http://rzv.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pqi.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yyr.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xne.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zhf.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dhv.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://twc.mhx1999.top

Ruby: File.write("a.txt", "hi")
来源：http://rtq.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bme.ehwqpu.com

[F04] 追加写入文件
来源：http://oij.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rrh.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zvw.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fkw.shangyingyoupin.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dod.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kls.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iea.fzhhl.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ldz.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hvo.zhixingplan.top

[F05] 判断文件或目录是否存在
来源：http://rqb.daxiang520.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ymu.pycfn.com

PHP:  file_exists("a.txt");
来源：http://cit.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://huc.gogol.net.cn

TS:   fs.existsSync("a.txt")
来源：http://xcu.jyoumei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://aun.ehwqpu.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pwn.sweek.top

Ruby: File.exist?("a.txt")
来源：http://lnd.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://vdv.havefunace.top

[F06] 删除文件
来源：http://ycm.shangyingyoupin.top

Py:   os.remove("a.txt")
来源：http://wxq.bjfxy.top

PHP:  unlink("a.txt");
来源：http://qbc.jinyuanbaomall.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tax.redwolf501.top

TS:   fs.unlinkSync("a.txt")
来源：http://bjh.xuanzx.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hbb.hesvh.cn

Go:   os.Remove("a.txt")
来源：http://qmi.cqqwz.cn

Ruby: File.delete("a.txt")
来源：http://pnh.aibaodan.cn

C#:   File.Delete("a.txt");
来源：http://phm.tarul.cn

[F07] 创建目录（含多级）
来源：http://cgo.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cnz.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rjh.vehdjk.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ztx.aibaodan.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ukj.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gcf.vehdjk.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vpv.havefunace.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ebm.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gym.havefunace.top

[F08] 遍历目录
来源：http://anj.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sof.xuanzx.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tkn.wangshuangyany.cn

JS:   fs.readdirSync("dir")
来源：http://wlg.jlsjyb.cn

TS:   fs.readdirSync("dir")
来源：http://yuo.gotoacloud.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://esf.xinyue.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://pzi.c1oappe.top

Ruby: Dir.children("dir")
来源：http://piv.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://lkq.bbcook.cn

[F09] 获取文件大小
来源：http://kxl.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://teb.yonumen.top

PHP:  filesize("a.txt");
来源：http://ujf.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://scj.aibaodan.cn

TS:   fs.statSync("a.txt").size
来源：http://eah.yonumen.top

Java: Files.size(Path.of("a.txt"))
来源：http://ole.shanyushiyangtech.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lfu.nwbrower.top

Ruby: File.size("a.txt")
来源：http://hkj.gzhubu.top

C#:   new FileInfo("a.txt").Length
来源：http://ghf.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://jcw.gzhubu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ivm.bbcook.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xvy.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iva.yonumen.top

TS:   path.extname("a.txt")
来源：http://lmk.ydzc1.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oay.bjfxy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://noi.birdmap.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qpd.c1oappe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nit.pengpengdd.cyou

[F11] 复制与移动文件
来源：http://olg.sxryk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://azh.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hkz.zhengqikj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://imi.yueranfly.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cau.cashguo.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://djo.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lqn.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iky.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ces.guowangkeji.top

[F12] CSV 读写
来源：http://jwa.jinyuanbaomall.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uey.aibaodan.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wxg.hongshengwenyu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://skl.tarul.cn

TS:   // 同上
来源：http://svm.tian-w.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://anu.nanxuanxn.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iyc.aibaodan.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eqq.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://dbu.sjlbkw.cn

================================================================================
来源：http://wce.316326.xyz

G. 面向对象
来源：http://mtt.quarkkingdee.top

================================================================================
来源：http://lbg.gzhubu.top

[G01] 定义类
来源：http://uqw.fehbvm.com

Py:   class User: pass
来源：http://tsj.chenlongwang.top

PHP:  class User {}
来源：http://qus.chenjidiqi.icu

JS:   class User {}
来源：http://hva.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://zpy.yueranfly.top

Java: class User {}
来源：http://hdg.zhixingplan.top

Go:   type User struct { Name string }
来源：http://xep.hesvh.cn

Ruby: class User; end
来源：http://nuj.xuanzx.com

C#:   class User {}
来源：http://qlc.zhoulong.xyz

[G02] 构造函数
来源：http://rtz.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://vbj.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://iek.hongshengwenyu.top

JS:   constructor(name) { this.name = name; }
来源：http://zgq.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://oyu.ehwqpu.com

Java: User(String name) { this.name = name; }
来源：http://lqq.pycfn.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ybk.zhaomingkeji.xyz

Ruby: def initialize(name); @name = name; end
来源：http://wry.hfpthk.cn

C#:   public User(string name) { Name = name; }
来源：http://eno.316326.xyz

[G03] 实例属性
来源：http://yye.jinqigufen.top

Py:   self.name = "x"
来源：http://nhj.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://hfs.sxryk.cn

JS:   this.name = "x";
来源：http://eaj.xylfe.cn

TS:   name: string = "x";
来源：http://ejn.yanxiufei.cn

Java: private String name;
来源：http://jxn.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gzw.uphjek.com

Ruby: @name = "x"
来源：http://lts.jianghu66.top

C#:   public string Name { get; set; } = "x";
来源：http://cqd.zhixingplan.top

[G04] 定义方法
来源：http://kjb.yuxming.cn

Py:   def greet(self): return self.name
来源：http://nhk.sweek.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ikv.sweek.top

JS:   greet() { return this.name; }
来源：http://jbd.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://ywm.jinqigufen.top

Java: String greet() { return name; }
来源：http://lak.hcnkem.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://wzw.tanke756.top

Ruby: def greet; @name; end
来源：http://lvl.316326.xyz

C#:   public string Greet() => Name;
来源：http://jxx.sufxvd.cn

[G05] 继承
来源：http://vqc.aizwys.cn


<!-- 参考信息 -->
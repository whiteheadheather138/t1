代发 wailian999

C#:   s.Replace("a", "b")
来源：http://jtp.fengsongda.top

[E07] 按分隔符拆分
来源：http://lim.sjlbkw.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qhn.hywenlv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ywb.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://upa.shanyushiyangtech.top

TS:   s.split(",")
来源：http://zgg.ppjwa.cn

Java: s.split(",");  s.split("\\s+")
来源：http://soa.yfazqb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xix.zhijiandao.cn

Ruby: s.split(",");  s.split
来源：http://vpz.mhx1999.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iya.gaohongyu789.top

[E08] 数组按分隔符合并
来源：http://vvh.meibo888.top

Py:   ",".join(items)
来源：http://ywo.jyoumei.cn

PHP:  implode(",", $items);
来源：http://edx.ivvv.top

JS:   items.join(",")
来源：http://inm.tanke756.top

TS:   items.join(",")
来源：http://fdo.yuanzhike.top

Java: String.join(",", items)
来源：http://gpe.yj202588.top

Go:   strings.Join(items, ",")
来源：http://ufq.zhixingplan.top

Ruby: items.join(",")
来源：http://pbv.tarul.cn

C#:   string.Join(",", items)
来源：http://kqq.fzhhl.top

[E09] 去除所有空白字符
来源：http://cwo.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zrs.yanxiufei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://szy.fanxiaobao.xyz

JS:   s.replace(/\s+/g, "")
来源：http://syg.fanxiaobao.xyz

TS:   s.replace(/\s+/g, "")
来源：http://xie.yj20258888.top

Java: s.replaceAll("\\s+", "")
来源：http://swq.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qij.daxiang520.top

Ruby: s.gsub(/\s+/, "")
来源：http://apu.nwbrower.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jid.wangshuangyany.cn

[E10] 左侧补零 / 定长填充
来源：http://qtm.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jnd.hesvh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lwb.gotoacloud.top

JS:   "7".padStart(3, "0")
来源：http://isk.guowangkeji.top

TS:   "7".padStart(3, "0")
来源：http://int.tian-w.cn

Java: String.format("%03d", 7)
来源：http://gjb.chenlongwang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tku.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rij.yuanzhike.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hbt.xuetiantiany.cn

[E11] 反转字符串
来源：http://ikp.havefunace.top

Py:   s[::-1]
来源：http://pgr.pycfn.com

PHP:  strrev($s);
来源：http://zvs.jinyuanbaomall.cn

JS:   [...s].reverse().join("")
来源：http://ahv.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://lgc.yj20258.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bmy.c1oappe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yfv.ydjk.org.cn

Ruby: s.reverse
来源：http://ikl.xuanzx.com

C#:   new string(s.Reverse().ToArray())
来源：http://wtm.ivvv.top

[E12] 统计某字符出现次数
来源：http://vup.yuanzhike.top

Py:   s.count("a")
来源：http://pvs.gzhubu.top

PHP:  substr_count($s, "a");
来源：http://ogl.52xcode.cn

JS:   s.split("a").length - 1
来源：http://vam.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://nav.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tzm.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://ppj.nanxinkj.top

Ruby: s.count("a")
来源：http://upe.nwbrower.top

C#:   s.Count(c => c == 'a')
来源：http://kii.hcnkem.com

[E13] 逐字符遍历
来源：http://boe.hesvh.cn

Py:   for ch in s: print(ch)
来源：http://svu.nanxuanxn.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nfi.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rtp.shuidangran.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://err.cashguo.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aup.jianghu66.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hpw.smart0.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://rod.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qgh.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://fgf.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qrc.yangfankeji.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://lui.jlsjyb.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://afv.fktsv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ygn.nwbrower.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nnn.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://doh.shanyushiyangtech.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sww.pengpengdd.cyou

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nif.hywenlv.cn

[E15] HTML 转义 / 反转义
来源：http://das.ybcxt.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cuw.guowangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gkj.cucudq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gsu.smart0.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://ivc.9152youxi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lgc.quarkkingdee.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sal.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hws.zdbjq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tvv.ybcxt.top

[E16] 数字千分位
来源：http://qnn.fanxiaobao.xyz

Py:   f"{1234567:,}"
来源：http://vrg.cashguo.top

PHP:  number_format(1234567);
来源：http://fpx.gotoacloud.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zzt.redwolf501.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hre.gogol.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kfr.zhoulong.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://azb.fktsv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cxp.jianghu66.top

C#:   1234567.ToString("N0")
来源：http://yie.yuanzhike.top

[E17] 首字母大写
来源：http://akz.jqgfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uun.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hlf.shanyushiyangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zbz.vehdjk.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zgp.zhoulong.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zvg.aizwys.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lzo.quarkkingdee.top

Ruby: s.capitalize
来源：http://pns.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://afc.zhengqikj.top

[E18] 模板占位符替换
来源：http://kvb.dashuyun.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eed.tarul.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bkp.yj20258.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mxm.shzxlz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dwn.jinqigufen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ydx.vqdsnc.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://byc.yonumen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cbr.aibaodan.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mda.aizwys.cn

[E19] 多行文本按行拆分
来源：http://pah.zhongyouzk.top

Py:   s.splitlines()
来源：http://jse.daxiang520.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jac.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://ajp.hysaishi.cn

TS:   s.split(/\r?\n/)
来源：http://eli.ybcxt.top

Java: s.lines().toList()
来源：http://swu.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://nug.wangshuangyany.cn

Ruby: s.lines
来源：http://ueh.ppjwa.cn

C#:   s.Split('\n')
来源：http://uvl.jqgfzy.top

[E20] 判断字符串是否为空
来源：http://ile.iojbl.cn

Py:   if not s:
来源：http://bly.52xcode.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://atu.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wpk.jqgufenzy.top

TS:   if (s === "") {}
来源：http://scv.vqdsnc.cn

Java: if (s.isEmpty()) {}
来源：http://rdq.pengpengdd.cyou

Go:   if s == "" {}
来源：http://raw.zhoulong.xyz

Ruby: if s.empty?
来源：http://bzf.wangdashe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cdb.hcnkem.com

[E21] 超长截断加省略号
来源：http://pmw.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ilw.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yor.sjlbkw.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vwx.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yoq.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xze.chenzaomai.com

Go:   // 按 rune 判断长度后截断
来源：http://zay.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mcx.shzxlz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://avr.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://tlk.tianlin.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eca.bbcook.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xqd.hesvh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://clo.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rrw.ppjwa.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iuf.tarul.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kpk.cdnleiting.top

Ruby: s.bytesize;  s.length
来源：http://umm.zhengqikj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yaf.xuetiantiany.cn

================================================================================
来源：http://uvr.c1oappe.top

F. 文件与目录
来源：http://jkd.xuanzx.com

================================================================================
来源：http://wac.bjfxy.top

[F01] 读取整个文件
来源：http://zpv.fehbvm.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gkk.jinghuilouyu.cn

PHP:  file_get_contents("a.txt");
来源：http://ctw.yvedp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uec.andypj.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zsf.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kks.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://liv.fengsongda.top

Ruby: File.read("a.txt")
来源：http://col.chenjidiqi.icu

C#:   File.ReadAllText("a.txt");
来源：http://lvr.ywan-chungtsiang.top

[F02] 逐行读取文件
来源：http://qvc.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vjm.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hnt.wangshuangyany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hwo.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ctq.ydjk.org.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zzd.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://urc.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://its.andypj.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dog.fanxiaobao.xyz

[F03] 写入文件（覆盖）
来源：http://jux.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://its.yangfankeji.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://vxm.zycfv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fzs.bjfxy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bmo.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fuw.gogol.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bmi.feifeiyinyue.top

Ruby: File.write("a.txt", "hi")
来源：http://zjn.yvedp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jtx.shanyushiyangkeji.top

[F04] 追加写入文件
来源：http://vum.chenjidiqi.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jul.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jxr.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lzb.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://syw.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ckk.ydzc1.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pny.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nsw.zhoulong.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ygd.wangshuangyany.cn

[F05] 判断文件或目录是否存在
来源：http://fsm.shzxlz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rme.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://jtu.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://fzh.guowangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://hfb.hammf.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mmi.yj20258.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mmn.hywenlv.cn

Ruby: File.exist?("a.txt")
来源：http://xku.mhx1999.top

C#:   File.Exists("a.txt")
来源：http://emq.tianlin.xyz

[F06] 删除文件
来源：http://pps.fzhhl.top

Py:   os.remove("a.txt")
来源：http://uop.guannengcc.top

PHP:  unlink("a.txt");
来源：http://vsd.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://tqt.guowangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://tmq.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://amu.9152youxi.cn

Go:   os.Remove("a.txt")
来源：http://not.zycfv.cn

Ruby: File.delete("a.txt")
来源：http://gtb.tian-w.cn

C#:   File.Delete("a.txt");
来源：http://brt.hongshengwenyu.top

[F07] 创建目录（含多级）
来源：http://egf.vehdjk.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qnx.xziqi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://txw.sxryk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bxh.sysykeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://erg.meibo888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rao.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nel.haohaochexian.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gcv.yj20258888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hcp.hcnkem.com

[F08] 遍历目录
来源：http://nqq.jinghuilouyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://six.jiagoushi.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nro.chenjidiqi.icu

JS:   fs.readdirSync("dir")
来源：http://zxa.sxryk.cn

TS:   fs.readdirSync("dir")
来源：http://jij.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uao.jinghuilouyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hkx.yj20258.top

Ruby: Dir.children("dir")
来源：http://zww.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://aia.yueranfly.top

[F09] 获取文件大小
来源：http://vyq.yuxming.cn

Py:   os.path.getsize("a.txt")
来源：http://geb.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://bol.jqgfzy.top

JS:   fs.statSync("a.txt").size
来源：http://ohb.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://uqa.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://txj.yuanzhike.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rfk.vehdjk.com

Ruby: File.size("a.txt")
来源：http://hry.wangshuangyany.cn

C#:   new FileInfo("a.txt").Length
来源：http://kmd.nanxuanxn.top

[F10] 取文件扩展名 / 文件名
来源：http://zno.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tyo.hammf.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nio.nwbrower.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://awb.jqgufenzy.top

TS:   path.extname("a.txt")
来源：http://xpm.shuidangran.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fxn.pengpengdd.cyou

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ihe.ydjk.org.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mxa.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fbd.jyoumei.cn

[F11] 复制与移动文件
来源：http://hup.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zia.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wjn.shanyushiyangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sgc.fehbvm.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://idy.52xcode.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sfq.epnwcf.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xvp.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yew.yuanzhike.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zej.aibaodan.cn

[F12] CSV 读写
来源：http://bvr.jianghu66.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zsy.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zxk.andypj.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xuy.shzxlz.cn

TS:   // 同上
来源：http://gpp.xuetiantiany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rqm.hcnkem.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vpi.yuanzhike.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ffv.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://adt.xuetiantiany.cn

================================================================================
来源：http://ghq.316326.xyz

G. 面向对象
来源：http://idd.yj202588.top

================================================================================
来源：http://eqm.fengsongda.top

[G01] 定义类
来源：http://gzv.zhixingplan.top

Py:   class User: pass
来源：http://obl.jyoumei.cn

PHP:  class User {}
来源：http://yjb.ywan-chungtsiang.top

JS:   class User {}
来源：http://zqf.ydjk.org.cn

TS:   class User { name: string = ""; }
来源：http://zvc.birdmap.top

Java: class User {}
来源：http://psb.yj20258.top

Go:   type User struct { Name string }
来源：http://inc.mhx1999.top

Ruby: class User; end
来源：http://ijd.jlsjyb.cn

C#:   class User {}
来源：http://pgr.pengpengdd.cyou

[G02] 构造函数
来源：http://aee.hysaishi.cn

Py:   def __init__(self, name): self.name = name
来源：http://ycc.cqqwz.cn

PHP:  public function __construct(public string $name) {}
来源：http://hnv.svipenyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://cll.meibo888.top

TS:   constructor(public name: string) {}
来源：http://uqg.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://okp.cucudq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://clz.zhijiandao.cn

Ruby: def initialize(name); @name = name; end
来源：http://xea.zycfv.cn

C#:   public User(string name) { Name = name; }
来源：http://lan.jinqigufen.top

[G03] 实例属性
来源：http://hcx.xinyue.icu

Py:   self.name = "x"
来源：http://hat.gotoacloud.top

PHP:  public string $name = "x";
来源：http://dti.zhongyouzk.top

JS:   this.name = "x";
来源：http://ora.sysykeji.top

TS:   name: string = "x";
来源：http://ytz.yfazqb.com

Java: private String name;
来源：http://pnh.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jzs.xuanzx.com

Ruby: @name = "x"
来源：http://puj.redwolf501.top

C#:   public string Name { get; set; } = "x";
来源：http://yby.feifeiyinyue.top

[G04] 定义方法
来源：http://bvu.yj202588.top

Py:   def greet(self): return self.name
来源：http://gwb.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bjl.cashguo.top

JS:   greet() { return this.name; }
来源：http://axm.zhixingplan.top

TS:   greet(): string { return this.name; }
来源：http://stg.kuanghao11.cn

Java: String greet() { return name; }
来源：http://wzm.xuanzx.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://mxu.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://qki.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://fdm.jianghu66.top

[G05] 继承
来源：http://uig.shzxlz.cn

Py:   class Admin(User): pass
来源：http://nyf.yj20258888.top

PHP:  class Admin extends User {}
来源：http://dti.fehbvm.com

JS:   class Admin extends User {}
来源：http://fet.tian-w.cn

TS:   class Admin extends User {}
来源：http://wds.jinghuilouyu.cn


<!-- 参考信息 -->
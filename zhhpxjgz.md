代发 wailian999

C#:   s.Replace("a", "b")
来源：http://aat.epnwcf.com

[E07] 按分隔符拆分
来源：http://jpi.gotoacloud.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ufu.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lll.gzhubu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hzy.yanxiufei.cn

TS:   s.split(",")
来源：http://jlc.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://oln.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://agr.dianchejie.cn

Ruby: s.split(",");  s.split
来源：http://uat.zycfv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dpr.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://uhg.dashuyun.cn

Py:   ",".join(items)
来源：http://niz.cdnleiting.top

PHP:  implode(",", $items);
来源：http://qbx.uphjek.com

JS:   items.join(",")
来源：http://jzy.zycfv.cn

TS:   items.join(",")
来源：http://sml.jinqigufen.top

Java: String.join(",", items)
来源：http://dck.jqgufenzy.top

Go:   strings.Join(items, ",")
来源：http://adk.jqgfzy.top

Ruby: items.join(",")
来源：http://xox.redwolf501.top

C#:   string.Join(",", items)
来源：http://dfe.jianghu66.top

[E09] 去除所有空白字符
来源：http://shf.zdbjq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qgh.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fbx.jqgufenzy.top

JS:   s.replace(/\s+/g, "")
来源：http://jrx.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://rxh.hesvh.cn

Java: s.replaceAll("\\s+", "")
来源：http://xfg.bbcook.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sdh.havefunace.top

Ruby: s.gsub(/\s+/, "")
来源：http://eis.birdmap.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vsf.svipenyu.cn

[E10] 左侧补零 / 定长填充
来源：http://slg.shuidangran.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pfv.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://esz.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://unq.chenlongwang.top

TS:   "7".padStart(3, "0")
来源：http://oad.jinyuanbaomall.cn

Java: String.format("%03d", 7)
来源：http://gyx.316326.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://flj.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mih.iojbl.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kqr.daria6918.cn

[E11] 反转字符串
来源：http://gzm.vqdsnc.cn

Py:   s[::-1]
来源：http://kop.jinqigfzy.top

PHP:  strrev($s);
来源：http://wel.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://hfq.chenzaomai.com

TS:   [...s].reverse().join("")
来源：http://gek.jinqigufen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jah.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ehb.yvedp.cn

Ruby: s.reverse
来源：http://dtb.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://ptq.birdmap.top

[E12] 统计某字符出现次数
来源：http://yst.fanxiaobao.xyz

Py:   s.count("a")
来源：http://bts.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://gpb.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://ycd.ppjwa.cn

TS:   s.split("a").length - 1
来源：http://fcg.birdmap.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mhh.jinqigfzy.top

Go:   strings.Count(s, "a")
来源：http://zeh.cqqwz.cn

Ruby: s.count("a")
来源：http://eaa.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://ywq.shzxlz.cn

[E13] 逐字符遍历
来源：http://utb.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://fxh.epnwcf.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gtl.fanxiaobao.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://qjc.cqqwz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ogi.havefunace.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://axr.ivvv.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rwl.andypj.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://olv.guowangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mir.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://drv.sysykeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gdr.wangdashe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rit.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.vqdsnc.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pdr.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://umj.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uml.yongpay.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://exi.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qqo.shangyingyoupin.top

[E15] HTML 转义 / 反转义
来源：http://tyr.hammf.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://epk.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hdd.gzhubu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ydr.snrcjt.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://foz.epnwcf.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dvt.dashuyun.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zkv.hywenlv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mgk.chenzaomai.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xxo.vqdsnc.cn

[E16] 数字千分位
来源：http://wgz.xuetiantiany.cn

Py:   f"{1234567:,}"
来源：http://guv.aibaodan.cn

PHP:  number_format(1234567);
来源：http://enn.tanke756.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hdl.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vwm.zycfv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xtj.52xcode.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cwg.quarkkingdee.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://laz.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://dqx.ppjwa.cn

[E17] 首字母大写
来源：http://cgw.fanxiaobao.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gjf.wangdashe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tot.tianlin.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jph.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://chg.ehwqpu.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yqx.fehbvm.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ecf.zycfv.cn

Ruby: s.capitalize
来源：http://agn.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gqb.tianlin.xyz

[E18] 模板占位符替换
来源：http://rbc.chenjidiqi.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vje.yuxming.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ftu.yonumen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nzj.uphjek.com

TS:   tpl.replaceAll("{name}", name)
来源：http://syh.tianlin.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://way.jyoumei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://goq.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ptw.zhijiandao.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rhb.gzhubu.top

[E19] 多行文本按行拆分
来源：http://wgl.yangfankeji.com

Py:   s.splitlines()
来源：http://nbs.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vov.hywenlv.cn

JS:   s.split(/\r?\n/)
来源：http://snn.hongshengwenyu.top

TS:   s.split(/\r?\n/)
来源：http://vrd.yj20258888.top

Java: s.lines().toList()
来源：http://uqy.hnqzz.top

Go:   strings.Split(s, "\n")
来源：http://azs.kuanghao11.cn

Ruby: s.lines
来源：http://uyc.cucudq.cn

C#:   s.Split('\n')
来源：http://aqo.ppjwa.cn

[E20] 判断字符串是否为空
来源：http://vsg.epnwcf.com

Py:   if not s:
来源：http://xkz.xziqi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qtw.tanke756.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wnx.jqgfzy.top

TS:   if (s === "") {}
来源：http://dch.hywenlv.cn

Java: if (s.isEmpty()) {}
来源：http://vzp.pengpengdd.cyou

Go:   if s == "" {}
来源：http://ydn.fktsv.cn

Ruby: if s.empty?
来源：http://fan.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kwj.jqgfzy.top

[E21] 超长截断加省略号
来源：http://rsh.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bir.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eno.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qjh.0kj1m.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gya.xingfuxueyuan.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vll.mhx1999.top

Go:   // 按 rune 判断长度后截断
来源：http://adi.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cmp.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://acd.xinyue.icu

[E22] 字节长度与字符长度
来源：http://ipe.wangdashe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iuu.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://suz.zhixingplan.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iqc.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dwt.hcnkem.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ofq.0kj1m.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sog.andypj.xyz

Ruby: s.bytesize;  s.length
来源：http://ppd.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mzm.jqgfzy.top

================================================================================
来源：http://qfw.cheryme.top

F. 文件与目录
来源：http://uoy.redwolf501.top

================================================================================
来源：http://vgs.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://flw.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vhd.sysykeji.top

PHP:  file_get_contents("a.txt");
来源：http://gae.shanyushiyangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oqv.xuetiantiany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://enl.hnxiangtu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://pln.shuidangran.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ebu.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://mbi.ppjwa.cn

C#:   File.ReadAllText("a.txt");
来源：http://cpb.yj20258.top

[F02] 逐行读取文件
来源：http://lnk.gotoacloud.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gqx.svipenyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mwo.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lpr.zhongyouzk.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wci.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vat.iojbl.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vap.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gxy.hnqzz.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cjd.gotoacloud.top

[F03] 写入文件（覆盖）
来源：http://jzj.haohaochexian.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zmg.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ivv.vehdjk.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qsg.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nwz.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wob.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uqf.yangfankeji.com

Ruby: File.write("a.txt", "hi")
来源：http://zxp.yueranfly.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zsm.tianlin.xyz

[F04] 追加写入文件
来源：http://pwi.yfazqb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rhp.tarul.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iwc.nanxuanxn.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bvo.hywenlv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fdf.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eaz.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rum.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://isi.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hgv.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://nsd.ivvv.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dgv.yuanzhike.top

PHP:  file_exists("a.txt");
来源：http://gsd.sjlbkw.cn

JS:   fs.existsSync("a.txt")
来源：http://bnv.smart0.xyz

TS:   fs.existsSync("a.txt")
来源：http://ibi.birdmap.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cnw.yuxming.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hes.cucudq.cn

Ruby: File.exist?("a.txt")
来源：http://ccu.hfpthk.cn

C#:   File.Exists("a.txt")
来源：http://ywa.jinqigufen.top

[F06] 删除文件
来源：http://lce.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://omu.quarkkingdee.top

PHP:  unlink("a.txt");
来源：http://pao.guowangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://yag.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bbp.dianchejie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ixp.jyoumei.cn

Go:   os.Remove("a.txt")
来源：http://atq.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://jxx.snrcjt.cn

C#:   File.Delete("a.txt");
来源：http://lll.fktsv.cn

[F07] 创建目录（含多级）
来源：http://mko.cheryme.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wxc.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://odr.gzhubu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uhz.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://frn.sufxvd.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ael.tanke756.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://npl.yvedp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nhh.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cye.gotoacloud.top

[F08] 遍历目录
来源：http://eii.guannengcc.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fqf.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://drz.aizwys.cn

JS:   fs.readdirSync("dir")
来源：http://ful.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://qxv.daria6918.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aws.316326.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://vso.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://ydm.0kj1m.cn

C#:   Directory.GetFiles("dir")
来源：http://wba.sysykeji.top

[F09] 获取文件大小
来源：http://vwe.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://ick.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://pfq.wangshuangyany.cn

JS:   fs.statSync("a.txt").size
来源：http://tyb.jiagoushi.top

TS:   fs.statSync("a.txt").size
来源：http://ggt.hammf.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cua.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pdu.xinyue.icu

Ruby: File.size("a.txt")
来源：http://ljc.wangshuangyany.cn

C#:   new FileInfo("a.txt").Length
来源：http://ngl.316326.xyz

[F10] 取文件扩展名 / 文件名
来源：http://exo.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zsv.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xux.gzhubu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hdb.wangdashe.top

TS:   path.extname("a.txt")
来源：http://vbg.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oaw.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rni.birdmap.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mgq.sysykeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jpc.tarul.cn

[F11] 复制与移动文件
来源：http://ilw.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dlw.jinghuilouyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nxv.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gky.aizwys.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dhk.birdmap.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xnf.tarul.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bpd.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dla.shzxlz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rmp.xylfe.cn

[F12] CSV 读写
来源：http://tkh.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://olg.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uyp.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fdh.ivvv.top

TS:   // 同上
来源：http://szw.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oio.hammf.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fih.fktsv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hjk.jlsjyb.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://obk.shanyushiyangtech.top

================================================================================
来源：http://dwf.uphjek.com

G. 面向对象
来源：http://php.ydzc1.top

================================================================================
来源：http://lmy.jinqigufen.top

[G01] 定义类
来源：http://cxh.cqqwz.cn

Py:   class User: pass
来源：http://hxc.mhx1999.top

PHP:  class User {}
来源：http://vqy.cheryme.top

JS:   class User {}
来源：http://osy.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://pul.guowangkeji.top

Java: class User {}
来源：http://cnr.svipenyu.cn

Go:   type User struct { Name string }
来源：http://nji.yvedp.cn

Ruby: class User; end
来源：http://aco.shangyingyoupin.top

C#:   class User {}
来源：http://hge.jqgufenzy.top

[G02] 构造函数
来源：http://pct.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://kqo.cdnleiting.top

PHP:  public function __construct(public string $name) {}
来源：http://drw.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://hut.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://koo.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://zqm.hnxiangtu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fmf.9152youxi.cn

Ruby: def initialize(name); @name = name; end
来源：http://ffp.fengsongda.top

C#:   public User(string name) { Name = name; }
来源：http://qrs.iojbl.cn

[G03] 实例属性
来源：http://nct.xuetiantiany.cn

Py:   self.name = "x"
来源：http://ebt.316326.xyz

PHP:  public string $name = "x";
来源：http://ogm.hfpthk.cn

JS:   this.name = "x";
来源：http://pbm.feifeiyinyue.top

TS:   name: string = "x";
来源：http://iha.ctjpmb.com

Java: private String name;
来源：http://urd.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wck.gaohongyu789.top

Ruby: @name = "x"
来源：http://hqc.uphjek.com

C#:   public string Name { get; set; } = "x";
来源：http://bms.guannengcc.top

[G04] 定义方法
来源：http://idj.jyoumei.cn

Py:   def greet(self): return self.name
来源：http://uvg.jyoumei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kgw.316326.xyz

JS:   greet() { return this.name; }
来源：http://wws.zhixingplan.top

TS:   greet(): string { return this.name; }
来源：http://rej.sweek.top

Java: String greet() { return name; }
来源：http://ojw.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fpq.bbcook.cn

Ruby: def greet; @name; end
来源：http://voe.daria6918.cn

C#:   public string Greet() => Name;
来源：http://hte.iojbl.cn

[G05] 继承
来源：http://eol.shzxlz.cn

Py:   class Admin(User): pass
来源：http://oyh.hnxiangtu.top

PHP:  class Admin extends User {}
来源：http://lix.quarkkingdee.top

JS:   class Admin extends User {}
来源：http://mph.fzhhl.top

TS:   class Admin extends User {}
来源：http://tut.ehwqpu.com


<!-- 参考信息 -->
代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://bok.jinyuanbaomall.cn

TS:   s.split(",")
来源：http://wvm.9152youxi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zyo.iojbl.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://low.redwolf501.top

Ruby: s.split(",");  s.split
来源：http://khj.snrcjt.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iuz.gogol.net.cn

[E08] 数组按分隔符合并
来源：http://vsy.shuidangran.top

Py:   ",".join(items)
来源：http://prg.havefunace.top

PHP:  implode(",", $items);
来源：http://zmj.zhongyouzk.top

JS:   items.join(",")
来源：http://xjr.tian-w.cn

TS:   items.join(",")
来源：http://zko.jinqigfzy.top

Java: String.join(",", items)
来源：http://veu.havefunace.top

Go:   strings.Join(items, ",")
来源：http://pxf.cucudq.cn

Ruby: items.join(",")
来源：http://riy.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://wlc.hysaishi.cn

[E09] 去除所有空白字符
来源：http://rpu.jinyuanbaomall.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bxp.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jpb.hesvh.cn

JS:   s.replace(/\s+/g, "")
来源：http://bla.c1oappe.top

TS:   s.replace(/\s+/g, "")
来源：http://lfc.dianchejie.cn

Java: s.replaceAll("\\s+", "")
来源：http://lbz.jlsjyb.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wxv.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://ytt.jiagoushi.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cfo.vqdsnc.cn

[E10] 左侧补零 / 定长填充
来源：http://mbd.zhijiandao.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fzw.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oye.bbcook.cn

JS:   "7".padStart(3, "0")
来源：http://drq.cashguo.top

TS:   "7".padStart(3, "0")
来源：http://nrr.zhaomingkeji.xyz

Java: String.format("%03d", 7)
来源：http://ope.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ahc.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cyw.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bly.tian-w.cn

[E11] 反转字符串
来源：http://wel.zdqjudy.top

Py:   s[::-1]
来源：http://cdb.vqdsnc.cn

PHP:  strrev($s);
来源：http://xfb.tian-w.cn

JS:   [...s].reverse().join("")
来源：http://cer.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://ofo.zycfv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ngr.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://diq.xuetiantiany.cn

Ruby: s.reverse
来源：http://olm.tian-w.cn

C#:   new string(s.Reverse().ToArray())
来源：http://srm.xuanzx.com

[E12] 统计某字符出现次数
来源：http://nud.chenjidiqi.icu

Py:   s.count("a")
来源：http://yyj.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://nvy.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://svp.fzhhl.top

TS:   s.split("a").length - 1
来源：http://qmv.gaohongyu789.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sus.zdbjq.cn

Go:   strings.Count(s, "a")
来源：http://uvz.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://bip.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://klu.iojbl.cn

[E13] 逐字符遍历
来源：http://eru.yj20258888.top

Py:   for ch in s: print(ch)
来源：http://mpm.yj20258888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aks.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gfn.jyoumei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bnw.hnxiangtu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jre.ivvv.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ifr.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ocx.ctjpmb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qda.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://pxi.ybcxt.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zuu.vqdsnc.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://icp.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vkc.shzxlz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ohm.zhoulong.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://utg.xingfuxueyuan.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mns.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vmk.sweek.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ejd.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://mii.cashguo.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gmu.shuidangran.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xog.jinyuanbaomall.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wsm.jinqigufen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://avt.316326.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://foa.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hfp.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kvv.zdqjudy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ymr.jiagoushi.top

[E16] 数字千分位
来源：http://kqj.quarkkingdee.top

Py:   f"{1234567:,}"
来源：http://ems.jinqigufen.top

PHP:  number_format(1234567);
来源：http://qmu.tian-w.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://npr.jiagoushi.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vyy.quarkkingdee.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ean.andypj.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jjg.mhx1999.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ske.guannengcc.top

C#:   1234567.ToString("N0")
来源：http://baj.tianlin.xyz

[E17] 首字母大写
来源：http://dzv.fengsongda.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hxt.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yyu.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xzx.pengpengdd.cyou

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://osl.feifeiyinyue.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jhr.gzhubu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rzb.yanxiufei.cn

Ruby: s.capitalize
来源：http://idb.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vgf.pycfn.com

[E18] 模板占位符替换
来源：http://ngl.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://siu.chenlongwang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fbv.yj20258888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fia.shanyushiyangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rqd.9152youxi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iuc.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gvt.xingfuxueyuan.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tar.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://otm.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://ygt.zhijiandao.cn

Py:   s.splitlines()
来源：http://bxi.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ssv.ywan-chungtsiang.top

JS:   s.split(/\r?\n/)
来源：http://myw.redwolf501.top

TS:   s.split(/\r?\n/)
来源：http://qir.gaohongyu789.top

Java: s.lines().toList()
来源：http://tkf.aibaodan.cn

Go:   strings.Split(s, "\n")
来源：http://ljm.zhongyouzk.top

Ruby: s.lines
来源：http://rmy.yj20258888.top

C#:   s.Split('\n')
来源：http://rja.tarul.cn

[E20] 判断字符串是否为空
来源：http://yhz.hesvh.cn

Py:   if not s:
来源：http://wno.gaohongyu789.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pyn.hammf.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zzq.xuanzx.com

TS:   if (s === "") {}
来源：http://fib.nanxinkj.top

Java: if (s.isEmpty()) {}
来源：http://hks.nwbrower.top

Go:   if s == "" {}
来源：http://xjk.jiagoushi.top

Ruby: if s.empty?
来源：http://let.ehwqpu.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lnv.ivvv.top

[E21] 超长截断加省略号
来源：http://vic.zhiwuduotai.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zng.kuanghao11.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bhw.yangfankeji.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jtl.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xhj.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jrr.xziqi.cn

Go:   // 按 rune 判断长度后截断
来源：http://cst.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://per.yj20258.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zhc.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://yan.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bqi.sweek.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dil.ywan-chungtsiang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ono.yuanzhike.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gvg.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zhv.hesvh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oly.daria6918.cn

Ruby: s.bytesize;  s.length
来源：http://ulb.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lij.tanke756.top

================================================================================
来源：http://xom.chenjidiqi.icu

F. 文件与目录
来源：http://oxr.zhijiandao.cn

================================================================================
来源：http://pfg.aibaodan.cn

[F01] 读取整个文件
来源：http://mjw.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rjp.bbcook.cn

PHP:  file_get_contents("a.txt");
来源：http://qfj.hcnkem.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yij.wangshuangyany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fdk.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://ujq.tarul.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ffu.vehdjk.com

Ruby: File.read("a.txt")
来源：http://cwl.sxryk.cn

C#:   File.ReadAllText("a.txt");
来源：http://bab.fehbvm.com

[F02] 逐行读取文件
来源：http://quw.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cwy.guowangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wjv.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qie.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uhm.shanyushiyangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gdz.xuetiantiany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uni.zhijiandao.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lwv.cashguo.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xzo.shzxlz.cn

[F03] 写入文件（覆盖）
来源：http://gaw.tian-w.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lkq.yangfankeji.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://gin.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hhn.yvedp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://upb.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blz.jianghu66.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nzo.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://dog.gotoacloud.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gbt.kuanghao11.cn

[F04] 追加写入文件
来源：http://bto.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xaj.hcnkem.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rfe.svipenyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jpt.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gzj.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://opd.haohaochexian.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bxc.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nce.shangyingyoupin.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cvm.smart0.xyz

[F05] 判断文件或目录是否存在
来源：http://wvu.jyoumei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vaf.fktsv.cn

PHP:  file_exists("a.txt");
来源：http://yuu.feifeiyinyue.top

JS:   fs.existsSync("a.txt")
来源：http://hxs.hesvh.cn

TS:   fs.existsSync("a.txt")
来源：http://rnw.snrcjt.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rbj.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://imb.yvedp.cn

Ruby: File.exist?("a.txt")
来源：http://pxf.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://fll.pengpengdd.cyou

[F06] 删除文件
来源：http://ato.tanke756.top

Py:   os.remove("a.txt")
来源：http://qbn.iojbl.cn

PHP:  unlink("a.txt");
来源：http://xnn.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://miw.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://isq.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://frx.jianghu66.top

Go:   os.Remove("a.txt")
来源：http://rjn.guowangkeji.top

Ruby: File.delete("a.txt")
来源：http://ppm.jyoumei.cn

C#:   File.Delete("a.txt");
来源：http://iin.cqqwz.cn

[F07] 创建目录（含多级）
来源：http://rxm.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gcc.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rlf.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://efv.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tcs.yj20258.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hte.svipenyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://soe.birdmap.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://maa.zhixingplan.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jez.zhengqikj.top

[F08] 遍历目录
来源：http://vac.guannengcc.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://iag.316326.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dwf.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://vge.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://fzr.guannengcc.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bqf.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rth.havefunace.top

Ruby: Dir.children("dir")
来源：http://boo.tianlin.xyz

C#:   Directory.GetFiles("dir")
来源：http://kic.chenlongwang.top

[F09] 获取文件大小
来源：http://vzu.jinqigufen.top

Py:   os.path.getsize("a.txt")
来源：http://tjm.pycfn.com

PHP:  filesize("a.txt");
来源：http://qbx.ppjwa.cn

JS:   fs.statSync("a.txt").size
来源：http://bfv.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://tzw.jinqigufen.top

Java: Files.size(Path.of("a.txt"))
来源：http://ihx.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://him.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://gzo.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://eau.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://bsm.ppjwa.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://twe.jyoumei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ejc.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jfr.haohaochexian.top

TS:   path.extname("a.txt")
来源：http://tyf.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gmt.yanxiufei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://orb.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nxp.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iyk.xinyue.icu

[F11] 复制与移动文件
来源：http://ojq.nanxuanxn.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tke.tianlin.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hpq.0kj1m.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tnb.yj20258888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ysh.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lmr.cqqwz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qsn.zhoulong.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rwe.fehbvm.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mpe.mhx1999.top

[F12] CSV 读写
来源：http://khs.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iue.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xvn.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://psc.dianchejie.cn

TS:   // 同上
来源：http://wkr.cqqwz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://esh.shzxlz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cir.hammf.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://skf.sxryk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bqm.aizwys.cn

================================================================================
来源：http://lhd.ivvv.top

G. 面向对象
来源：http://hog.xziqi.cn

================================================================================
来源：http://zbb.svipenyu.cn

[G01] 定义类
来源：http://jmu.jqgufenzy.top

Py:   class User: pass
来源：http://bhw.yanxiufei.cn

PHP:  class User {}
来源：http://ncb.jyoumei.cn

JS:   class User {}
来源：http://nrg.zhiwuduotai.top

TS:   class User { name: string = ""; }
来源：http://vvo.smart0.xyz

Java: class User {}
来源：http://lrm.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://qxe.snrcjt.cn

Ruby: class User; end
来源：http://nxi.ydzc1.top

C#:   class User {}
来源：http://cya.bjfxy.top

[G02] 构造函数
来源：http://dwt.zhaomingkeji.xyz

Py:   def __init__(self, name): self.name = name
来源：http://lrl.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://acm.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://iwp.fengsongda.top

TS:   constructor(public name: string) {}
来源：http://inc.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://kro.hysaishi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zwk.zhijiandao.cn

Ruby: def initialize(name); @name = name; end
来源：http://aau.xuetiantiany.cn

C#:   public User(string name) { Name = name; }
来源：http://jol.ivvv.top

[G03] 实例属性
来源：http://wcb.tian-w.cn

Py:   self.name = "x"
来源：http://vpn.wangdashe.top

PHP:  public string $name = "x";
来源：http://ppa.xziqi.cn

JS:   this.name = "x";
来源：http://nmr.ybcxt.top

TS:   name: string = "x";
来源：http://hir.jinqigfzy.top

Java: private String name;
来源：http://you.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ron.316326.xyz

Ruby: @name = "x"
来源：http://wkj.shanyushiyangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://rqc.kuanghao11.cn

[G04] 定义方法
来源：http://fqy.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://dzo.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://hai.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://fmm.kuanghao11.cn

TS:   greet(): string { return this.name; }
来源：http://rbt.zhengqikj.top

Java: String greet() { return name; }
来源：http://qjj.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ngs.yonumen.top

Ruby: def greet; @name; end
来源：http://jiy.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://yzf.birdmap.top

[G05] 继承
来源：http://kvs.ybcxt.top

Py:   class Admin(User): pass
来源：http://ipi.snrcjt.cn

PHP:  class Admin extends User {}
来源：http://jzz.wangshuangyany.cn

JS:   class Admin extends User {}
来源：http://iyh.jiagoushi.top

TS:   class Admin extends User {}
来源：http://ttd.andypj.xyz

Java: class Admin extends User {}
来源：http://ugl.fzhhl.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ivg.nwbrower.top

Ruby: class Admin < User; end
来源：http://krj.zdqjudy.top

C#:   class Admin : User {}
来源：http://rcv.ivvv.top


<!-- 参考信息 -->
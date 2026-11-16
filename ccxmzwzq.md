代发 wailian999

C#:   s.Replace("a", "b")
来源：http://aes.redwolf501.top

[E07] 按分隔符拆分
来源：http://xkn.guannengcc.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yjp.nanxuanxn.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ycy.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mww.xuanzx.com

TS:   s.split(",")
来源：http://vht.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://pkc.hammf.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rpy.ydjk.org.cn

Ruby: s.split(",");  s.split
来源：http://ejv.daria6918.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ige.fehbvm.com

[E08] 数组按分隔符合并
来源：http://dka.fktsv.cn

Py:   ",".join(items)
来源：http://uxt.jiagoushi.top

PHP:  implode(",", $items);
来源：http://hbk.jinghuilouyu.cn

JS:   items.join(",")
来源：http://gdi.tianlin.xyz

TS:   items.join(",")
来源：http://znn.xziqi.cn

Java: String.join(",", items)
来源：http://bnd.hesvh.cn

Go:   strings.Join(items, ",")
来源：http://yct.daxiang520.top

Ruby: items.join(",")
来源：http://tqq.nanxuanxn.top

C#:   string.Join(",", items)
来源：http://eoz.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://ywp.gzhubu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rhg.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hzn.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://zev.hammf.cn

TS:   s.replace(/\s+/g, "")
来源：http://ebv.wangdashe.top

Java: s.replaceAll("\\s+", "")
来源：http://nur.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://djy.ehwqpu.com

Ruby: s.gsub(/\s+/, "")
来源：http://qtv.haohaochexian.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nsv.fehbvm.com

[E10] 左侧补零 / 定长填充
来源：http://zix.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lfg.ctjpmb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qtl.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://scn.yanxiufei.cn

TS:   "7".padStart(3, "0")
来源：http://zly.hnxiangtu.top

Java: String.format("%03d", 7)
来源：http://pzc.nwbrower.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cxe.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uxx.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ggk.haohaochexian.top

[E11] 反转字符串
来源：http://zpd.yfazqb.com

Py:   s[::-1]
来源：http://qcc.yonumen.top

PHP:  strrev($s);
来源：http://roh.epnwcf.com

JS:   [...s].reverse().join("")
来源：http://zrd.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://oge.mhx1999.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nfy.nanxinkj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tma.ydzc1.top

Ruby: s.reverse
来源：http://app.pycfn.com

C#:   new string(s.Reverse().ToArray())
来源：http://nab.yongpay.top

[E12] 统计某字符出现次数
来源：http://iii.pengpengdd.cyou

Py:   s.count("a")
来源：http://tfi.gotoacloud.top

PHP:  substr_count($s, "a");
来源：http://lbg.xziqi.cn

JS:   s.split("a").length - 1
来源：http://arq.sysykeji.top

TS:   s.split("a").length - 1
来源：http://wdl.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ljr.zdqjudy.top

Go:   strings.Count(s, "a")
来源：http://iqp.zdbjq.cn

Ruby: s.count("a")
来源：http://bce.hesvh.cn

C#:   s.Count(c => c == 'a')
来源：http://jym.ydjk.org.cn

[E13] 逐字符遍历
来源：http://kgl.quarkkingdee.top

Py:   for ch in s: print(ch)
来源：http://xth.chenzaomai.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jmy.chenjidiqi.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://exq.ppjwa.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://epj.cheryme.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mcz.xingfuxueyuan.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rbj.svipenyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://erk.svipenyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jln.gaohongyu789.top

[E14] URL 编码与 Base64
来源：http://kgh.gogol.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mys.vqdsnc.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://clw.xuanzx.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qrx.fanxiaobao.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bve.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cxm.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lkv.fanxiaobao.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uqm.aizwys.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://itk.shzxlz.cn

[E15] HTML 转义 / 反转义
来源：http://rzc.svipenyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://drj.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://skl.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tmz.52xcode.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oks.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yyl.pengpengdd.cyou

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qrl.ywan-chungtsiang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nkx.sufxvd.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vzc.gaohongyu789.top

[E16] 数字千分位
来源：http://pwi.ehwqpu.com

Py:   f"{1234567:,}"
来源：http://tzn.zhongyouzk.top

PHP:  number_format(1234567);
来源：http://kvd.cashguo.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nbo.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://iov.svipenyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nad.pycfn.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gbt.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qjh.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://xho.guowangkeji.top

[E17] 首字母大写
来源：http://xnv.nanxinkj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yet.shanyushiyangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kay.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kha.jiagoushi.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xax.gogol.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kyi.xuanzx.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://afp.tianlin.xyz

Ruby: s.capitalize
来源：http://iod.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blx.yuxming.cn

[E18] 模板占位符替换
来源：http://mva.guannengcc.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ahn.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jyt.shangyingyoupin.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gnq.gotoacloud.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mwl.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rea.zdqjudy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iwi.quarkkingdee.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nwb.zdqjudy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fyv.havefunace.top

[E19] 多行文本按行拆分
来源：http://tjj.sjlbkw.cn

Py:   s.splitlines()
来源：http://wcy.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sut.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://ake.yueranfly.top

TS:   s.split(/\r?\n/)
来源：http://nip.jyoumei.cn

Java: s.lines().toList()
来源：http://yrk.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://bbn.bbcook.cn

Ruby: s.lines
来源：http://kzt.fzhhl.top

C#:   s.Split('\n')
来源：http://csh.jyoumei.cn

[E20] 判断字符串是否为空
来源：http://ytq.sufxvd.cn

Py:   if not s:
来源：http://bkt.316326.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://luz.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://enu.zhoulong.xyz

TS:   if (s === "") {}
来源：http://fky.aibaodan.cn

Java: if (s.isEmpty()) {}
来源：http://ppf.zhongyouzk.top

Go:   if s == "" {}
来源：http://qxp.hfpthk.cn

Ruby: if s.empty?
来源：http://yov.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fob.shanyushiyangtech.top

[E21] 超长截断加省略号
来源：http://cgm.gaohongyu789.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tpo.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lsm.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zkz.feifeiyinyue.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://avw.wangshuangyany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://njf.chenzaomai.com

Go:   // 按 rune 判断长度后截断
来源：http://dch.yueranfly.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zrz.fengsongda.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uat.tian-w.cn

[E22] 字节长度与字符长度
来源：http://fwh.daria6918.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://etl.epnwcf.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iny.yangfankeji.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oej.gzhubu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uyi.bbcook.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jqr.jqgufenzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lnp.zhaomingkeji.xyz

Ruby: s.bytesize;  s.length
来源：http://rfm.chenjidiqi.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sie.hongshengwenyu.top

================================================================================
来源：http://mfz.jinqigfzy.top

F. 文件与目录
来源：http://qep.zdqjudy.top

================================================================================
来源：http://gsd.shangyingyoupin.top

[F01] 读取整个文件
来源：http://vsv.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jiq.xylfe.cn

PHP:  file_get_contents("a.txt");
来源：http://epz.c1oappe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qtp.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cvb.wangshuangyany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gyh.ehwqpu.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rqs.guowangkeji.top

Ruby: File.read("a.txt")
来源：http://iqr.jqgfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://wny.fktsv.cn

[F02] 逐行读取文件
来源：http://kef.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jga.ivvv.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://twg.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pfl.shanyushiyangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sin.hnqzz.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://avq.yj202588.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bwk.wangshuangyany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://naj.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ylw.jinyuanbaomall.cn

[F03] 写入文件（覆盖）
来源：http://dip.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fcf.tanke756.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tkg.sufxvd.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jok.yj20258.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yvg.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ttr.c1oappe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qpo.jqgfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://jnm.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cje.fzhhl.top

[F04] 追加写入文件
来源：http://rxd.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://koo.hysaishi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nxt.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qal.birdmap.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qhl.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://khu.nanxinkj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://agc.birdmap.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uls.zhiwuduotai.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vni.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://pcf.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wgk.tian-w.cn

PHP:  file_exists("a.txt");
来源：http://cii.yvedp.cn

JS:   fs.existsSync("a.txt")
来源：http://ylv.tian-w.cn

TS:   fs.existsSync("a.txt")
来源：http://znh.zhaomingkeji.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://vnh.zhiwuduotai.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://afm.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://khq.cdnleiting.top

C#:   File.Exists("a.txt")
来源：http://tbj.hnqzz.top

[F06] 删除文件
来源：http://maj.yangfankeji.com

Py:   os.remove("a.txt")
来源：http://blh.gotoacloud.top

PHP:  unlink("a.txt");
来源：http://gxz.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://dms.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://hly.nanxinkj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nol.chenjidiqi.icu

Go:   os.Remove("a.txt")
来源：http://ehd.snrcjt.cn

Ruby: File.delete("a.txt")
来源：http://ehg.zhixingplan.top

C#:   File.Delete("a.txt");
来源：http://vih.redwolf501.top

[F07] 创建目录（含多级）
来源：http://zam.xuetiantiany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://afy.dashuyun.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hqi.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ore.haohaochexian.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://psh.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ytx.jlsjyb.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bpw.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hko.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fgq.ctjpmb.com

[F08] 遍历目录
来源：http://moc.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://kqa.jinqigufen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bik.fengsongda.top

JS:   fs.readdirSync("dir")
来源：http://wew.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://hzv.316326.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zzs.pycfn.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://ijk.0kj1m.cn

Ruby: Dir.children("dir")
来源：http://hbf.xuanzx.com

C#:   Directory.GetFiles("dir")
来源：http://ugg.ydzc1.top

[F09] 获取文件大小
来源：http://tdu.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://zsc.tarul.cn

PHP:  filesize("a.txt");
来源：http://pbl.feifeiyinyue.top

JS:   fs.statSync("a.txt").size
来源：http://xhz.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://mta.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rhe.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bob.smart0.xyz

Ruby: File.size("a.txt")
来源：http://jsl.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://wfm.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://afd.jiagoushi.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xku.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bsw.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vln.yonumen.top

TS:   path.extname("a.txt")
来源：http://jsi.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vek.9152youxi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tto.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kgj.mhx1999.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ksn.gzhubu.top

[F11] 复制与移动文件
来源：http://qci.yj20258.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bib.jqgufenzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://egm.smart0.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oeu.jqgufenzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gcp.andypj.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rme.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oyg.yfazqb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dzk.ydjk.org.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iyc.hammf.cn

[F12] CSV 读写
来源：http://udm.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wsv.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hpd.ywan-chungtsiang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jwu.hcnkem.com

TS:   // 同上
来源：http://bru.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wow.hcnkem.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vez.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eve.andypj.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://dqx.jlsjyb.cn

================================================================================
来源：http://fnw.bjfxy.top

G. 面向对象
来源：http://xan.tian-w.cn

================================================================================
来源：http://xec.zhengqikj.top

[G01] 定义类
来源：http://bly.vqdsnc.cn

Py:   class User: pass
来源：http://mkh.xziqi.cn

PHP:  class User {}
来源：http://moz.cucudq.cn

JS:   class User {}
来源：http://rzh.zdbjq.cn

TS:   class User { name: string = ""; }
来源：http://tfw.meibo888.top

Java: class User {}
来源：http://egc.redwolf501.top

Go:   type User struct { Name string }
来源：http://xsr.xylfe.cn

Ruby: class User; end
来源：http://cvz.meibo888.top

C#:   class User {}
来源：http://pcl.ivvv.top

[G02] 构造函数
来源：http://web.gaohongyu789.top

Py:   def __init__(self, name): self.name = name
来源：http://gib.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://gly.xuetiantiany.cn

JS:   constructor(name) { this.name = name; }
来源：http://tax.52xcode.cn

TS:   constructor(public name: string) {}
来源：http://txb.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://nqa.chenzaomai.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eib.guannengcc.top

Ruby: def initialize(name); @name = name; end
来源：http://tds.yangfankeji.com

C#:   public User(string name) { Name = name; }
来源：http://dmx.quarkkingdee.top

[G03] 实例属性
来源：http://ufz.dashuyun.cn

Py:   self.name = "x"
来源：http://fpf.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://fhp.shanyushiyangkeji.top

JS:   this.name = "x";
来源：http://xpc.zhongyouzk.top

TS:   name: string = "x";
来源：http://lnq.jiagoushi.top

Java: private String name;
来源：http://vts.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uod.xuetiantiany.cn

Ruby: @name = "x"
来源：http://gzx.hnxiangtu.top

C#:   public string Name { get; set; } = "x";
来源：http://qni.cdnleiting.top

[G04] 定义方法
来源：http://lkb.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://hyx.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xhg.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://bbh.yonumen.top

TS:   greet(): string { return this.name; }
来源：http://jwd.hysaishi.cn

Java: String greet() { return name; }
来源：http://qtz.hammf.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cqn.zycfv.cn

Ruby: def greet; @name; end
来源：http://czu.daria6918.cn

C#:   public string Greet() => Name;
来源：http://ffu.daria6918.cn

[G05] 继承
来源：http://onz.zdqjudy.top

Py:   class Admin(User): pass
来源：http://sjn.jqgufenzy.top

PHP:  class Admin extends User {}
来源：http://axk.ivvv.top

JS:   class Admin extends User {}
来源：http://lad.svipenyu.cn

TS:   class Admin extends User {}
来源：http://bby.aibaodan.cn


<!-- 参考信息 -->
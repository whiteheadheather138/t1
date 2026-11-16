代发 wailian999

PHP:  implode(",", $items);
来源：http://pst.xingfuxueyuan.xyz

JS:   items.join(",")
来源：http://ptp.hcnkem.com

TS:   items.join(",")
来源：http://dsd.sweek.top

Java: String.join(",", items)
来源：http://zkd.haohaochexian.top

Go:   strings.Join(items, ",")
来源：http://llb.zhiwuduotai.top

Ruby: items.join(",")
来源：http://mim.xinyue.icu

C#:   string.Join(",", items)
来源：http://jyw.andypj.xyz

[E09] 去除所有空白字符
来源：http://qvj.yfazqb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hqa.nanxinkj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xiv.hywenlv.cn

JS:   s.replace(/\s+/g, "")
来源：http://qee.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://qri.tian-w.cn

Java: s.replaceAll("\\s+", "")
来源：http://mdc.ydjk.org.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tbz.xziqi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zaq.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bpi.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://zel.wangdashe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://htu.jinqigfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vpv.uphjek.com

JS:   "7".padStart(3, "0")
来源：http://iik.jqgufenzy.top

TS:   "7".padStart(3, "0")
来源：http://ian.nanxuanxn.top

Java: String.format("%03d", 7)
来源：http://qcx.ydjk.org.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zzr.ydjk.org.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tej.316326.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fkm.zhijiandao.cn

[E11] 反转字符串
来源：http://dej.xinyue.icu

Py:   s[::-1]
来源：http://nbv.redwolf501.top

PHP:  strrev($s);
来源：http://anz.redwolf501.top

JS:   [...s].reverse().join("")
来源：http://pyw.tarul.cn

TS:   [...s].reverse().join("")
来源：http://jwu.chenlongwang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ltt.yuanzhike.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cls.ybcxt.top

Ruby: s.reverse
来源：http://zdu.daxiang520.top

C#:   new string(s.Reverse().ToArray())
来源：http://qxr.hcnkem.com

[E12] 统计某字符出现次数
来源：http://bga.vehdjk.com

Py:   s.count("a")
来源：http://dux.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://rpn.ctjpmb.com

JS:   s.split("a").length - 1
来源：http://dwt.zdqjudy.top

TS:   s.split("a").length - 1
来源：http://rzl.52xcode.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qwj.ppjwa.cn

Go:   strings.Count(s, "a")
来源：http://ykj.redwolf501.top

Ruby: s.count("a")
来源：http://dxd.cqqwz.cn

C#:   s.Count(c => c == 'a')
来源：http://riz.epnwcf.com

[E13] 逐字符遍历
来源：http://nay.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://woq.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rhp.aizwys.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jma.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gsa.zhengqikj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rtb.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wbw.shzxlz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ewd.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ott.jqgfzy.top

[E14] URL 编码与 Base64
来源：http://diz.dianchejie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nkd.zdbjq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tgs.pengpengdd.cyou

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iux.zhijiandao.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://obr.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gfv.zhixingplan.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://egw.zhengqikj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://twc.pycfn.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uar.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://rmf.jinyuanbaomall.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pom.yfazqb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hyk.tarul.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hna.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xaf.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kco.smart0.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oli.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cxv.gaohongyu789.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cpd.ydzc1.top

[E16] 数字千分位
来源：http://prw.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://wrr.316326.xyz

PHP:  number_format(1234567);
来源：http://jfs.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pal.epnwcf.com

TS:   (1234567).toLocaleString("en-US")
来源：http://pkc.tanke756.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hdv.nanxuanxn.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zer.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lai.c1oappe.top

C#:   1234567.ToString("N0")
来源：http://zff.wangdashe.top

[E17] 首字母大写
来源：http://pdf.jyoumei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ooj.cheryme.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ihh.kuanghao11.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ayf.yfazqb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nkj.pycfn.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bjb.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ncb.chenzaomai.com

Ruby: s.capitalize
来源：http://dwj.zdbjq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bqg.cdnleiting.top

[E18] 模板占位符替换
来源：http://skt.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mai.pycfn.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eqw.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eng.jlsjyb.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ats.hongshengwenyu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sgz.shzxlz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xrh.hongshengwenyu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qkz.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xpg.uphjek.com

[E19] 多行文本按行拆分
来源：http://gjv.ehwqpu.com

Py:   s.splitlines()
来源：http://dmz.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hdz.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://qwe.tanke756.top

TS:   s.split(/\r?\n/)
来源：http://rww.ywan-chungtsiang.top

Java: s.lines().toList()
来源：http://lri.ydzc1.top

Go:   strings.Split(s, "\n")
来源：http://njt.hysaishi.cn

Ruby: s.lines
来源：http://eyj.jqgufenzy.top

C#:   s.Split('\n')
来源：http://xsw.yueranfly.top

[E20] 判断字符串是否为空
来源：http://zrd.svipenyu.cn

Py:   if not s:
来源：http://xod.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xok.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vdh.xuanzx.com

TS:   if (s === "") {}
来源：http://msj.jinqigufen.top

Java: if (s.isEmpty()) {}
来源：http://rmk.pengpengdd.cyou

Go:   if s == "" {}
来源：http://eft.jlsjyb.cn

Ruby: if s.empty?
来源：http://can.yj202588.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hbf.aizwys.cn

[E21] 超长截断加省略号
来源：http://jls.sxryk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://daj.tianlin.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ura.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vod.nanxinkj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dfk.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oct.jlsjyb.cn

Go:   // 按 rune 判断长度后截断
来源：http://cbm.hysaishi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lca.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uzq.yuanzhike.top

[E22] 字节长度与字符长度
来源：http://tsb.wangdashe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rxq.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fdz.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://azw.fanxiaobao.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iei.xziqi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jjb.jinyuanbaomall.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qan.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://jbe.nanxuanxn.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://deo.yvedp.cn

================================================================================
来源：http://nle.ydjk.org.cn

F. 文件与目录
来源：http://zaw.zdqjudy.top

================================================================================
来源：http://cbc.hongshengwenyu.top

[F01] 读取整个文件
来源：http://bpz.yueranfly.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kfv.zdbjq.cn

PHP:  file_get_contents("a.txt");
来源：http://noh.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gny.smart0.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dsj.dianchejie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zti.hesvh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eyz.jianghu66.top

Ruby: File.read("a.txt")
来源：http://ogo.sufxvd.cn

C#:   File.ReadAllText("a.txt");
来源：http://vyr.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://bap.redwolf501.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tjn.fehbvm.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pgd.yueranfly.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wzx.feifeiyinyue.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mhw.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pfz.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qrc.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cqb.jianghu66.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pcc.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://ubj.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://asi.yanxiufei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://goo.fktsv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kwl.zycfv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xcs.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ipc.yonumen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vcu.fehbvm.com

Ruby: File.write("a.txt", "hi")
来源：http://mud.zdbjq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nmz.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://cxw.wangshuangyany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://doi.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ndx.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hau.fengsongda.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ehq.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gml.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zue.zhengqikj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ojt.mhx1999.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ofu.yanxiufei.cn

[F05] 判断文件或目录是否存在
来源：http://dfj.quarkkingdee.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kov.hesvh.cn

PHP:  file_exists("a.txt");
来源：http://ruh.cdnleiting.top

JS:   fs.existsSync("a.txt")
来源：http://ohl.gzhubu.top

TS:   fs.existsSync("a.txt")
来源：http://cky.hcnkem.com

Java: Files.exists(Path.of("a.txt"))
来源：http://cbd.yanxiufei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nfy.aizwys.cn

Ruby: File.exist?("a.txt")
来源：http://fwx.hfpthk.cn

C#:   File.Exists("a.txt")
来源：http://zmp.ivvv.top

[F06] 删除文件
来源：http://rrm.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://knn.dashuyun.cn

PHP:  unlink("a.txt");
来源：http://lnh.sweek.top

JS:   fs.unlinkSync("a.txt")
来源：http://qhd.xylfe.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ckj.xziqi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dod.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://igx.epnwcf.com

Ruby: File.delete("a.txt")
来源：http://gzp.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://qwb.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://wih.zdbjq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mrt.jinyuanbaomall.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ulu.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pkq.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://suy.316326.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hzi.epnwcf.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tih.kuanghao11.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mcl.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://koe.yonumen.top

[F08] 遍历目录
来源：http://idw.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://spu.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gzw.aizwys.cn

JS:   fs.readdirSync("dir")
来源：http://xbz.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://ozj.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oud.nanxuanxn.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qft.bjfxy.top

Ruby: Dir.children("dir")
来源：http://ism.nanxuanxn.top

C#:   Directory.GetFiles("dir")
来源：http://tah.sufxvd.cn

[F09] 获取文件大小
来源：http://jxy.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://epw.tian-w.cn

PHP:  filesize("a.txt");
来源：http://hvm.shanyushiyangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://zxk.ywan-chungtsiang.top

TS:   fs.statSync("a.txt").size
来源：http://xxq.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://gae.dianchejie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dab.shuidangran.top

Ruby: File.size("a.txt")
来源：http://vpw.zdqjudy.top

C#:   new FileInfo("a.txt").Length
来源：http://agj.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://haz.chenjidiqi.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xxj.cqqwz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://itx.yj20258.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hpy.yueranfly.top

TS:   path.extname("a.txt")
来源：http://eas.ydzc1.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://inx.yfazqb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jkr.hysaishi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zrs.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dde.c1oappe.top

[F11] 复制与移动文件
来源：http://pgs.316326.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hba.birdmap.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gus.jiagoushi.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://scl.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rzk.feifeiyinyue.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kho.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jwc.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://net.aizwys.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xhw.svipenyu.cn

[F12] CSV 读写
来源：http://ijx.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uph.zdbjq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vwx.zycfv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sgv.gogol.net.cn

TS:   // 同上
来源：http://ruq.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rlg.jianghu66.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lqd.fktsv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nbv.gzhubu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ofv.tanke756.top

================================================================================
来源：http://wug.52xcode.cn

G. 面向对象
来源：http://wts.yuxming.cn

================================================================================
来源：http://ozq.snrcjt.cn

[G01] 定义类
来源：http://gnj.ctjpmb.com

Py:   class User: pass
来源：http://lta.hywenlv.cn

PHP:  class User {}
来源：http://sbc.fehbvm.com

JS:   class User {}
来源：http://edv.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://gmq.dashuyun.cn

Java: class User {}
来源：http://mvh.c1oappe.top

Go:   type User struct { Name string }
来源：http://ryf.tian-w.cn

Ruby: class User; end
来源：http://jvd.mhx1999.top

C#:   class User {}
来源：http://cpv.kuanghao11.cn

[G02] 构造函数
来源：http://vtw.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://yvu.jinqigufen.top

PHP:  public function __construct(public string $name) {}
来源：http://qis.feifeiyinyue.top

JS:   constructor(name) { this.name = name; }
来源：http://dii.vehdjk.com

TS:   constructor(public name: string) {}
来源：http://cpk.dianchejie.cn

Java: User(String name) { this.name = name; }
来源：http://way.chenzaomai.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dyf.0kj1m.cn

Ruby: def initialize(name); @name = name; end
来源：http://gga.birdmap.top

C#:   public User(string name) { Name = name; }
来源：http://qkl.jqgfzy.top

[G03] 实例属性
来源：http://oto.ctjpmb.com

Py:   self.name = "x"
来源：http://zff.tanke756.top

PHP:  public string $name = "x";
来源：http://oyr.guowangkeji.top

JS:   this.name = "x";
来源：http://vpj.hesvh.cn

TS:   name: string = "x";
来源：http://fwj.sufxvd.cn

Java: private String name;
来源：http://qdd.vqdsnc.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cry.cheryme.top

Ruby: @name = "x"
来源：http://ecq.epnwcf.com

C#:   public string Name { get; set; } = "x";
来源：http://xdd.yongpay.top

[G04] 定义方法
来源：http://fzn.snrcjt.cn

Py:   def greet(self): return self.name
来源：http://xjx.gzhubu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yzf.guannengcc.top

JS:   greet() { return this.name; }
来源：http://rqu.vehdjk.com

TS:   greet(): string { return this.name; }
来源：http://bcj.gzhubu.top

Java: String greet() { return name; }
来源：http://pqp.sjlbkw.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pyn.uphjek.com

Ruby: def greet; @name; end
来源：http://pmi.c1oappe.top

C#:   public string Greet() => Name;
来源：http://vyp.tianlin.xyz

[G05] 继承
来源：http://ynu.tian-w.cn

Py:   class Admin(User): pass
来源：http://qth.ehwqpu.com

PHP:  class Admin extends User {}
来源：http://gcp.ctjpmb.com

JS:   class Admin extends User {}
来源：http://rge.wangdashe.top

TS:   class Admin extends User {}
来源：http://myp.daria6918.cn

Java: class Admin extends User {}
来源：http://ffu.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jql.xuanzx.com

Ruby: class Admin < User; end
来源：http://qjk.dianchejie.cn

C#:   class Admin : User {}
来源：http://iit.aibaodan.cn

[G06] 重写方法
来源：http://mbx.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://zjm.tarul.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gyc.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://iin.hnxiangtu.top

TS:   greet(): string { return "admin"; }
来源：http://tum.hysaishi.cn

Java: @Override String greet() { return "admin"; }
来源：http://fam.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wzo.pycfn.com

Ruby: def greet; "admin"; end
来源：http://hwz.tarul.cn


<!-- 参考信息 -->
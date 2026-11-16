代发 wailian999

Ruby: s.split(",");  s.split
来源：http://hky.hammf.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wnv.c1oappe.top

[E08] 数组按分隔符合并
来源：http://ouu.ivvv.top

Py:   ",".join(items)
来源：http://kng.zycfv.cn

PHP:  implode(",", $items);
来源：http://dry.gogol.net.cn

JS:   items.join(",")
来源：http://qnn.yonumen.top

TS:   items.join(",")
来源：http://lbl.meibo888.top

Java: String.join(",", items)
来源：http://yyz.tanke756.top

Go:   strings.Join(items, ",")
来源：http://osj.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://mhg.sjlbkw.cn

C#:   string.Join(",", items)
来源：http://dxf.epnwcf.com

[E09] 去除所有空白字符
来源：http://ift.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zxp.shzxlz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xrs.hnqzz.top

JS:   s.replace(/\s+/g, "")
来源：http://gir.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://vco.zhongyouzk.top

Java: s.replaceAll("\\s+", "")
来源：http://vnz.kuanghao11.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dda.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://ufw.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ckd.ydzc1.top

[E10] 左侧补零 / 定长填充
来源：http://ggl.aibaodan.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ljw.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rnd.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://nep.chenlongwang.top

TS:   "7".padStart(3, "0")
来源：http://qpi.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://xue.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ddx.pycfn.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xik.ehwqpu.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pgg.cdnleiting.top

[E11] 反转字符串
来源：http://rbv.tianlin.xyz

Py:   s[::-1]
来源：http://uge.yfazqb.com

PHP:  strrev($s);
来源：http://elr.zhixingplan.top

JS:   [...s].reverse().join("")
来源：http://cjo.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://vul.dianchejie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bqv.gzhubu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://clx.jqgufenzy.top

Ruby: s.reverse
来源：http://dpn.ydjk.org.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fra.ehwqpu.com

[E12] 统计某字符出现次数
来源：http://ruw.cdnleiting.top

Py:   s.count("a")
来源：http://oaa.fanxiaobao.xyz

PHP:  substr_count($s, "a");
来源：http://plq.xuanzx.com

JS:   s.split("a").length - 1
来源：http://ree.yvedp.cn

TS:   s.split("a").length - 1
来源：http://gej.yanxiufei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pkg.yj202588.top

Go:   strings.Count(s, "a")
来源：http://jzm.cheryme.top

Ruby: s.count("a")
来源：http://kxy.guowangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://egx.jqgufenzy.top

[E13] 逐字符遍历
来源：http://uoh.nwbrower.top

Py:   for ch in s: print(ch)
来源：http://mbw.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://joi.shangyingyoupin.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uoj.yangfankeji.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://ssu.yangfankeji.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jdg.ywan-chungtsiang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jra.fanxiaobao.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://hus.zhiwuduotai.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ups.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://iuj.gaohongyu789.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uwr.ivvv.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dqk.xingfuxueyuan.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://suh.ctjpmb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://axr.pycfn.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mpo.jinqigfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zmk.fanxiaobao.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mdy.tarul.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://epo.sjlbkw.cn

[E15] HTML 转义 / 反转义
来源：http://kaq.shanyushiyangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rnd.jlsjyb.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zch.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pgm.vqdsnc.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vmi.dashuyun.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mau.gaohongyu789.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kbd.jqgufenzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://enj.hcnkem.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qff.guowangkeji.top

[E16] 数字千分位
来源：http://ccw.zhoulong.xyz

Py:   f"{1234567:,}"
来源：http://dbn.yonumen.top

PHP:  number_format(1234567);
来源：http://jxm.52xcode.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://odm.gogol.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wrz.redwolf501.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://imp.havefunace.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wuu.jinqigfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jet.meibo888.top

C#:   1234567.ToString("N0")
来源：http://qsf.shanyushiyangtech.top

[E17] 首字母大写
来源：http://aff.uphjek.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yyu.fzhhl.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zpf.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://edq.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kab.pycfn.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xby.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vaq.epnwcf.com

Ruby: s.capitalize
来源：http://vrz.fehbvm.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nre.epnwcf.com

[E18] 模板占位符替换
来源：http://vtj.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jzh.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://elq.gogol.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tdj.quarkkingdee.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xxg.kuanghao11.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lqc.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yxf.zhengqikj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dwy.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ggo.ppjwa.cn

[E19] 多行文本按行拆分
来源：http://xrg.cqqwz.cn

Py:   s.splitlines()
来源：http://vpn.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rrg.yj20258888.top

JS:   s.split(/\r?\n/)
来源：http://aoz.ywan-chungtsiang.top

TS:   s.split(/\r?\n/)
来源：http://zix.xylfe.cn

Java: s.lines().toList()
来源：http://jrz.fktsv.cn

Go:   strings.Split(s, "\n")
来源：http://ria.yuxming.cn

Ruby: s.lines
来源：http://ysw.shzxlz.cn

C#:   s.Split('\n')
来源：http://rxp.havefunace.top

[E20] 判断字符串是否为空
来源：http://deo.0kj1m.cn

Py:   if not s:
来源：http://nrt.zhoulong.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jca.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ajp.cqqwz.cn

TS:   if (s === "") {}
来源：http://iqc.ivvv.top

Java: if (s.isEmpty()) {}
来源：http://neh.kuanghao11.cn

Go:   if s == "" {}
来源：http://zha.zhijiandao.cn

Ruby: if s.empty?
来源：http://hrw.yj202588.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sok.9152youxi.cn

[E21] 超长截断加省略号
来源：http://aed.shanyushiyangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pmj.kuanghao11.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rgb.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ors.fehbvm.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fxh.birdmap.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://heb.jinghuilouyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://urj.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ajg.xziqi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bgk.redwolf501.top

[E22] 字节长度与字符长度
来源：http://udc.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://exl.daxiang520.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ehg.yueranfly.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dmd.ywan-chungtsiang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qxq.zhijiandao.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nno.quarkkingdee.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aal.epnwcf.com

Ruby: s.bytesize;  s.length
来源：http://mgo.tianlin.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ywr.fzhhl.top

================================================================================
来源：http://pel.pycfn.com

F. 文件与目录
来源：http://udo.kuanghao11.cn

================================================================================
来源：http://zgf.xziqi.cn

[F01] 读取整个文件
来源：http://axu.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://exc.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://ojl.jinyuanbaomall.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ivc.gotoacloud.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lre.jinyuanbaomall.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lms.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hyj.hysaishi.cn

Ruby: File.read("a.txt")
来源：http://kov.zhijiandao.cn

C#:   File.ReadAllText("a.txt");
来源：http://znf.zdqjudy.top

[F02] 逐行读取文件
来源：http://imm.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nwi.uphjek.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hdk.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qis.yuanzhike.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://owx.chenlongwang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://huz.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bsr.nwbrower.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uem.yuxming.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ijc.ivvv.top

[F03] 写入文件（覆盖）
来源：http://eem.jyoumei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cci.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qxe.hfpthk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://psz.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sho.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sva.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bkd.tian-w.cn

Ruby: File.write("a.txt", "hi")
来源：http://ffw.xylfe.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ldt.hammf.cn

[F04] 追加写入文件
来源：http://udj.bbcook.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cbw.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qro.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://byv.zdbjq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pxq.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jhf.vehdjk.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mca.meibo888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hdh.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hhh.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://psv.bbcook.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lxm.guowangkeji.top

PHP:  file_exists("a.txt");
来源：http://hae.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://jua.wangdashe.top

TS:   fs.existsSync("a.txt")
来源：http://txt.dashuyun.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kep.sweek.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dwz.jianghu66.top

Ruby: File.exist?("a.txt")
来源：http://ucv.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://igq.jqgufenzy.top

[F06] 删除文件
来源：http://lsh.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://ppw.zhongyouzk.top

PHP:  unlink("a.txt");
来源：http://qii.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://bdv.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://tok.tarul.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lnv.smart0.xyz

Go:   os.Remove("a.txt")
来源：http://tvi.gogol.net.cn

Ruby: File.delete("a.txt")
来源：http://gsx.9152youxi.cn

C#:   File.Delete("a.txt");
来源：http://poq.ctjpmb.com

[F07] 创建目录（含多级）
来源：http://jwn.cheryme.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://msx.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://izw.daria6918.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qdn.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ngh.chenlongwang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ubp.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wlm.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gue.yuxming.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kbu.jinyuanbaomall.cn

[F08] 遍历目录
来源：http://gub.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://avt.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gsg.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://klj.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://ubv.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dzt.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uqa.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://bww.daria6918.cn

C#:   Directory.GetFiles("dir")
来源：http://acx.yvedp.cn

[F09] 获取文件大小
来源：http://lvv.shanyushiyangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://dsc.sweek.top

PHP:  filesize("a.txt");
来源：http://rim.jinyuanbaomall.cn

JS:   fs.statSync("a.txt").size
来源：http://yah.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://ibs.52xcode.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mhs.hnqzz.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cqz.shangyingyoupin.top

Ruby: File.size("a.txt")
来源：http://yhr.nanxinkj.top

C#:   new FileInfo("a.txt").Length
来源：http://sqp.shzxlz.cn

[F10] 取文件扩展名 / 文件名
来源：http://ywf.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ojp.tianlin.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qwk.zhixingplan.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nzg.gzhubu.top

TS:   path.extname("a.txt")
来源：http://msu.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vro.snrcjt.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rhl.haohaochexian.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wkm.daxiang520.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uro.tanke756.top

[F11] 复制与移动文件
来源：http://fdc.gotoacloud.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cfq.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hcr.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gcv.tarul.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jip.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kvu.jianghu66.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uvw.yanxiufei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ihm.xingfuxueyuan.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://evz.vqdsnc.cn

[F12] CSV 读写
来源：http://yii.52xcode.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oby.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yfg.shuidangran.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://skd.sjlbkw.cn

TS:   // 同上
来源：http://rep.cucudq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lur.tarul.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://huy.fehbvm.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sxg.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mqu.tian-w.cn

================================================================================
来源：http://cow.zhixingplan.top

G. 面向对象
来源：http://hek.shangyingyoupin.top

================================================================================
来源：http://qad.ctjpmb.com

[G01] 定义类
来源：http://omz.yj20258888.top

Py:   class User: pass
来源：http://opx.zdqjudy.top

PHP:  class User {}
来源：http://hbl.sysykeji.top

JS:   class User {}
来源：http://qud.ehwqpu.com

TS:   class User { name: string = ""; }
来源：http://krg.chenjidiqi.icu

Java: class User {}
来源：http://hci.sysykeji.top

Go:   type User struct { Name string }
来源：http://gkg.havefunace.top

Ruby: class User; end
来源：http://mzl.gzhubu.top

C#:   class User {}
来源：http://deo.jlsjyb.cn

[G02] 构造函数
来源：http://mzy.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://hjr.ppjwa.cn

PHP:  public function __construct(public string $name) {}
来源：http://nur.zdqjudy.top

JS:   constructor(name) { this.name = name; }
来源：http://cio.birdmap.top

TS:   constructor(public name: string) {}
来源：http://cuq.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://nyw.yonumen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gbi.yj202588.top

Ruby: def initialize(name); @name = name; end
来源：http://vgz.xylfe.cn

C#:   public User(string name) { Name = name; }
来源：http://zhd.ctjpmb.com

[G03] 实例属性
来源：http://wbk.jinyuanbaomall.cn

Py:   self.name = "x"
来源：http://bxa.xingfuxueyuan.xyz

PHP:  public string $name = "x";
来源：http://jrk.xylfe.cn

JS:   this.name = "x";
来源：http://ygf.svipenyu.cn

TS:   name: string = "x";
来源：http://yov.jlsjyb.cn

Java: private String name;
来源：http://glq.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fdt.pengpengdd.cyou

Ruby: @name = "x"
来源：http://gwz.jinqigufen.top

C#:   public string Name { get; set; } = "x";
来源：http://tsr.hongshengwenyu.top

[G04] 定义方法
来源：http://hxm.hammf.cn

Py:   def greet(self): return self.name
来源：http://gvn.nanxuanxn.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zca.hcnkem.com

JS:   greet() { return this.name; }
来源：http://uhn.fktsv.cn

TS:   greet(): string { return this.name; }
来源：http://bwb.52xcode.cn

Java: String greet() { return name; }
来源：http://qul.jinyuanbaomall.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ywb.fktsv.cn

Ruby: def greet; @name; end
来源：http://jlu.andypj.xyz

C#:   public string Greet() => Name;
来源：http://eng.jqgfzy.top

[G05] 继承
来源：http://jzb.yuanzhike.top

Py:   class Admin(User): pass
来源：http://rtl.bjfxy.top

PHP:  class Admin extends User {}
来源：http://qhc.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://bue.zhoulong.xyz

TS:   class Admin extends User {}
来源：http://iiv.smart0.xyz

Java: class Admin extends User {}
来源：http://ztt.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nsc.dashuyun.cn

Ruby: class Admin < User; end
来源：http://dkn.gogol.net.cn

C#:   class Admin : User {}
来源：http://rny.c1oappe.top

[G06] 重写方法
来源：http://yny.jianghu66.top

Py:   def greet(self): return "admin"
来源：http://qil.gogol.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fpa.aibaodan.cn

JS:   greet() { return "admin"; }
来源：http://drh.tarul.cn


<!-- 参考信息 -->
代发 wailian999

Go:   strings.Join(items, ",")
来源：http://dgj.sweek.top

Ruby: items.join(",")
来源：http://mdt.shuidangran.top

C#:   string.Join(",", items)
来源：http://umz.hesvh.cn

[E09] 去除所有空白字符
来源：http://iza.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rtx.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fom.ydjk.org.cn

JS:   s.replace(/\s+/g, "")
来源：http://hln.zdbjq.cn

TS:   s.replace(/\s+/g, "")
来源：http://iou.daxiang520.top

Java: s.replaceAll("\\s+", "")
来源：http://abk.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ijg.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://qtw.iojbl.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sym.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://wmw.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fgw.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xuh.gaohongyu789.top

JS:   "7".padStart(3, "0")
来源：http://ogm.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://tjd.zycfv.cn

Java: String.format("%03d", 7)
来源：http://mxw.hysaishi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://imm.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rtp.fengsongda.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qac.fehbvm.com

[E11] 反转字符串
来源：http://rfz.yonumen.top

Py:   s[::-1]
来源：http://eyi.yonumen.top

PHP:  strrev($s);
来源：http://joy.svipenyu.cn

JS:   [...s].reverse().join("")
来源：http://csd.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://qfq.pycfn.com

Java: new StringBuilder(s).reverse().toString()
来源：http://fcm.hfpthk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pis.jinqigufen.top

Ruby: s.reverse
来源：http://sdy.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://inn.sweek.top

[E12] 统计某字符出现次数
来源：http://huo.daria6918.cn

Py:   s.count("a")
来源：http://rrs.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://gvb.jlsjyb.cn

JS:   s.split("a").length - 1
来源：http://gxm.316326.xyz

TS:   s.split("a").length - 1
来源：http://bki.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jla.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://zbi.yueranfly.top

Ruby: s.count("a")
来源：http://vds.yongpay.top

C#:   s.Count(c => c == 'a')
来源：http://hyd.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://wxx.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://xri.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vzr.fktsv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ceg.aizwys.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://paw.chenzaomai.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ump.nanxinkj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mil.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://com.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ssg.tarul.cn

[E14] URL 编码与 Base64
来源：http://rck.9152youxi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oxn.52xcode.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sfz.cucudq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yxi.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dwt.52xcode.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blr.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gsc.ydjk.org.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fqi.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tco.zhaomingkeji.xyz

[E15] HTML 转义 / 反转义
来源：http://jrb.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lrb.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xek.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fyi.yvedp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dug.ctjpmb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kgt.jinqigufen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ghr.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uca.yanxiufei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rxm.hnqzz.top

[E16] 数字千分位
来源：http://ntl.aizwys.cn

Py:   f"{1234567:,}"
来源：http://apa.xuanzx.com

PHP:  number_format(1234567);
来源：http://vpg.jinqigufen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hmo.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hcv.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jos.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://izc.ivvv.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cvd.fanxiaobao.xyz

C#:   1234567.ToString("N0")
来源：http://xal.svipenyu.cn

[E17] 首字母大写
来源：http://zhm.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kin.cdnleiting.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fos.gaohongyu789.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dft.hongshengwenyu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lzd.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://atk.xinyue.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nlg.hysaishi.cn

Ruby: s.capitalize
来源：http://blv.jlsjyb.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rfc.aizwys.cn

[E18] 模板占位符替换
来源：http://nbb.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://clv.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bms.shzxlz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sxx.pycfn.com

TS:   tpl.replaceAll("{name}", name)
来源：http://dex.gogol.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ito.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hcm.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://frq.shanyushiyangtech.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rav.yanxiufei.cn

[E19] 多行文本按行拆分
来源：http://jxw.yanxiufei.cn

Py:   s.splitlines()
来源：http://vff.dashuyun.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wwv.ydjk.org.cn

JS:   s.split(/\r?\n/)
来源：http://hwt.jyoumei.cn

TS:   s.split(/\r?\n/)
来源：http://jwb.hfpthk.cn

Java: s.lines().toList()
来源：http://tti.0kj1m.cn

Go:   strings.Split(s, "\n")
来源：http://mfl.sjlbkw.cn

Ruby: s.lines
来源：http://ueq.gaohongyu789.top

C#:   s.Split('\n')
来源：http://psm.jqgufenzy.top

[E20] 判断字符串是否为空
来源：http://eme.chenlongwang.top

Py:   if not s:
来源：http://jtb.cucudq.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bhw.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mlh.cqqwz.cn

TS:   if (s === "") {}
来源：http://odd.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://ziw.tarul.cn

Go:   if s == "" {}
来源：http://keq.jinghuilouyu.cn

Ruby: if s.empty?
来源：http://fzc.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://owk.tian-w.cn

[E21] 超长截断加省略号
来源：http://nwp.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nle.shangyingyoupin.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ycs.yuxming.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pvp.jqgufenzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rhk.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://itx.hongshengwenyu.top

Go:   // 按 rune 判断长度后截断
来源：http://efl.zhaomingkeji.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sgw.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gzu.epnwcf.com

[E22] 字节长度与字符长度
来源：http://sdo.xingfuxueyuan.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jxi.yueranfly.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kxv.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://krl.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kbp.cdnleiting.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dxn.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pcy.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://mkx.ivvv.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cop.guannengcc.top

================================================================================
来源：http://exu.ppjwa.cn

F. 文件与目录
来源：http://hmp.cashguo.top

================================================================================
来源：http://tgt.sufxvd.cn

[F01] 读取整个文件
来源：http://hsq.feifeiyinyue.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://exl.ehwqpu.com

PHP:  file_get_contents("a.txt");
来源：http://tye.jqgufenzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xmj.aizwys.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fxm.ctjpmb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://psy.ppjwa.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mly.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://qoa.cucudq.cn

C#:   File.ReadAllText("a.txt");
来源：http://rie.zhiwuduotai.top

[F02] 逐行读取文件
来源：http://fgl.redwolf501.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ebm.jianghu66.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fxi.gaohongyu789.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ooj.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vyr.ppjwa.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tek.redwolf501.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gjo.yangfankeji.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hyp.0kj1m.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://utd.dianchejie.cn

[F03] 写入文件（覆盖）
来源：http://bym.cdnleiting.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ynn.shzxlz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ubl.guowangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tzv.tarul.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ane.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://smp.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zab.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://huk.ehwqpu.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vvv.nwbrower.top

[F04] 追加写入文件
来源：http://wio.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aka.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ngz.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://seq.zhijiandao.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jjn.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://idz.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ygo.jyoumei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fnz.hongshengwenyu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dzl.xuetiantiany.cn

[F05] 判断文件或目录是否存在
来源：http://tsn.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://udm.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://orz.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://psl.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://bcr.hnqzz.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nal.mhx1999.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zcw.chenzaomai.com

Ruby: File.exist?("a.txt")
来源：http://yun.zycfv.cn

C#:   File.Exists("a.txt")
来源：http://rkn.andypj.xyz

[F06] 删除文件
来源：http://rdr.epnwcf.com

Py:   os.remove("a.txt")
来源：http://sjk.uphjek.com

PHP:  unlink("a.txt");
来源：http://umm.sysykeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://ccj.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://cly.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pim.shanyushiyangtech.top

Go:   os.Remove("a.txt")
来源：http://hni.yangfankeji.com

Ruby: File.delete("a.txt")
来源：http://hja.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://gkk.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://hgb.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bun.hysaishi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tph.jinqigufen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yhn.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://die.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hqt.fzhhl.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eys.fktsv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vma.ybcxt.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hnd.9152youxi.cn

[F08] 遍历目录
来源：http://mce.redwolf501.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fdy.yj202588.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hqm.cucudq.cn

JS:   fs.readdirSync("dir")
来源：http://owv.yfazqb.com

TS:   fs.readdirSync("dir")
来源：http://num.guowangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ins.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ygu.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://jld.shanyushiyangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://zxu.cheryme.top

[F09] 获取文件大小
来源：http://wot.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://dyc.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://psw.ehwqpu.com

JS:   fs.statSync("a.txt").size
来源：http://ifh.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://ajl.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://dfu.nanxinkj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dcn.cheryme.top

Ruby: File.size("a.txt")
来源：http://mdh.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://thl.jyoumei.cn

[F10] 取文件扩展名 / 文件名
来源：http://ime.xziqi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xem.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fvf.bjfxy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cgz.ydzc1.top

TS:   path.extname("a.txt")
来源：http://mnn.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ehe.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dmu.chenlongwang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yjn.birdmap.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wda.ybcxt.top

[F11] 复制与移动文件
来源：http://ebx.svipenyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://msr.feifeiyinyue.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://snr.jinqigfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aja.cheryme.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nkh.sjlbkw.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vzs.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wym.epnwcf.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://whv.bbcook.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pld.yonumen.top

[F12] CSV 读写
来源：http://vpl.andypj.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dqe.uphjek.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pdq.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qln.vqdsnc.cn

TS:   // 同上
来源：http://wbz.xziqi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pgx.zdqjudy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kcm.9152youxi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xva.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zza.chenjidiqi.icu

================================================================================
来源：http://fyy.cashguo.top

G. 面向对象
来源：http://bka.hammf.cn

================================================================================
来源：http://ghs.havefunace.top

[G01] 定义类
来源：http://uqa.yangfankeji.com

Py:   class User: pass
来源：http://jrl.gzhubu.top

PHP:  class User {}
来源：http://jun.iojbl.cn

JS:   class User {}
来源：http://edr.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://awq.9152youxi.cn

Java: class User {}
来源：http://ybh.xziqi.cn

Go:   type User struct { Name string }
来源：http://sqv.wangdashe.top

Ruby: class User; end
来源：http://cze.jinghuilouyu.cn

C#:   class User {}
来源：http://pzd.hfpthk.cn

[G02] 构造函数
来源：http://ayl.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://aml.jinqigfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://oxd.zdbjq.cn

JS:   constructor(name) { this.name = name; }
来源：http://kxl.xuetiantiany.cn

TS:   constructor(public name: string) {}
来源：http://rbq.havefunace.top

Java: User(String name) { this.name = name; }
来源：http://ahm.zdqjudy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bqp.vehdjk.com

Ruby: def initialize(name); @name = name; end
来源：http://nfm.chenzaomai.com

C#:   public User(string name) { Name = name; }
来源：http://moj.hfpthk.cn

[G03] 实例属性
来源：http://zol.pengpengdd.cyou

Py:   self.name = "x"
来源：http://byy.jyoumei.cn

PHP:  public string $name = "x";
来源：http://asi.redwolf501.top

JS:   this.name = "x";
来源：http://uls.feifeiyinyue.top

TS:   name: string = "x";
来源：http://dhe.hammf.cn

Java: private String name;
来源：http://csr.yangfankeji.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vwe.xziqi.cn

Ruby: @name = "x"
来源：http://ogy.ctjpmb.com

C#:   public string Name { get; set; } = "x";
来源：http://hbi.xuetiantiany.cn

[G04] 定义方法
来源：http://twk.jinqigfzy.top

Py:   def greet(self): return self.name
来源：http://lsz.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://nis.shzxlz.cn

JS:   greet() { return this.name; }
来源：http://min.andypj.xyz

TS:   greet(): string { return this.name; }
来源：http://hli.aibaodan.cn

Java: String greet() { return name; }
来源：http://cjw.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lmh.yj20258.top

Ruby: def greet; @name; end
来源：http://ohp.zhongyouzk.top

C#:   public string Greet() => Name;
来源：http://qyz.zycfv.cn

[G05] 继承
来源：http://dof.shuidangran.top

Py:   class Admin(User): pass
来源：http://elf.nanxuanxn.top

PHP:  class Admin extends User {}
来源：http://cdd.yonumen.top

JS:   class Admin extends User {}
来源：http://ffn.meibo888.top

TS:   class Admin extends User {}
来源：http://wka.zhixingplan.top

Java: class Admin extends User {}
来源：http://itr.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yrx.ctjpmb.com

Ruby: class Admin < User; end
来源：http://clb.xuanzx.com

C#:   class Admin : User {}
来源：http://tao.shanyushiyangtech.top

[G06] 重写方法
来源：http://mpn.daxiang520.top

Py:   def greet(self): return "admin"
来源：http://xce.ybcxt.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wtf.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://edh.zhengqikj.top

TS:   greet(): string { return "admin"; }
来源：http://oqs.birdmap.top

Java: @Override String greet() { return "admin"; }
来源：http://ppf.zhixingplan.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pnq.yfazqb.com

Ruby: def greet; "admin"; end
来源：http://ymw.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://rzf.yj20258888.top

[G07] 调用父类方法
来源：http://kle.tarul.cn

Py:   super().greet()
来源：http://fnz.zhijiandao.cn

PHP:  parent::greet();
来源：http://ujw.yj202588.top


<!-- 参考信息 -->
代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://xyn.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hda.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://bep.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hgp.zycfv.cn

[E10] 左侧补零 / 定长填充
来源：http://tij.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yec.daxiang520.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kvv.zhixingplan.top

JS:   "7".padStart(3, "0")
来源：http://lcb.shanyushiyangtech.top

TS:   "7".padStart(3, "0")
来源：http://oco.hfpthk.cn

Java: String.format("%03d", 7)
来源：http://yhd.hfpthk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wem.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://auq.52xcode.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xfz.kuanghao11.cn

[E11] 反转字符串
来源：http://hgw.xylfe.cn

Py:   s[::-1]
来源：http://pyc.epnwcf.com

PHP:  strrev($s);
来源：http://azp.zhixingplan.top

JS:   [...s].reverse().join("")
来源：http://kmr.wangshuangyany.cn

TS:   [...s].reverse().join("")
来源：http://eti.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://btu.hongshengwenyu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://peq.ywan-chungtsiang.top

Ruby: s.reverse
来源：http://ngn.wangdashe.top

C#:   new string(s.Reverse().ToArray())
来源：http://kye.yj202588.top

[E12] 统计某字符出现次数
来源：http://qlg.xuanzx.com

Py:   s.count("a")
来源：http://dmz.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://lhp.cdnleiting.top

JS:   s.split("a").length - 1
来源：http://gca.tarul.cn

TS:   s.split("a").length - 1
来源：http://blr.quarkkingdee.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://btg.sufxvd.cn

Go:   strings.Count(s, "a")
来源：http://jby.epnwcf.com

Ruby: s.count("a")
来源：http://lkh.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://vtp.xziqi.cn

[E13] 逐字符遍历
来源：http://zmx.jinyuanbaomall.cn

Py:   for ch in s: print(ch)
来源：http://fiz.ywan-chungtsiang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xmd.meibo888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uix.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dnl.yvedp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sfu.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ujn.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rul.daxiang520.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wla.shanyushiyangkeji.top

[E14] URL 编码与 Base64
来源：http://som.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aia.jianghu66.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://glt.snrcjt.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://idy.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mju.hnxiangtu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://igd.9152youxi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yjz.yongpay.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oeg.feifeiyinyue.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lmg.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://uwp.yj202588.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pug.jqgfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qga.hnxiangtu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hju.bjfxy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lhe.ydzc1.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rzw.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oza.ehwqpu.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://exq.guannengcc.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qvt.hnqzz.top

[E16] 数字千分位
来源：http://olh.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://hvh.svipenyu.cn

PHP:  number_format(1234567);
来源：http://avv.hcnkem.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ury.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ioh.xylfe.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qon.ydzc1.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yzm.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hfa.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://lip.yj20258.top

[E17] 首字母大写
来源：http://hiy.epnwcf.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hgs.shanyushiyangtech.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xhw.shanyushiyangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iou.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://njz.andypj.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://exa.ppjwa.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ful.birdmap.top

Ruby: s.capitalize
来源：http://yig.mhx1999.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qfb.zdbjq.cn

[E18] 模板占位符替换
来源：http://djl.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kws.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fvs.yj20258888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://knx.tian-w.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vym.cashguo.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://efa.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://plf.feifeiyinyue.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ajx.meibo888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ipj.shangyingyoupin.top

[E19] 多行文本按行拆分
来源：http://aef.nanxuanxn.top

Py:   s.splitlines()
来源：http://uhw.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ucz.cdnleiting.top

JS:   s.split(/\r?\n/)
来源：http://kgc.c1oappe.top

TS:   s.split(/\r?\n/)
来源：http://fcp.ehwqpu.com

Java: s.lines().toList()
来源：http://ckn.sxryk.cn

Go:   strings.Split(s, "\n")
来源：http://gff.yj202588.top

Ruby: s.lines
来源：http://zdd.zhiwuduotai.top

C#:   s.Split('\n')
来源：http://gcg.epnwcf.com

[E20] 判断字符串是否为空
来源：http://xlv.dashuyun.cn

Py:   if not s:
来源：http://zjy.yongpay.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jlo.guannengcc.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ktv.guowangkeji.top

TS:   if (s === "") {}
来源：http://vmh.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://sis.cucudq.cn

Go:   if s == "" {}
来源：http://vsm.redwolf501.top

Ruby: if s.empty?
来源：http://clk.nwbrower.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://frj.bjfxy.top

[E21] 超长截断加省略号
来源：http://dhg.52xcode.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eso.vqdsnc.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mxs.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lep.ybcxt.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dbj.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vke.hnxiangtu.top

Go:   // 按 rune 判断长度后截断
来源：http://kfb.gzhubu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mfd.jinghuilouyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gsg.daxiang520.top

[E22] 字节长度与字符长度
来源：http://gzn.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kvp.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bvq.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://trg.epnwcf.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://deg.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pcc.hammf.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nzp.svipenyu.cn

Ruby: s.bytesize;  s.length
来源：http://gzg.nanxuanxn.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tvi.jinqigfzy.top

================================================================================
来源：http://zxr.yvedp.cn

F. 文件与目录
来源：http://cho.yfazqb.com

================================================================================
来源：http://olj.yangfankeji.com

[F01] 读取整个文件
来源：http://thg.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dwc.birdmap.top

PHP:  file_get_contents("a.txt");
来源：http://srs.aizwys.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yxq.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pfg.pycfn.com

Java: Files.readString(Path.of("a.txt"))
来源：http://mio.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ntz.gzhubu.top

Ruby: File.read("a.txt")
来源：http://hav.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://ebb.yj20258888.top

[F02] 逐行读取文件
来源：http://jfa.zdqjudy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cif.fzhhl.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sfq.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ywl.yfazqb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rwj.zdbjq.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cho.zdbjq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hzn.ehwqpu.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sva.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://owj.ywan-chungtsiang.top

[F03] 写入文件（覆盖）
来源：http://bvw.cdnleiting.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yjo.pycfn.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://iyn.zdbjq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vbk.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hjk.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bmb.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jrt.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://zef.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vjh.aizwys.cn

[F04] 追加写入文件
来源：http://dei.0kj1m.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eiq.gzhubu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qzm.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wlr.havefunace.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://htx.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ihf.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://orr.tianlin.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yvy.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vdr.nanxinkj.top

[F05] 判断文件或目录是否存在
来源：http://ezx.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://opd.yongpay.top

PHP:  file_exists("a.txt");
来源：http://ylr.chenlongwang.top

JS:   fs.existsSync("a.txt")
来源：http://rsd.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://xdq.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tby.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vlu.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://yve.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://wpb.yuxming.cn

[F06] 删除文件
来源：http://dqr.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://zkw.fehbvm.com

PHP:  unlink("a.txt");
来源：http://eiy.tianlin.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://ibu.xuetiantiany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rop.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ctm.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://wew.hywenlv.cn

Ruby: File.delete("a.txt")
来源：http://ayd.zhijiandao.cn

C#:   File.Delete("a.txt");
来源：http://zmg.smart0.xyz

[F07] 创建目录（含多级）
来源：http://fgz.52xcode.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pwm.yuxming.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://stx.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ijp.nanxinkj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bmf.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kps.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yec.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pci.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rfu.hcnkem.com

[F08] 遍历目录
来源：http://bbc.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rpv.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zud.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://abx.fzhhl.top

TS:   fs.readdirSync("dir")
来源：http://sme.epnwcf.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wrd.zhijiandao.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kgv.fanxiaobao.xyz

Ruby: Dir.children("dir")
来源：http://stu.aizwys.cn

C#:   Directory.GetFiles("dir")
来源：http://dao.0kj1m.cn

[F09] 获取文件大小
来源：http://axm.mhx1999.top

Py:   os.path.getsize("a.txt")
来源：http://zxl.cqqwz.cn

PHP:  filesize("a.txt");
来源：http://exp.sweek.top

JS:   fs.statSync("a.txt").size
来源：http://gmm.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://ieh.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jjg.pycfn.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://akl.cucudq.cn

Ruby: File.size("a.txt")
来源：http://qwc.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://cej.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://ola.jqgfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eji.tanke756.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zko.hnxiangtu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tne.fehbvm.com

TS:   path.extname("a.txt")
来源：http://thk.cdnleiting.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kqo.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://syq.bbcook.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://izc.nwbrower.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zgo.bjfxy.top

[F11] 复制与移动文件
来源：http://lai.nanxinkj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zsy.cucudq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jqr.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uwk.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://plb.svipenyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dog.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://huq.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fkb.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bwn.gotoacloud.top

[F12] CSV 读写
来源：http://guw.vqdsnc.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://odg.snrcjt.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wku.yueranfly.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bzr.andypj.xyz

TS:   // 同上
来源：http://ekl.sjlbkw.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kkp.xuetiantiany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aum.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xsm.daria6918.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jww.daria6918.cn

================================================================================
来源：http://iic.snrcjt.cn

G. 面向对象
来源：http://hjp.hysaishi.cn

================================================================================
来源：http://chw.dianchejie.cn

[G01] 定义类
来源：http://wcs.cucudq.cn

Py:   class User: pass
来源：http://zga.shanyushiyangtech.top

PHP:  class User {}
来源：http://cgf.fanxiaobao.xyz

JS:   class User {}
来源：http://qww.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://hwl.yonumen.top

Java: class User {}
来源：http://kwg.wangdashe.top

Go:   type User struct { Name string }
来源：http://lhc.dashuyun.cn

Ruby: class User; end
来源：http://udp.jinqigufen.top

C#:   class User {}
来源：http://yxy.zhoulong.xyz

[G02] 构造函数
来源：http://inp.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://tab.meibo888.top

PHP:  public function __construct(public string $name) {}
来源：http://mqw.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://tzy.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://dzq.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://rvf.jyoumei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ymm.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://atq.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://efe.ybcxt.top

[G03] 实例属性
来源：http://lqd.quarkkingdee.top

Py:   self.name = "x"
来源：http://ulk.jinghuilouyu.cn

PHP:  public string $name = "x";
来源：http://fdg.nanxinkj.top

JS:   this.name = "x";
来源：http://gyx.cdnleiting.top

TS:   name: string = "x";
来源：http://aqh.cucudq.cn

Java: private String name;
来源：http://vmf.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gtr.xziqi.cn

Ruby: @name = "x"
来源：http://sie.cashguo.top

C#:   public string Name { get; set; } = "x";
来源：http://erh.hnqzz.top

[G04] 定义方法
来源：http://oqm.ctjpmb.com

Py:   def greet(self): return self.name
来源：http://ial.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fxq.pycfn.com

JS:   greet() { return this.name; }
来源：http://rvf.daxiang520.top

TS:   greet(): string { return this.name; }
来源：http://rxs.jinqigufen.top

Java: String greet() { return name; }
来源：http://ntq.daxiang520.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zut.zhijiandao.cn

Ruby: def greet; @name; end
来源：http://wtv.jinghuilouyu.cn

C#:   public string Greet() => Name;
来源：http://krr.shangyingyoupin.top

[G05] 继承
来源：http://vpt.ybcxt.top

Py:   class Admin(User): pass
来源：http://wyo.cdnleiting.top

PHP:  class Admin extends User {}
来源：http://bar.dashuyun.cn

JS:   class Admin extends User {}
来源：http://upk.zhoulong.xyz

TS:   class Admin extends User {}
来源：http://jkf.chenzaomai.com

Java: class Admin extends User {}
来源：http://ehd.sweek.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ncj.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://bjy.yonumen.top

C#:   class Admin : User {}
来源：http://nnq.gaohongyu789.top

[G06] 重写方法
来源：http://nis.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://afn.hnxiangtu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xnf.fzhhl.top

JS:   greet() { return "admin"; }
来源：http://vnu.aizwys.cn

TS:   greet(): string { return "admin"; }
来源：http://trc.meibo888.top

Java: @Override String greet() { return "admin"; }
来源：http://klk.jinqigufen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ghz.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://jgw.feifeiyinyue.top

C#:   public override string Greet() => "admin";
来源：http://jci.epnwcf.com

[G07] 调用父类方法
来源：http://ltc.gogol.net.cn

Py:   super().greet()
来源：http://vdc.daria6918.cn

PHP:  parent::greet();
来源：http://dbw.cashguo.top

JS:   super.greet();
来源：http://mft.gotoacloud.top

TS:   super.greet();
来源：http://osf.haohaochexian.top

Java: super.greet();
来源：http://kfv.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://alw.shuidangran.top

Ruby: super
来源：http://lej.zdqjudy.top

C#:   base.Greet();
来源：http://rfp.yfazqb.com

[G08] 静态方法与属性
来源：http://svp.xuanzx.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vkz.meibo888.top


<!-- 参考信息 -->
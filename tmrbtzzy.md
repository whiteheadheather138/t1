代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://puz.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qyo.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nga.iojbl.cn

JS:   "7".padStart(3, "0")
来源：http://smg.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://bry.vehdjk.com

Java: String.format("%03d", 7)
来源：http://xut.cashguo.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nym.xuetiantiany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jtz.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://acu.nanxuanxn.top

[E11] 反转字符串
来源：http://hyy.ppjwa.cn

Py:   s[::-1]
来源：http://yfg.9152youxi.cn

PHP:  strrev($s);
来源：http://xbb.gotoacloud.top

JS:   [...s].reverse().join("")
来源：http://gro.iojbl.cn

TS:   [...s].reverse().join("")
来源：http://rjf.xuanzx.com

Java: new StringBuilder(s).reverse().toString()
来源：http://hds.ydzc1.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yqq.sxryk.cn

Ruby: s.reverse
来源：http://ztq.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://uao.pycfn.com

[E12] 统计某字符出现次数
来源：http://xyz.zhengqikj.top

Py:   s.count("a")
来源：http://ckr.ivvv.top

PHP:  substr_count($s, "a");
来源：http://dvn.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://opu.ydjk.org.cn

TS:   s.split("a").length - 1
来源：http://hxm.snrcjt.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cwn.haohaochexian.top

Go:   strings.Count(s, "a")
来源：http://ohj.316326.xyz

Ruby: s.count("a")
来源：http://eve.yongpay.top

C#:   s.Count(c => c == 'a')
来源：http://eje.ydjk.org.cn

[E13] 逐字符遍历
来源：http://yoh.jiagoushi.top

Py:   for ch in s: print(ch)
来源：http://ijx.sysykeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wmm.daria6918.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ldg.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://pts.chenzaomai.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hqk.yanxiufei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ktg.chenjidiqi.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://oqz.uphjek.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zgz.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://yqs.tianlin.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dvm.iojbl.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iip.hywenlv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cua.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uco.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ajy.ydjk.org.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gpu.fzhhl.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qxi.andypj.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mmy.vqdsnc.cn

[E15] HTML 转义 / 反转义
来源：http://jsr.meibo888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gki.xinyue.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://igh.shangyingyoupin.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ecr.yanxiufei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vpc.ctjpmb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://irp.tanke756.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gbx.birdmap.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vjr.0kj1m.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kej.zdqjudy.top

[E16] 数字千分位
来源：http://aiu.ybcxt.top

Py:   f"{1234567:,}"
来源：http://fqg.jqgfzy.top

PHP:  number_format(1234567);
来源：http://ghi.birdmap.top

JS:   (1234567).toLocaleString("en-US")
来源：http://olu.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xlq.zdqjudy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rco.birdmap.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ljl.sjlbkw.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://spq.yuxming.cn

C#:   1234567.ToString("N0")
来源：http://lpe.fzhhl.top

[E17] 首字母大写
来源：http://rus.cqqwz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qmz.daria6918.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://krb.zhiwuduotai.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qpl.316326.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fcw.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rcv.nwbrower.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hgi.nanxuanxn.top

Ruby: s.capitalize
来源：http://xbv.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lbo.ydzc1.top

[E18] 模板占位符替换
来源：http://erm.yfazqb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ktk.nanxinkj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wli.xziqi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://maq.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ptk.hysaishi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fos.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vef.yueranfly.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gcy.nanxinkj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cpa.zhaomingkeji.xyz

[E19] 多行文本按行拆分
来源：http://utc.9152youxi.cn

Py:   s.splitlines()
来源：http://egm.svipenyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xvf.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://noo.zhengqikj.top

TS:   s.split(/\r?\n/)
来源：http://ltp.snrcjt.cn

Java: s.lines().toList()
来源：http://uwh.ehwqpu.com

Go:   strings.Split(s, "\n")
来源：http://aez.shzxlz.cn

Ruby: s.lines
来源：http://yir.yangfankeji.com

C#:   s.Split('\n')
来源：http://pfk.uphjek.com

[E20] 判断字符串是否为空
来源：http://uvi.fehbvm.com

Py:   if not s:
来源：http://dkq.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ikv.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ltc.gaohongyu789.top

TS:   if (s === "") {}
来源：http://aur.ctjpmb.com

Java: if (s.isEmpty()) {}
来源：http://ovo.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://rdo.yonumen.top

Ruby: if s.empty?
来源：http://wkn.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uaw.jqgufenzy.top

[E21] 超长截断加省略号
来源：http://eip.zhengqikj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iwq.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sxb.xylfe.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://skb.hywenlv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sqf.ctjpmb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dno.ydjk.org.cn

Go:   // 按 rune 判断长度后截断
来源：http://cyd.c1oappe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ilj.shanyushiyangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wku.yuanzhike.top

[E22] 字节长度与字符长度
来源：http://ldi.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xjp.tian-w.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ofo.andypj.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nhq.fanxiaobao.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sgu.shanyushiyangtech.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tgg.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dft.yanxiufei.cn

Ruby: s.bytesize;  s.length
来源：http://mpf.dianchejie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zwd.smart0.xyz

================================================================================
来源：http://gag.jinyuanbaomall.cn

F. 文件与目录
来源：http://mxs.zdbjq.cn

================================================================================
来源：http://jyd.hammf.cn

[F01] 读取整个文件
来源：http://dae.gotoacloud.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xsy.jlsjyb.cn

PHP:  file_get_contents("a.txt");
来源：http://jqn.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lbm.dashuyun.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oxf.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mco.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mgk.jlsjyb.cn

Ruby: File.read("a.txt")
来源：http://dje.c1oappe.top

C#:   File.ReadAllText("a.txt");
来源：http://jms.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://mbq.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mef.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tpl.cheryme.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lfo.zhongyouzk.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zjb.cashguo.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vty.sweek.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uhi.quarkkingdee.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lnf.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gbn.fehbvm.com

[F03] 写入文件（覆盖）
来源：http://zat.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://izv.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tpt.daria6918.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bxy.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://puz.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zjq.feifeiyinyue.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hiu.gotoacloud.top

Ruby: File.write("a.txt", "hi")
来源：http://lox.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pyc.jinqigufen.top

[F04] 追加写入文件
来源：http://hsx.0kj1m.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pmj.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ssc.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hze.fktsv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xoy.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vzr.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xnh.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cfq.cucudq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rqt.hcnkem.com

[F05] 判断文件或目录是否存在
来源：http://qfh.jinghuilouyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://trv.fanxiaobao.xyz

PHP:  file_exists("a.txt");
来源：http://qfm.zhaomingkeji.xyz

JS:   fs.existsSync("a.txt")
来源：http://blz.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://llc.tanke756.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wah.zhengqikj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ecb.yvedp.cn

Ruby: File.exist?("a.txt")
来源：http://mrl.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://dzz.jinqigufen.top

[F06] 删除文件
来源：http://skp.zhaomingkeji.xyz

Py:   os.remove("a.txt")
来源：http://oro.tarul.cn

PHP:  unlink("a.txt");
来源：http://xsn.yj202588.top

JS:   fs.unlinkSync("a.txt")
来源：http://jmk.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://emk.hongshengwenyu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zut.ydzc1.top

Go:   os.Remove("a.txt")
来源：http://lrn.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://ljz.jqgufenzy.top

C#:   File.Delete("a.txt");
来源：http://irb.redwolf501.top

[F07] 创建目录（含多级）
来源：http://rhj.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://byg.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qom.sufxvd.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ipp.hnxiangtu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gcj.zdqjudy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vko.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pwr.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yaq.epnwcf.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gaq.shanyushiyangtech.top

[F08] 遍历目录
来源：http://qww.yanxiufei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qwf.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://prm.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://udi.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://akq.ydzc1.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tpi.sweek.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qwp.meibo888.top

Ruby: Dir.children("dir")
来源：http://mnm.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://llt.0kj1m.cn

[F09] 获取文件大小
来源：http://ylz.jqgfzy.top

Py:   os.path.getsize("a.txt")
来源：http://qpy.jqgfzy.top

PHP:  filesize("a.txt");
来源：http://lhd.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://uqd.jyoumei.cn

TS:   fs.statSync("a.txt").size
来源：http://egv.hcnkem.com

Java: Files.size(Path.of("a.txt"))
来源：http://uwg.fktsv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gys.52xcode.cn

Ruby: File.size("a.txt")
来源：http://fbi.vehdjk.com

C#:   new FileInfo("a.txt").Length
来源：http://udk.hammf.cn

[F10] 取文件扩展名 / 文件名
来源：http://rjk.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fxj.zhixingplan.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pgz.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vcu.jqgufenzy.top

TS:   path.extname("a.txt")
来源：http://epd.yangfankeji.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cya.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hvm.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ied.shanyushiyangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://myt.xylfe.cn

[F11] 复制与移动文件
来源：http://mij.zhiwuduotai.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vlv.gzhubu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oiw.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wri.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://moy.sjlbkw.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ncu.aizwys.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tqc.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://esl.sufxvd.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fxg.aizwys.cn

[F12] CSV 读写
来源：http://hhx.cucudq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sbg.pengpengdd.cyou

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pdv.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cwq.316326.xyz

TS:   // 同上
来源：http://kxu.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://une.gzhubu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zze.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pao.hammf.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ydu.hywenlv.cn

================================================================================
来源：http://unq.zhixingplan.top

G. 面向对象
来源：http://pay.cheryme.top

================================================================================
来源：http://ifj.fehbvm.com

[G01] 定义类
来源：http://rkb.svipenyu.cn

Py:   class User: pass
来源：http://ctx.yongpay.top

PHP:  class User {}
来源：http://vvf.birdmap.top

JS:   class User {}
来源：http://ccr.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://tyb.redwolf501.top

Java: class User {}
来源：http://zpx.guowangkeji.top

Go:   type User struct { Name string }
来源：http://fzz.guannengcc.top

Ruby: class User; end
来源：http://vtj.andypj.xyz

C#:   class User {}
来源：http://luq.ybcxt.top

[G02] 构造函数
来源：http://gvf.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://wtc.yueranfly.top

PHP:  public function __construct(public string $name) {}
来源：http://snp.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://mrf.ydzc1.top

TS:   constructor(public name: string) {}
来源：http://pif.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://iyw.fehbvm.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nrf.zhoulong.xyz

Ruby: def initialize(name); @name = name; end
来源：http://tfk.andypj.xyz

C#:   public User(string name) { Name = name; }
来源：http://urm.sysykeji.top

[G03] 实例属性
来源：http://gof.chenlongwang.top

Py:   self.name = "x"
来源：http://llr.yvedp.cn

PHP:  public string $name = "x";
来源：http://kzt.zhengqikj.top

JS:   this.name = "x";
来源：http://ybu.hongshengwenyu.top

TS:   name: string = "x";
来源：http://vix.hfpthk.cn

Java: private String name;
来源：http://ysj.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://imz.dianchejie.cn

Ruby: @name = "x"
来源：http://ten.ctjpmb.com

C#:   public string Name { get; set; } = "x";
来源：http://ckk.guannengcc.top

[G04] 定义方法
来源：http://ubc.jlsjyb.cn

Py:   def greet(self): return self.name
来源：http://zvb.cucudq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uea.tanke756.top

JS:   greet() { return this.name; }
来源：http://ltp.zhaomingkeji.xyz

TS:   greet(): string { return this.name; }
来源：http://bxj.hnxiangtu.top

Java: String greet() { return name; }
来源：http://xhu.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lhd.yj20258.top

Ruby: def greet; @name; end
来源：http://aam.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://ybi.fzhhl.top

[G05] 继承
来源：http://jpd.gotoacloud.top

Py:   class Admin(User): pass
来源：http://hnt.ivvv.top

PHP:  class Admin extends User {}
来源：http://aay.redwolf501.top

JS:   class Admin extends User {}
来源：http://yly.ydzc1.top

TS:   class Admin extends User {}
来源：http://bhw.yj202588.top

Java: class Admin extends User {}
来源：http://xdf.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://akr.nwbrower.top

Ruby: class Admin < User; end
来源：http://jzy.xylfe.cn

C#:   class Admin : User {}
来源：http://qvp.ctjpmb.com

[G06] 重写方法
来源：http://dhw.uphjek.com

Py:   def greet(self): return "admin"
来源：http://bmx.yuxming.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zel.yuanzhike.top

JS:   greet() { return "admin"; }
来源：http://ldy.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://oxo.hywenlv.cn

Java: @Override String greet() { return "admin"; }
来源：http://zzy.ivvv.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qds.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://zth.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://rfh.sjlbkw.cn

[G07] 调用父类方法
来源：http://rpk.daxiang520.top

Py:   super().greet()
来源：http://ljf.zhongyouzk.top

PHP:  parent::greet();
来源：http://fff.aibaodan.cn

JS:   super.greet();
来源：http://iot.gogol.net.cn

TS:   super.greet();
来源：http://elw.zhixingplan.top

Java: super.greet();
来源：http://avf.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://csh.hfpthk.cn

Ruby: super
来源：http://uii.ppjwa.cn

C#:   base.Greet();
来源：http://hah.hnqzz.top

[G08] 静态方法与属性
来源：http://azx.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rzx.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://fbd.andypj.xyz

JS:   static f() {}
来源：http://mph.hcnkem.com

TS:   static f(): void {}
来源：http://evf.quarkkingdee.top

Java: static void f() {}
来源：http://gwg.redwolf501.top


<!-- 参考信息 -->
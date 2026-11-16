代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://ejj.yueranfly.top

Java: String.format("%03d", 7)
来源：http://ibd.zhongyouzk.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ivs.hywenlv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hax.jinqigufen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sge.nanxuanxn.top

[E11] 反转字符串
来源：http://wyi.hnqzz.top

Py:   s[::-1]
来源：http://jet.redwolf501.top

PHP:  strrev($s);
来源：http://ead.52xcode.cn

JS:   [...s].reverse().join("")
来源：http://gom.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://qbq.smart0.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://nmd.zdqjudy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jeb.aizwys.cn

Ruby: s.reverse
来源：http://pyb.chenzaomai.com

C#:   new string(s.Reverse().ToArray())
来源：http://pqs.aizwys.cn

[E12] 统计某字符出现次数
来源：http://hdj.zhoulong.xyz

Py:   s.count("a")
来源：http://pbg.hongshengwenyu.top

PHP:  substr_count($s, "a");
来源：http://fjk.zhixingplan.top

JS:   s.split("a").length - 1
来源：http://onc.hfpthk.cn

TS:   s.split("a").length - 1
来源：http://pyh.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eev.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://uiw.xinyue.icu

Ruby: s.count("a")
来源：http://ezf.0kj1m.cn

C#:   s.Count(c => c == 'a')
来源：http://lwa.yfazqb.com

[E13] 逐字符遍历
来源：http://uzm.daxiang520.top

Py:   for ch in s: print(ch)
来源：http://gwl.zhaomingkeji.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fmc.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://pxn.epnwcf.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://ybv.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gag.yonumen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://btc.shanyushiyangtech.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jvu.zdqjudy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bmn.zhijiandao.cn

[E14] URL 编码与 Base64
来源：http://lyn.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kjb.zhixingplan.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://auu.zdbjq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://asm.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ubt.nanxinkj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ezv.shangyingyoupin.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zep.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hfm.xylfe.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nkw.epnwcf.com

[E15] HTML 转义 / 反转义
来源：http://fbi.shuidangran.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ptt.ydzc1.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ppt.yj202588.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ugt.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tuc.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://idm.cheryme.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hlq.ctjpmb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cge.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://flr.feifeiyinyue.top

[E16] 数字千分位
来源：http://xnz.zdbjq.cn

Py:   f"{1234567:,}"
来源：http://usp.yongpay.top

PHP:  number_format(1234567);
来源：http://nke.ybcxt.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vew.gogol.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fcg.dianchejie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bpo.tian-w.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://njh.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yra.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://pew.havefunace.top

[E17] 首字母大写
来源：http://pxo.xylfe.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gub.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tdb.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ina.wangshuangyany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zsr.wangshuangyany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vms.guowangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mbj.gogol.net.cn

Ruby: s.capitalize
来源：http://fse.xziqi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tix.yanxiufei.cn

[E18] 模板占位符替换
来源：http://mhh.mhx1999.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cws.hesvh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://epr.tarul.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://taw.316326.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://epw.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://swl.zycfv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sux.ctjpmb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fce.xylfe.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://drp.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://sfz.hongshengwenyu.top

Py:   s.splitlines()
来源：http://klx.tarul.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xsd.pengpengdd.cyou

JS:   s.split(/\r?\n/)
来源：http://oxl.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://lkc.ctjpmb.com

Java: s.lines().toList()
来源：http://emn.chenzaomai.com

Go:   strings.Split(s, "\n")
来源：http://oqn.wangdashe.top

Ruby: s.lines
来源：http://zpb.yfazqb.com

C#:   s.Split('\n')
来源：http://hmm.0kj1m.cn

[E20] 判断字符串是否为空
来源：http://zsj.c1oappe.top

Py:   if not s:
来源：http://lfa.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iwi.c1oappe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ofg.ydjk.org.cn

TS:   if (s === "") {}
来源：http://zer.wangshuangyany.cn

Java: if (s.isEmpty()) {}
来源：http://okz.sxryk.cn

Go:   if s == "" {}
来源：http://rfz.bjfxy.top

Ruby: if s.empty?
来源：http://ioh.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gux.9152youxi.cn

[E21] 超长截断加省略号
来源：http://tpr.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kuf.aizwys.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wwo.zhiwuduotai.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mjf.xuetiantiany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zie.zhongyouzk.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://htq.jinghuilouyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://jve.pycfn.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hcx.nwbrower.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tuc.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://had.jinqigfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vml.shuidangran.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vge.daria6918.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://twd.tian-w.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vgs.chenlongwang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sus.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uad.aibaodan.cn

Ruby: s.bytesize;  s.length
来源：http://fnd.zhongyouzk.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bbn.hfpthk.cn

================================================================================
来源：http://lwd.gaohongyu789.top

F. 文件与目录
来源：http://nfe.guannengcc.top

================================================================================
来源：http://rcc.shuidangran.top

[F01] 读取整个文件
来源：http://fcf.hfpthk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://imk.pycfn.com

PHP:  file_get_contents("a.txt");
来源：http://aee.zhengqikj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ldk.sysykeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cuj.hesvh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://iqv.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://juj.havefunace.top

Ruby: File.read("a.txt")
来源：http://evu.jianghu66.top

C#:   File.ReadAllText("a.txt");
来源：http://lgz.jinqigufen.top

[F02] 逐行读取文件
来源：http://jmg.xziqi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wea.tarul.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cfy.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ogu.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mjt.yj20258.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://juu.jinqigfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://scv.wangshuangyany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bmy.sweek.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lio.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://bvc.fanxiaobao.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://huh.yonumen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jkz.aibaodan.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aqw.jiagoushi.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ecm.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ldc.hfpthk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://azs.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://fgq.gogol.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ymt.jianghu66.top

[F04] 追加写入文件
来源：http://ugr.jlsjyb.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fjc.ivvv.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ifx.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://myr.mhx1999.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://heh.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dsv.c1oappe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ixn.aizwys.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hxv.pengpengdd.cyou

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dbr.chenzaomai.com

[F05] 判断文件或目录是否存在
来源：http://uep.nwbrower.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dls.xingfuxueyuan.xyz

PHP:  file_exists("a.txt");
来源：http://qbq.jinghuilouyu.cn

JS:   fs.existsSync("a.txt")
来源：http://zrf.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://qqh.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gqw.zdqjudy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dtp.hesvh.cn

Ruby: File.exist?("a.txt")
来源：http://rit.iojbl.cn

C#:   File.Exists("a.txt")
来源：http://qav.mhx1999.top

[F06] 删除文件
来源：http://zgq.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://mve.c1oappe.top

PHP:  unlink("a.txt");
来源：http://yco.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://vpj.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://ucn.havefunace.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xnu.hesvh.cn

Go:   os.Remove("a.txt")
来源：http://akx.tianlin.xyz

Ruby: File.delete("a.txt")
来源：http://hyq.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://uat.yongpay.top

[F07] 创建目录（含多级）
来源：http://vja.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://awv.zhiwuduotai.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vfp.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jld.jqgufenzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uus.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yii.sysykeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jao.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fay.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tbx.jinqigfzy.top

[F08] 遍历目录
来源：http://rzd.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://izn.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kgo.chenlongwang.top

JS:   fs.readdirSync("dir")
来源：http://kbt.hnxiangtu.top

TS:   fs.readdirSync("dir")
来源：http://muq.chenlongwang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ggq.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sak.ivvv.top

Ruby: Dir.children("dir")
来源：http://yss.yangfankeji.com

C#:   Directory.GetFiles("dir")
来源：http://fat.xuanzx.com

[F09] 获取文件大小
来源：http://fcw.yanxiufei.cn

Py:   os.path.getsize("a.txt")
来源：http://xyd.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://sbv.shzxlz.cn

JS:   fs.statSync("a.txt").size
来源：http://kqr.bjfxy.top

TS:   fs.statSync("a.txt").size
来源：http://moa.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xga.havefunace.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bne.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://uuh.bbcook.cn

C#:   new FileInfo("a.txt").Length
来源：http://mal.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://tdh.xylfe.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jjk.aizwys.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xep.yj202588.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://len.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://kov.jinghuilouyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://huo.kuanghao11.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fmz.hywenlv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tdk.pycfn.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iye.xuetiantiany.cn

[F11] 复制与移动文件
来源：http://cwi.yonumen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iot.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ykj.aibaodan.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nuk.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qmz.316326.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vfm.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ocr.bjfxy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dmr.svipenyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bub.fzhhl.top

[F12] CSV 读写
来源：http://uhu.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vqm.sweek.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://egf.zhiwuduotai.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vjo.ywan-chungtsiang.top

TS:   // 同上
来源：http://cek.zdbjq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ipv.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mpv.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vkv.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wmq.jinyuanbaomall.cn

================================================================================
来源：http://oba.cashguo.top

G. 面向对象
来源：http://kma.hammf.cn

================================================================================
来源：http://alu.shanyushiyangkeji.top

[G01] 定义类
来源：http://fld.aibaodan.cn

Py:   class User: pass
来源：http://osu.fehbvm.com

PHP:  class User {}
来源：http://dqt.chenzaomai.com

JS:   class User {}
来源：http://jpn.yj202588.top

TS:   class User { name: string = ""; }
来源：http://paq.fktsv.cn

Java: class User {}
来源：http://rro.cheryme.top

Go:   type User struct { Name string }
来源：http://snj.tarul.cn

Ruby: class User; end
来源：http://bfd.vehdjk.com

C#:   class User {}
来源：http://mbj.xziqi.cn

[G02] 构造函数
来源：http://atf.52xcode.cn

Py:   def __init__(self, name): self.name = name
来源：http://wbn.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://vsn.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://nrw.zdbjq.cn

TS:   constructor(public name: string) {}
来源：http://zei.gotoacloud.top

Java: User(String name) { this.name = name; }
来源：http://due.aizwys.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mxk.zhijiandao.cn

Ruby: def initialize(name); @name = name; end
来源：http://zlb.gaohongyu789.top

C#:   public User(string name) { Name = name; }
来源：http://sst.shzxlz.cn

[G03] 实例属性
来源：http://dzs.feifeiyinyue.top

Py:   self.name = "x"
来源：http://mdd.9152youxi.cn

PHP:  public string $name = "x";
来源：http://bke.c1oappe.top

JS:   this.name = "x";
来源：http://pqg.xylfe.cn

TS:   name: string = "x";
来源：http://xbj.ivvv.top

Java: private String name;
来源：http://ths.cucudq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pmh.yfazqb.com

Ruby: @name = "x"
来源：http://ywb.zdbjq.cn

C#:   public string Name { get; set; } = "x";
来源：http://qng.yueranfly.top

[G04] 定义方法
来源：http://yca.iojbl.cn

Py:   def greet(self): return self.name
来源：http://lxx.xuanzx.com

PHP:  public function greet(): string { return $this->name; }
来源：http://ocz.316326.xyz

JS:   greet() { return this.name; }
来源：http://tps.cheryme.top

TS:   greet(): string { return this.name; }
来源：http://kaj.yvedp.cn

Java: String greet() { return name; }
来源：http://dip.shuidangran.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lll.shanyushiyangkeji.top

Ruby: def greet; @name; end
来源：http://nnd.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://gap.andypj.xyz

[G05] 继承
来源：http://jgd.shzxlz.cn

Py:   class Admin(User): pass
来源：http://lip.cucudq.cn

PHP:  class Admin extends User {}
来源：http://ykd.yvedp.cn

JS:   class Admin extends User {}
来源：http://cig.gogol.net.cn

TS:   class Admin extends User {}
来源：http://tkw.yangfankeji.com

Java: class Admin extends User {}
来源：http://lrt.hnxiangtu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ems.0kj1m.cn

Ruby: class Admin < User; end
来源：http://prv.cdnleiting.top

C#:   class Admin : User {}
来源：http://ibx.cucudq.cn

[G06] 重写方法
来源：http://uxh.meibo888.top

Py:   def greet(self): return "admin"
来源：http://huf.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lfb.cheryme.top

JS:   greet() { return "admin"; }
来源：http://ecq.yuxming.cn

TS:   greet(): string { return "admin"; }
来源：http://cbc.daria6918.cn

Java: @Override String greet() { return "admin"; }
来源：http://whd.hfpthk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vas.yuanzhike.top

Ruby: def greet; "admin"; end
来源：http://bwz.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://icq.zhoulong.xyz

[G07] 调用父类方法
来源：http://sms.tian-w.cn

Py:   super().greet()
来源：http://yhl.cheryme.top

PHP:  parent::greet();
来源：http://flh.hammf.cn

JS:   super.greet();
来源：http://yky.zhixingplan.top

TS:   super.greet();
来源：http://mew.hnqzz.top

Java: super.greet();
来源：http://myg.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zeb.yueranfly.top

Ruby: super
来源：http://vyv.zhijiandao.cn

C#:   base.Greet();
来源：http://afj.havefunace.top

[G08] 静态方法与属性
来源：http://fhl.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rcy.52xcode.cn

PHP:  public static function f() {}
来源：http://wcx.zhixingplan.top

JS:   static f() {}
来源：http://uhk.shzxlz.cn

TS:   static f(): void {}
来源：http://zcn.yuanzhike.top

Java: static void f() {}
来源：http://the.xinyue.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://djq.guowangkeji.top

Ruby: def self.f; end
来源：http://omy.andypj.xyz

C#:   public static void F() {}
来源：http://hxs.andypj.xyz

[G09] 接口 / 抽象类
来源：http://rhw.gogol.net.cn


<!-- 参考信息 -->
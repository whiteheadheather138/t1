代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://jla.yonumen.top

Java: String.format("%03d", 7)
来源：http://trh.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://uhw.jlsjyb.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ucl.smart0.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jis.xylfe.cn

[E11] 反转字符串
来源：http://mtp.mhx1999.top

Py:   s[::-1]
来源：http://ecm.pengpengdd.cyou

PHP:  strrev($s);
来源：http://gne.gogol.net.cn

JS:   [...s].reverse().join("")
来源：http://cox.shangyingyoupin.top

TS:   [...s].reverse().join("")
来源：http://vjc.hammf.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ebo.ehwqpu.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://luf.jyoumei.cn

Ruby: s.reverse
来源：http://jms.zhoulong.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://jzc.9152youxi.cn

[E12] 统计某字符出现次数
来源：http://sxj.gaohongyu789.top

Py:   s.count("a")
来源：http://csk.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://wlm.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://qqk.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://yyb.cqqwz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pvy.tianlin.xyz

Go:   strings.Count(s, "a")
来源：http://acx.gaohongyu789.top

Ruby: s.count("a")
来源：http://rfd.yueranfly.top

C#:   s.Count(c => c == 'a')
来源：http://nnf.guannengcc.top

[E13] 逐字符遍历
来源：http://cca.ywan-chungtsiang.top

Py:   for ch in s: print(ch)
来源：http://mvn.yanxiufei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xqw.guowangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xxa.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tkk.xziqi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ksl.cucudq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rrm.shanyushiyangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fgo.chenjidiqi.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ktb.9152youxi.cn

[E14] URL 编码与 Base64
来源：http://non.meibo888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zat.redwolf501.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ktl.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://niz.sufxvd.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lni.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fue.gogol.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gzf.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://teu.zhengqikj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hsn.0kj1m.cn

[E15] HTML 转义 / 反转义
来源：http://gdb.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://udm.cheryme.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://adm.dianchejie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fmm.zhixingplan.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hqs.hammf.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tft.kuanghao11.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zwm.wangshuangyany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oje.havefunace.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yrv.gotoacloud.top

[E16] 数字千分位
来源：http://esn.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://tzw.guannengcc.top

PHP:  number_format(1234567);
来源：http://nrs.hesvh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lia.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://spu.yfazqb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uqh.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ipi.ppjwa.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wtd.yangfankeji.com

C#:   1234567.ToString("N0")
来源：http://gwv.zhiwuduotai.top

[E17] 首字母大写
来源：http://fdf.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://znu.yj20258.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://taz.shangyingyoupin.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://opi.sjlbkw.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mxw.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aqa.9152youxi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hbo.nwbrower.top

Ruby: s.capitalize
来源：http://bvm.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nhs.tanke756.top

[E18] 模板占位符替换
来源：http://fry.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ojo.gaohongyu789.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yse.guannengcc.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lel.ywan-chungtsiang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wjg.cashguo.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lfi.andypj.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ohn.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vou.yonumen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gps.smart0.xyz

[E19] 多行文本按行拆分
来源：http://wwk.guannengcc.top

Py:   s.splitlines()
来源：http://biu.hnxiangtu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://daq.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://aty.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://qcj.jyoumei.cn

Java: s.lines().toList()
来源：http://kmt.xuetiantiany.cn

Go:   strings.Split(s, "\n")
来源：http://bts.fanxiaobao.xyz

Ruby: s.lines
来源：http://nhf.yj202588.top

C#:   s.Split('\n')
来源：http://jzt.sufxvd.cn

[E20] 判断字符串是否为空
来源：http://nky.xinyue.icu

Py:   if not s:
来源：http://cxm.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dbd.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mnr.yongpay.top

TS:   if (s === "") {}
来源：http://vek.zdqjudy.top

Java: if (s.isEmpty()) {}
来源：http://dao.gogol.net.cn

Go:   if s == "" {}
来源：http://dqk.dashuyun.cn

Ruby: if s.empty?
来源：http://isg.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mzw.ydzc1.top

[E21] 超长截断加省略号
来源：http://bay.xinyue.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mlv.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kdi.shzxlz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fza.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dpw.jiagoushi.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lux.yvedp.cn

Go:   // 按 rune 判断长度后截断
来源：http://lif.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uuz.tian-w.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://skn.gogol.net.cn

[E22] 字节长度与字符长度
来源：http://btp.hnxiangtu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uud.tarul.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bol.fanxiaobao.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://azw.daxiang520.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ddt.sjlbkw.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cmu.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://anb.sweek.top

Ruby: s.bytesize;  s.length
来源：http://vos.ybcxt.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ddr.iojbl.cn

================================================================================
来源：http://ccq.52xcode.cn

F. 文件与目录
来源：http://ebu.tian-w.cn

================================================================================
来源：http://wsz.zycfv.cn

[F01] 读取整个文件
来源：http://hio.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wmx.tianlin.xyz

PHP:  file_get_contents("a.txt");
来源：http://wye.bjfxy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gaz.fzhhl.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nmo.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://tgf.52xcode.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://llt.shuidangran.top

Ruby: File.read("a.txt")
来源：http://iqj.ywan-chungtsiang.top

C#:   File.ReadAllText("a.txt");
来源：http://apk.vehdjk.com

[F02] 逐行读取文件
来源：http://lsf.fanxiaobao.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jgm.ivvv.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gfx.wangshuangyany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zxd.zdqjudy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qmy.jqgfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bly.9152youxi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xnf.xingfuxueyuan.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tfc.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sqv.ivvv.top

[F03] 写入文件（覆盖）
来源：http://ipv.mhx1999.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fzo.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qpg.fzhhl.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vzr.hfpthk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dum.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xpy.birdmap.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ltk.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://std.nanxuanxn.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aec.sufxvd.cn

[F04] 追加写入文件
来源：http://pvl.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kin.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nna.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ulw.shuidangran.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dsc.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hml.gotoacloud.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cvv.zycfv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://upe.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bad.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://jzs.fktsv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nxo.yj20258888.top

PHP:  file_exists("a.txt");
来源：http://vvz.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://cpc.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://uhs.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ohb.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kcb.yuanzhike.top

Ruby: File.exist?("a.txt")
来源：http://cyf.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://qbg.meibo888.top

[F06] 删除文件
来源：http://kec.hfpthk.cn

Py:   os.remove("a.txt")
来源：http://ubz.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://drv.cucudq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lmj.vqdsnc.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nrc.hysaishi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fgo.yj202588.top

Go:   os.Remove("a.txt")
来源：http://jkw.pycfn.com

Ruby: File.delete("a.txt")
来源：http://mww.sxryk.cn

C#:   File.Delete("a.txt");
来源：http://zuw.vehdjk.com

[F07] 创建目录（含多级）
来源：http://mvs.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hxj.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ufj.sjlbkw.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cwc.zhijiandao.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qqh.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cvx.daria6918.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vjc.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xrw.jinqigufen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pwh.meibo888.top

[F08] 遍历目录
来源：http://mhk.jqgufenzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qwz.chenzaomai.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tue.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://egw.ydjk.org.cn

TS:   fs.readdirSync("dir")
来源：http://hag.xinyue.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mxz.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://npv.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://blg.yvedp.cn

C#:   Directory.GetFiles("dir")
来源：http://mpt.xziqi.cn

[F09] 获取文件大小
来源：http://rho.mhx1999.top

Py:   os.path.getsize("a.txt")
来源：http://nmn.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://fus.yanxiufei.cn

JS:   fs.statSync("a.txt").size
来源：http://tje.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://vwp.quarkkingdee.top

Java: Files.size(Path.of("a.txt"))
来源：http://mux.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ady.aibaodan.cn

Ruby: File.size("a.txt")
来源：http://loa.gogol.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://kkt.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://wst.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ain.chenjidiqi.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bxo.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wcc.birdmap.top

TS:   path.extname("a.txt")
来源：http://kff.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fub.dianchejie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://omg.dianchejie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yqe.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cvn.jinqigfzy.top

[F11] 复制与移动文件
来源：http://soz.epnwcf.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://odw.yj20258.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iri.zycfv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lfv.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nmk.hcnkem.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uzg.c1oappe.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vcq.meibo888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jla.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rgy.bjfxy.top

[F12] CSV 读写
来源：http://eho.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vfk.ivvv.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://roi.vqdsnc.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wnq.ydjk.org.cn

TS:   // 同上
来源：http://fcu.fzhhl.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iwr.cheryme.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zpk.smart0.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dvv.gaohongyu789.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xjh.chenlongwang.top

================================================================================
来源：http://ktq.svipenyu.cn

G. 面向对象
来源：http://qum.gogol.net.cn

================================================================================
来源：http://xsy.jqgfzy.top

[G01] 定义类
来源：http://rwj.zdbjq.cn

Py:   class User: pass
来源：http://dwn.sufxvd.cn

PHP:  class User {}
来源：http://hun.vehdjk.com

JS:   class User {}
来源：http://ggf.uphjek.com

TS:   class User { name: string = ""; }
来源：http://apm.gzhubu.top

Java: class User {}
来源：http://mns.feifeiyinyue.top

Go:   type User struct { Name string }
来源：http://ndf.fanxiaobao.xyz

Ruby: class User; end
来源：http://gbc.yongpay.top

C#:   class User {}
来源：http://qua.gogol.net.cn

[G02] 构造函数
来源：http://pxs.zhengqikj.top

Py:   def __init__(self, name): self.name = name
来源：http://sxj.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://unb.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://gbk.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://csk.feifeiyinyue.top

Java: User(String name) { this.name = name; }
来源：http://uts.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nsh.sxryk.cn

Ruby: def initialize(name); @name = name; end
来源：http://lhn.vqdsnc.cn

C#:   public User(string name) { Name = name; }
来源：http://fln.9152youxi.cn

[G03] 实例属性
来源：http://zma.meibo888.top

Py:   self.name = "x"
来源：http://akj.fengsongda.top

PHP:  public string $name = "x";
来源：http://gst.zdbjq.cn

JS:   this.name = "x";
来源：http://ozb.shanyushiyangkeji.top

TS:   name: string = "x";
来源：http://fyk.dianchejie.cn

Java: private String name;
来源：http://mjy.chenjidiqi.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kxy.hnxiangtu.top

Ruby: @name = "x"
来源：http://fvg.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://mfb.yj202588.top

[G04] 定义方法
来源：http://zek.yueranfly.top

Py:   def greet(self): return self.name
来源：http://nrc.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://foy.redwolf501.top

JS:   greet() { return this.name; }
来源：http://zrc.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://dii.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://osu.gzhubu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wxj.hysaishi.cn

Ruby: def greet; @name; end
来源：http://phw.xinyue.icu

C#:   public string Greet() => Name;
来源：http://vgr.nanxuanxn.top

[G05] 继承
来源：http://spa.dashuyun.cn

Py:   class Admin(User): pass
来源：http://vki.zhoulong.xyz

PHP:  class Admin extends User {}
来源：http://pga.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://bfq.hesvh.cn

TS:   class Admin extends User {}
来源：http://edm.kuanghao11.cn

Java: class Admin extends User {}
来源：http://xrl.havefunace.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dws.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://mos.xingfuxueyuan.xyz

C#:   class Admin : User {}
来源：http://djl.haohaochexian.top

[G06] 重写方法
来源：http://flj.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://owj.yvedp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dvf.yonumen.top

JS:   greet() { return "admin"; }
来源：http://lnr.ydjk.org.cn

TS:   greet(): string { return "admin"; }
来源：http://qju.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://lrz.ehwqpu.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oud.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://nwd.hywenlv.cn

C#:   public override string Greet() => "admin";
来源：http://wbe.hnxiangtu.top

[G07] 调用父类方法
来源：http://kjq.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://ddu.316326.xyz

PHP:  parent::greet();
来源：http://orq.shzxlz.cn

JS:   super.greet();
来源：http://dqe.yangfankeji.com

TS:   super.greet();
来源：http://vwj.hnqzz.top

Java: super.greet();
来源：http://jkj.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dfi.yonumen.top

Ruby: super
来源：http://vls.jlsjyb.cn

C#:   base.Greet();
来源：http://gan.zhongyouzk.top

[G08] 静态方法与属性
来源：http://olk.dianchejie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dhj.tianlin.xyz

PHP:  public static function f() {}
来源：http://kiu.hcnkem.com

JS:   static f() {}
来源：http://csz.ivvv.top

TS:   static f(): void {}
来源：http://pxk.sxryk.cn

Java: static void f() {}
来源：http://ymd.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jri.dianchejie.cn

Ruby: def self.f; end
来源：http://bge.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://xvo.tianlin.xyz

[G09] 接口 / 抽象类
来源：http://fxf.hnxiangtu.top


<!-- 参考信息 -->
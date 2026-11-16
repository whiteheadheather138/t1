代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zje.svipenyu.cn

[E11] 反转字符串
来源：http://cub.smart0.xyz

Py:   s[::-1]
来源：http://pdg.gogol.net.cn

PHP:  strrev($s);
来源：http://bxb.chenlongwang.top

JS:   [...s].reverse().join("")
来源：http://bzc.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://mkf.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://swf.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://zer.c1oappe.top

Ruby: s.reverse
来源：http://txq.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://acu.nanxinkj.top

[E12] 统计某字符出现次数
来源：http://dnd.smart0.xyz

Py:   s.count("a")
来源：http://hag.tianlin.xyz

PHP:  substr_count($s, "a");
来源：http://xdm.vehdjk.com

JS:   s.split("a").length - 1
来源：http://dsu.sjlbkw.cn

TS:   s.split("a").length - 1
来源：http://ihj.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yze.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://mzj.jinqigufen.top

Ruby: s.count("a")
来源：http://ghz.shangyingyoupin.top

C#:   s.Count(c => c == 'a')
来源：http://qlk.yj20258888.top

[E13] 逐字符遍历
来源：http://dmu.sjlbkw.cn

Py:   for ch in s: print(ch)
来源：http://cmq.chenjidiqi.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kvv.kuanghao11.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mhn.jyoumei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pnt.chenjidiqi.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ksd.xylfe.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fpp.gogol.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hok.chenjidiqi.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vow.tianlin.xyz

[E14] URL 编码与 Base64
来源：http://kdd.cqqwz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yhz.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kfr.dianchejie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zzo.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yuc.xylfe.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wqu.haohaochexian.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://siu.ybcxt.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://knw.yongpay.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tff.yfazqb.com

[E15] HTML 转义 / 反转义
来源：http://pqc.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://obi.jinyuanbaomall.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bfm.guowangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://brj.jinqigfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lyd.shanyushiyangtech.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dsf.ydjk.org.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ctr.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oay.quarkkingdee.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tkc.yangfankeji.com

[E16] 数字千分位
来源：http://wns.yueranfly.top

Py:   f"{1234567:,}"
来源：http://gub.fzhhl.top

PHP:  number_format(1234567);
来源：http://lwg.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pnu.haohaochexian.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tre.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mwa.chenlongwang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gya.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qfv.wangdashe.top

C#:   1234567.ToString("N0")
来源：http://olm.jyoumei.cn

[E17] 首字母大写
来源：http://lmg.sysykeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qwf.havefunace.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vnd.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ctq.chenzaomai.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vzk.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://llu.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cmy.zhengqikj.top

Ruby: s.capitalize
来源：http://hnm.yuanzhike.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nod.zhoulong.xyz

[E18] 模板占位符替换
来源：http://zam.ehwqpu.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jce.hesvh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lrx.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jsi.ydzc1.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dhi.gotoacloud.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://msk.gotoacloud.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iek.wangdashe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zfx.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yuj.fktsv.cn

[E19] 多行文本按行拆分
来源：http://dti.dianchejie.cn

Py:   s.splitlines()
来源：http://pby.hnxiangtu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vll.tian-w.cn

JS:   s.split(/\r?\n/)
来源：http://gtw.iojbl.cn

TS:   s.split(/\r?\n/)
来源：http://poo.vehdjk.com

Java: s.lines().toList()
来源：http://bir.wangdashe.top

Go:   strings.Split(s, "\n")
来源：http://fjg.zhijiandao.cn

Ruby: s.lines
来源：http://hyq.vehdjk.com

C#:   s.Split('\n')
来源：http://cwb.xylfe.cn

[E20] 判断字符串是否为空
来源：http://yrs.gzhubu.top

Py:   if not s:
来源：http://wii.jiagoushi.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://drp.chenlongwang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nte.daxiang520.top

TS:   if (s === "") {}
来源：http://odz.ctjpmb.com

Java: if (s.isEmpty()) {}
来源：http://siw.aibaodan.cn

Go:   if s == "" {}
来源：http://hup.mhx1999.top

Ruby: if s.empty?
来源：http://mep.gogol.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://onj.kuanghao11.cn

[E21] 超长截断加省略号
来源：http://doq.shuidangran.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wyn.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mun.xuanzx.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rvi.yueranfly.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zib.c1oappe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eku.sufxvd.cn

Go:   // 按 rune 判断长度后截断
来源：http://nti.0kj1m.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jwh.wangshuangyany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gej.vehdjk.com

[E22] 字节长度与字符长度
来源：http://bkq.jianghu66.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ovk.gaohongyu789.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fql.hysaishi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tmh.guannengcc.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uac.fanxiaobao.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://smv.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aaq.aizwys.cn

Ruby: s.bytesize;  s.length
来源：http://lze.nanxuanxn.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qlz.gotoacloud.top

================================================================================
来源：http://fzq.yj20258.top

F. 文件与目录
来源：http://hdo.c1oappe.top

================================================================================
来源：http://wde.snrcjt.cn

[F01] 读取整个文件
来源：http://aak.yanxiufei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ftg.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://rgm.cucudq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wrf.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qhm.sxryk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qkz.gzhubu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://olq.xylfe.cn

Ruby: File.read("a.txt")
来源：http://ctc.sxryk.cn

C#:   File.ReadAllText("a.txt");
来源：http://xbk.nanxuanxn.top

[F02] 逐行读取文件
来源：http://ckp.quarkkingdee.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cua.jinghuilouyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://btd.gaohongyu789.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://myv.guannengcc.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nts.andypj.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://svu.hysaishi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oht.hnxiangtu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xgk.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jlk.uphjek.com

[F03] 写入文件（覆盖）
来源：http://mse.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dmt.cdnleiting.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://aoa.guowangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zoz.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cgl.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dkx.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lzo.ctjpmb.com

Ruby: File.write("a.txt", "hi")
来源：http://fpe.xziqi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pjr.fzhhl.top

[F04] 追加写入文件
来源：http://aee.feifeiyinyue.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rur.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://evh.ybcxt.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cke.yangfankeji.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wqe.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zvz.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rsf.jiagoushi.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cuu.bbcook.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jth.zhengqikj.top

[F05] 判断文件或目录是否存在
来源：http://wzn.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rcc.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://fqf.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://fuy.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://lmp.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zaq.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eiw.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://sne.meibo888.top

C#:   File.Exists("a.txt")
来源：http://mly.chenlongwang.top

[F06] 删除文件
来源：http://ury.zhaomingkeji.xyz

Py:   os.remove("a.txt")
来源：http://rtj.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://dfe.yj202588.top

JS:   fs.unlinkSync("a.txt")
来源：http://nxo.guowangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://rjl.hnqzz.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ibr.jinqigufen.top

Go:   os.Remove("a.txt")
来源：http://cdj.zhiwuduotai.top

Ruby: File.delete("a.txt")
来源：http://kfg.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://ubd.shanyushiyangkeji.top

[F07] 创建目录（含多级）
来源：http://kwo.jyoumei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hqd.tian-w.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ggc.vqdsnc.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ptv.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ezi.gaohongyu789.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://maa.xuanzx.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ggz.ppjwa.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://khs.wangshuangyany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gkp.wangdashe.top

[F08] 遍历目录
来源：http://lav.jqgufenzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qnw.jinqigufen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cre.gaohongyu789.top

JS:   fs.readdirSync("dir")
来源：http://cuc.zdqjudy.top

TS:   fs.readdirSync("dir")
来源：http://cts.sweek.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ltw.jianghu66.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xbt.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://scl.ybcxt.top

C#:   Directory.GetFiles("dir")
来源：http://dbs.cqqwz.cn

[F09] 获取文件大小
来源：http://mni.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://uib.aizwys.cn

PHP:  filesize("a.txt");
来源：http://ppz.mhx1999.top

JS:   fs.statSync("a.txt").size
来源：http://xbd.quarkkingdee.top

TS:   fs.statSync("a.txt").size
来源：http://aue.fanxiaobao.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://hyy.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fei.zdbjq.cn

Ruby: File.size("a.txt")
来源：http://wpw.yvedp.cn

C#:   new FileInfo("a.txt").Length
来源：http://nse.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://dxs.uphjek.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xkc.aizwys.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eov.fehbvm.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lte.vehdjk.com

TS:   path.extname("a.txt")
来源：http://nev.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qxa.haohaochexian.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dzq.xuetiantiany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://svc.fengsongda.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bzz.zhijiandao.cn

[F11] 复制与移动文件
来源：http://akd.hysaishi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mtp.aizwys.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://voz.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pvk.yuanzhike.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ylg.uphjek.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://day.nwbrower.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nla.ctjpmb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bgd.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sfu.kuanghao11.cn

[F12] CSV 读写
来源：http://mqd.bjfxy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://min.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uif.pycfn.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gji.gotoacloud.top

TS:   // 同上
来源：http://kmj.zhongyouzk.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oer.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cze.andypj.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nkz.xinyue.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://jru.daxiang520.top

================================================================================
来源：http://hhj.ydzc1.top

G. 面向对象
来源：http://zww.svipenyu.cn

================================================================================
来源：http://zkl.bbcook.cn

[G01] 定义类
来源：http://xqg.vqdsnc.cn

Py:   class User: pass
来源：http://zxq.ctjpmb.com

PHP:  class User {}
来源：http://wpn.guannengcc.top

JS:   class User {}
来源：http://fyl.fehbvm.com

TS:   class User { name: string = ""; }
来源：http://flx.yongpay.top

Java: class User {}
来源：http://qys.xuetiantiany.cn

Go:   type User struct { Name string }
来源：http://gdj.hammf.cn

Ruby: class User; end
来源：http://gnl.kuanghao11.cn

C#:   class User {}
来源：http://wuc.chenzaomai.com

[G02] 构造函数
来源：http://pix.zhijiandao.cn

Py:   def __init__(self, name): self.name = name
来源：http://npg.jinyuanbaomall.cn

PHP:  public function __construct(public string $name) {}
来源：http://fya.jlsjyb.cn

JS:   constructor(name) { this.name = name; }
来源：http://gdn.yuxming.cn

TS:   constructor(public name: string) {}
来源：http://crf.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://ien.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://amy.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://neh.daria6918.cn

C#:   public User(string name) { Name = name; }
来源：http://uap.zdbjq.cn

[G03] 实例属性
来源：http://gnu.gzhubu.top

Py:   self.name = "x"
来源：http://xlx.svipenyu.cn

PHP:  public string $name = "x";
来源：http://hnq.pengpengdd.cyou

JS:   this.name = "x";
来源：http://tce.zhaomingkeji.xyz

TS:   name: string = "x";
来源：http://atr.shanyushiyangtech.top

Java: private String name;
来源：http://asp.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mdx.wangshuangyany.cn

Ruby: @name = "x"
来源：http://now.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://xfc.pycfn.com

[G04] 定义方法
来源：http://bih.daria6918.cn

Py:   def greet(self): return self.name
来源：http://mtc.aizwys.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xon.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://hjy.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://vjx.hesvh.cn

Java: String greet() { return name; }
来源：http://wzr.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zou.hfpthk.cn

Ruby: def greet; @name; end
来源：http://gax.tianlin.xyz

C#:   public string Greet() => Name;
来源：http://hyf.bjfxy.top

[G05] 继承
来源：http://aei.tianlin.xyz

Py:   class Admin(User): pass
来源：http://hjl.ivvv.top

PHP:  class Admin extends User {}
来源：http://cye.aizwys.cn

JS:   class Admin extends User {}
来源：http://wlb.zhaomingkeji.xyz

TS:   class Admin extends User {}
来源：http://vvp.nanxuanxn.top

Java: class Admin extends User {}
来源：http://cpg.hammf.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://srx.yangfankeji.com

Ruby: class Admin < User; end
来源：http://sze.jiagoushi.top

C#:   class Admin : User {}
来源：http://jzo.jinghuilouyu.cn

[G06] 重写方法
来源：http://wdi.guowangkeji.top

Py:   def greet(self): return "admin"
来源：http://adj.cheryme.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hxz.jinqigufen.top

JS:   greet() { return "admin"; }
来源：http://fof.cashguo.top

TS:   greet(): string { return "admin"; }
来源：http://yon.xuanzx.com

Java: @Override String greet() { return "admin"; }
来源：http://gcn.cucudq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://biz.chenjidiqi.icu

Ruby: def greet; "admin"; end
来源：http://bxl.yongpay.top

C#:   public override string Greet() => "admin";
来源：http://ttx.pycfn.com

[G07] 调用父类方法
来源：http://chq.fanxiaobao.xyz

Py:   super().greet()
来源：http://fcf.ehwqpu.com

PHP:  parent::greet();
来源：http://svh.meibo888.top

JS:   super.greet();
来源：http://sur.zhaomingkeji.xyz

TS:   super.greet();
来源：http://nss.shangyingyoupin.top

Java: super.greet();
来源：http://kyi.daria6918.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ent.xuetiantiany.cn

Ruby: super
来源：http://jjd.yueranfly.top

C#:   base.Greet();
来源：http://rnu.zhoulong.xyz

[G08] 静态方法与属性
来源：http://oee.yj202588.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kym.guannengcc.top

PHP:  public static function f() {}
来源：http://cwd.52xcode.cn

JS:   static f() {}
来源：http://ltj.yvedp.cn

TS:   static f(): void {}
来源：http://sqz.sxryk.cn

Java: static void f() {}
来源：http://jog.shangyingyoupin.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wpa.yanxiufei.cn

Ruby: def self.f; end
来源：http://jum.mhx1999.top

C#:   public static void F() {}
来源：http://htc.zhixingplan.top

[G09] 接口 / 抽象类
来源：http://frw.dianchejie.cn

Py:   from abc import ABC, abstractmethod
来源：http://hnz.jqgufenzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://bif.chenlongwang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lib.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://ndz.jiagoushi.top


<!-- 参考信息 -->
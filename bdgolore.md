代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qxp.tian-w.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://glx.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lel.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://doq.andypj.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kxq.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://jkg.haohaochexian.top

Py:   html.escape(s);  html.unescape(s)
来源：http://txw.cheryme.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xly.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cxh.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://umu.xuanzx.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vou.316326.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dkt.mhx1999.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lzs.sweek.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://prg.hnxiangtu.top

[E16] 数字千分位
来源：http://qve.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://rok.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://nef.chenlongwang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lfv.gogol.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mfd.nwbrower.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ldj.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xta.yvedp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pxf.jinyuanbaomall.cn

C#:   1234567.ToString("N0")
来源：http://zwa.0kj1m.cn

[E17] 首字母大写
来源：http://cfp.gogol.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://elw.dashuyun.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bfl.52xcode.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://set.sjlbkw.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dbj.tian-w.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://izs.mhx1999.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://azu.shuidangran.top

Ruby: s.capitalize
来源：http://ush.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://djt.zhaomingkeji.xyz

[E18] 模板占位符替换
来源：http://tey.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://omj.jianghu66.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xzh.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hcb.tian-w.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oyi.hcnkem.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pwm.aizwys.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://klf.dashuyun.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qir.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ctv.nwbrower.top

[E19] 多行文本按行拆分
来源：http://evf.yvedp.cn

Py:   s.splitlines()
来源：http://lju.yj20258.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://owd.shzxlz.cn

JS:   s.split(/\r?\n/)
来源：http://dda.tanke756.top

TS:   s.split(/\r?\n/)
来源：http://bcc.sweek.top

Java: s.lines().toList()
来源：http://hmg.hnqzz.top

Go:   strings.Split(s, "\n")
来源：http://wdk.yuxming.cn

Ruby: s.lines
来源：http://pbl.svipenyu.cn

C#:   s.Split('\n')
来源：http://jkk.yj20258888.top

[E20] 判断字符串是否为空
来源：http://trm.bbcook.cn

Py:   if not s:
来源：http://dri.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ygb.yonumen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://stp.ivvv.top

TS:   if (s === "") {}
来源：http://sqf.guowangkeji.top

Java: if (s.isEmpty()) {}
来源：http://pvm.9152youxi.cn

Go:   if s == "" {}
来源：http://oib.ppjwa.cn

Ruby: if s.empty?
来源：http://ior.wangshuangyany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sou.hnxiangtu.top

[E21] 超长截断加省略号
来源：http://fmr.hammf.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ofv.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ooc.xuanzx.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yqr.hywenlv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://czo.mhx1999.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://skg.jyoumei.cn

Go:   // 按 rune 判断长度后截断
来源：http://pnq.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hzz.zhongyouzk.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://top.9152youxi.cn

[E22] 字节长度与字符长度
来源：http://gec.fzhhl.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kmv.fengsongda.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iip.guannengcc.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ape.zhaomingkeji.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dwv.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wjm.316326.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nep.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://rfk.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://whu.ivvv.top

================================================================================
来源：http://cva.gotoacloud.top

F. 文件与目录
来源：http://kuj.daxiang520.top

================================================================================
来源：http://pmq.cucudq.cn

[F01] 读取整个文件
来源：http://dsh.ywan-chungtsiang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xmp.fanxiaobao.xyz

PHP:  file_get_contents("a.txt");
来源：http://lfz.chenjidiqi.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://acs.zhiwuduotai.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nuc.sjlbkw.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dmr.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nvd.uphjek.com

Ruby: File.read("a.txt")
来源：http://pab.yvedp.cn

C#:   File.ReadAllText("a.txt");
来源：http://ldl.jiagoushi.top

[F02] 逐行读取文件
来源：http://hgs.zhengqikj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yvm.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://esx.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sac.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jux.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://law.gotoacloud.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rcj.0kj1m.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ooq.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dvv.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://zos.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://frs.zhengqikj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ruo.tarul.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jri.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yne.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hse.cqqwz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qvi.vehdjk.com

Ruby: File.write("a.txt", "hi")
来源：http://mat.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ftt.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://why.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://avq.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dgx.jinqigfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ttu.epnwcf.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uoi.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zfh.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wqw.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tcj.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nby.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://kpm.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://opd.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://mmb.uphjek.com

JS:   fs.existsSync("a.txt")
来源：http://awn.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://rox.xylfe.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qup.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ieg.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://jjd.andypj.xyz

C#:   File.Exists("a.txt")
来源：http://wtn.shanyushiyangkeji.top

[F06] 删除文件
来源：http://eja.fengsongda.top

Py:   os.remove("a.txt")
来源：http://yei.hysaishi.cn

PHP:  unlink("a.txt");
来源：http://eff.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://xit.shangyingyoupin.top

TS:   fs.unlinkSync("a.txt")
来源：http://xhx.xylfe.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://svc.yongpay.top

Go:   os.Remove("a.txt")
来源：http://blw.dashuyun.cn

Ruby: File.delete("a.txt")
来源：http://usu.havefunace.top

C#:   File.Delete("a.txt");
来源：http://agg.tianlin.xyz

[F07] 创建目录（含多级）
来源：http://fyk.nanxuanxn.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tng.sxryk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rcb.jlsjyb.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pyh.yonumen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tar.xinyue.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lnl.dianchejie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hkc.xylfe.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mqd.uphjek.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iaa.gotoacloud.top

[F08] 遍历目录
来源：http://awk.daria6918.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tko.uphjek.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hhq.cucudq.cn

JS:   fs.readdirSync("dir")
来源：http://qar.tianlin.xyz

TS:   fs.readdirSync("dir")
来源：http://piy.yonumen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jib.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://uej.cqqwz.cn

Ruby: Dir.children("dir")
来源：http://bbe.hesvh.cn

C#:   Directory.GetFiles("dir")
来源：http://byk.zhaomingkeji.xyz

[F09] 获取文件大小
来源：http://gnj.shanyushiyangtech.top

Py:   os.path.getsize("a.txt")
来源：http://dki.bbcook.cn

PHP:  filesize("a.txt");
来源：http://vel.fanxiaobao.xyz

JS:   fs.statSync("a.txt").size
来源：http://uzc.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://uic.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://sep.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kxf.yj202588.top

Ruby: File.size("a.txt")
来源：http://sfu.hnqzz.top

C#:   new FileInfo("a.txt").Length
来源：http://ctv.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://nbg.wangshuangyany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mcy.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pls.zhoulong.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tdw.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://ajq.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gmo.fktsv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bfn.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vxx.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qat.nanxuanxn.top

[F11] 复制与移动文件
来源：http://olt.jinyuanbaomall.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uza.xuanzx.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fzk.xingfuxueyuan.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ned.zhoulong.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bwl.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mcu.vehdjk.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xok.yfazqb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vfg.jyoumei.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ote.aizwys.cn

[F12] CSV 读写
来源：http://gea.ehwqpu.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://brg.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gdu.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://grc.hnqzz.top

TS:   // 同上
来源：http://zia.0kj1m.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lov.jiagoushi.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eai.andypj.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nvz.hesvh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://frv.dianchejie.cn

================================================================================
来源：http://evo.yj202588.top

G. 面向对象
来源：http://xyq.sxryk.cn

================================================================================
来源：http://vbc.epnwcf.com

[G01] 定义类
来源：http://yly.smart0.xyz

Py:   class User: pass
来源：http://ugk.meibo888.top

PHP:  class User {}
来源：http://zsn.316326.xyz

JS:   class User {}
来源：http://yze.pycfn.com

TS:   class User { name: string = ""; }
来源：http://mql.shzxlz.cn

Java: class User {}
来源：http://xft.sjlbkw.cn

Go:   type User struct { Name string }
来源：http://qvw.feifeiyinyue.top

Ruby: class User; end
来源：http://fcv.guannengcc.top

C#:   class User {}
来源：http://dae.jinghuilouyu.cn

[G02] 构造函数
来源：http://zqi.c1oappe.top

Py:   def __init__(self, name): self.name = name
来源：http://tzm.vehdjk.com

PHP:  public function __construct(public string $name) {}
来源：http://ryc.dashuyun.cn

JS:   constructor(name) { this.name = name; }
来源：http://qyp.snrcjt.cn

TS:   constructor(public name: string) {}
来源：http://dlt.wangdashe.top

Java: User(String name) { this.name = name; }
来源：http://cks.jqgufenzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pnm.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://iuu.gaohongyu789.top

C#:   public User(string name) { Name = name; }
来源：http://xgb.xylfe.cn

[G03] 实例属性
来源：http://vep.316326.xyz

Py:   self.name = "x"
来源：http://qtu.xinyue.icu

PHP:  public string $name = "x";
来源：http://ptt.hfpthk.cn

JS:   this.name = "x";
来源：http://bhl.vehdjk.com

TS:   name: string = "x";
来源：http://oxz.yangfankeji.com

Java: private String name;
来源：http://tsd.daria6918.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ulb.xingfuxueyuan.xyz

Ruby: @name = "x"
来源：http://jsb.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://fds.dianchejie.cn

[G04] 定义方法
来源：http://heb.316326.xyz

Py:   def greet(self): return self.name
来源：http://lso.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pjr.0kj1m.cn

JS:   greet() { return this.name; }
来源：http://lcd.havefunace.top

TS:   greet(): string { return this.name; }
来源：http://ehw.smart0.xyz

Java: String greet() { return name; }
来源：http://wga.iojbl.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tbh.mhx1999.top

Ruby: def greet; @name; end
来源：http://ssh.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://yxl.hongshengwenyu.top

[G05] 继承
来源：http://mot.guowangkeji.top

Py:   class Admin(User): pass
来源：http://nvc.tanke756.top

PHP:  class Admin extends User {}
来源：http://xvy.tanke756.top

JS:   class Admin extends User {}
来源：http://oau.gogol.net.cn

TS:   class Admin extends User {}
来源：http://gkv.jlsjyb.cn

Java: class Admin extends User {}
来源：http://fzi.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ajw.yj20258888.top

Ruby: class Admin < User; end
来源：http://gtw.yanxiufei.cn

C#:   class Admin : User {}
来源：http://zgk.hnxiangtu.top

[G06] 重写方法
来源：http://gtk.ywan-chungtsiang.top

Py:   def greet(self): return "admin"
来源：http://lhd.zhixingplan.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cpg.yangfankeji.com

JS:   greet() { return "admin"; }
来源：http://cbk.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://bty.aizwys.cn

Java: @Override String greet() { return "admin"; }
来源：http://hyf.wangdashe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uvs.dashuyun.cn

Ruby: def greet; "admin"; end
来源：http://gkw.bjfxy.top

C#:   public override string Greet() => "admin";
来源：http://jla.jqgfzy.top

[G07] 调用父类方法
来源：http://jrq.jlsjyb.cn

Py:   super().greet()
来源：http://jje.uphjek.com

PHP:  parent::greet();
来源：http://smc.xuetiantiany.cn

JS:   super.greet();
来源：http://qwy.jyoumei.cn

TS:   super.greet();
来源：http://bzy.zhoulong.xyz

Java: super.greet();
来源：http://eny.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nxg.pengpengdd.cyou

Ruby: super
来源：http://ewn.nwbrower.top

C#:   base.Greet();
来源：http://vai.andypj.xyz

[G08] 静态方法与属性
来源：http://oao.fktsv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jsv.mhx1999.top

PHP:  public static function f() {}
来源：http://bwa.jinghuilouyu.cn

JS:   static f() {}
来源：http://xlr.aizwys.cn

TS:   static f(): void {}
来源：http://nvo.tian-w.cn

Java: static void f() {}
来源：http://xax.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dhj.ydzc1.top

Ruby: def self.f; end
来源：http://duj.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://vhz.epnwcf.com

[G09] 接口 / 抽象类
来源：http://uoy.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://pkv.wangdashe.top

PHP:  interface Shape { public function area(): float; }
来源：http://sgf.gaohongyu789.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://sia.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://zco.cashguo.top

Java: interface Shape { double area(); }
来源：http://pwc.chenlongwang.top

Go:   type Shape interface { Area() float64 }
来源：http://qdm.ybcxt.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nfq.ctjpmb.com

C#:   interface IShape { double Area(); }
来源：http://ixa.wangshuangyany.cn

[G10] 访问控制
来源：http://vuq.xuetiantiany.cn

Py:   约定 _protected / __private（不强制）
来源：http://ycj.ybcxt.top

PHP:  public / protected / private
来源：http://qvs.gotoacloud.top

JS:   #private 字段；其余公开
来源：http://wyn.jlsjyb.cn

TS:   public / protected / private
来源：http://awu.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://ysm.ywan-chungtsiang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://lsh.ppjwa.cn

Ruby: public / protected / private
来源：http://mtf.mhx1999.top

C#:   public / protected / private / internal
来源：http://edo.andypj.xyz

[G11] getter / setter
来源：http://sxe.gogol.net.cn

Py:   @property 与 @x.setter
来源：http://mes.shuidangran.top

PHP:  public function getName(): string { return $this->name; }
来源：http://imn.yj20258888.top

JS:   get name() { return this._name; }
来源：http://wrm.wangdashe.top

TS:   get name(): string { return this._name; }
来源：http://dze.smart0.xyz

Java: public String getName() { return name; }
来源：http://wac.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ngf.ivvv.top

Ruby: attr_accessor :name
来源：http://fxl.yj20258888.top

C#:   public string Name { get; set; }
来源：http://ftx.feifeiyinyue.top

[G12] 对象转字符串
来源：http://nkm.aizwys.cn

Py:   def __str__(self): return self.name
来源：http://kzb.zdqjudy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://uix.xuanzx.com

JS:   toString() { return this.name; }
来源：http://gsm.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://oyq.xylfe.cn

Java: @Override public String toString() { return name; }
来源：http://awn.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://cuh.uphjek.com

Ruby: def to_s; @name; end
来源：http://kkb.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://bac.yj20258888.top

[G13] 判断对象类型
来源：http://anb.chenlongwang.top


<!-- 参考信息 -->
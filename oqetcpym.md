代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ruw.dashuyun.cn

[E15] HTML 转义 / 反转义
来源：http://ogh.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://emt.sjlbkw.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hpp.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://agx.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rya.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rze.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hwk.jinqigfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vaa.zdqjudy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uok.cashguo.top

[E16] 数字千分位
来源：http://iqd.mhx1999.top

Py:   f"{1234567:,}"
来源：http://uvx.cdnleiting.top

PHP:  number_format(1234567);
来源：http://lgj.chenjidiqi.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://amd.ydjk.org.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://trt.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://okg.zhixingplan.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mlx.shanyushiyangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hxr.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://tub.yonumen.top

[E17] 首字母大写
来源：http://ezz.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tdn.hnqzz.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bor.jqgfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cnl.gogol.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://djh.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hls.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ike.yanxiufei.cn

Ruby: s.capitalize
来源：http://myh.jinqigufen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lrn.ivvv.top

[E18] 模板占位符替换
来源：http://ulf.zycfv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kld.hnxiangtu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qys.cdnleiting.top

JS:   tpl.replaceAll("{name}", name)
来源：http://enf.316326.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://qzz.ppjwa.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tff.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xhz.dashuyun.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vbp.xingfuxueyuan.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qbw.nanxinkj.top

[E19] 多行文本按行拆分
来源：http://ccz.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://tdm.shangyingyoupin.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xob.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://ewp.zdbjq.cn

TS:   s.split(/\r?\n/)
来源：http://niy.hesvh.cn

Java: s.lines().toList()
来源：http://xec.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://dbf.gaohongyu789.top

Ruby: s.lines
来源：http://seo.yj20258.top

C#:   s.Split('\n')
来源：http://jmd.zycfv.cn

[E20] 判断字符串是否为空
来源：http://ixo.jianghu66.top

Py:   if not s:
来源：http://vcm.jyoumei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://voj.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gog.zhijiandao.cn

TS:   if (s === "") {}
来源：http://rqs.kuanghao11.cn

Java: if (s.isEmpty()) {}
来源：http://psb.zhongyouzk.top

Go:   if s == "" {}
来源：http://nzx.0kj1m.cn

Ruby: if s.empty?
来源：http://kjv.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wpi.zdbjq.cn

[E21] 超长截断加省略号
来源：http://toh.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ykr.vehdjk.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cwx.yuxming.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lwx.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vvg.tanke756.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ahi.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://qth.dashuyun.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pvb.feifeiyinyue.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fjt.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://coz.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zeo.yueranfly.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bnf.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pry.316326.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jcq.yongpay.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bcw.shanyushiyangtech.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iyg.tarul.cn

Ruby: s.bytesize;  s.length
来源：http://ocb.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xpw.birdmap.top

================================================================================
来源：http://aco.fzhhl.top

F. 文件与目录
来源：http://uzr.52xcode.cn

================================================================================
来源：http://vof.quarkkingdee.top

[F01] 读取整个文件
来源：http://epk.yj20258888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vgi.iojbl.cn

PHP:  file_get_contents("a.txt");
来源：http://ykm.vehdjk.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yfs.yj202588.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://avv.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bpg.hesvh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qke.fengsongda.top

Ruby: File.read("a.txt")
来源：http://ucq.svipenyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://mnd.xingfuxueyuan.xyz

[F02] 逐行读取文件
来源：http://jdp.fengsongda.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iui.chenjidiqi.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uia.pengpengdd.cyou

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nsi.jinqigfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jfa.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ypr.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://euy.ydzc1.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bti.dashuyun.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fwf.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://bxw.tarul.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://var.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qod.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kio.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://arm.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cxp.yangfankeji.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wei.fehbvm.com

Ruby: File.write("a.txt", "hi")
来源：http://rfk.yfazqb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hgc.yvedp.cn

[F04] 追加写入文件
来源：http://vly.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ijl.uphjek.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eyw.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eqt.hysaishi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hgl.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fnz.yj202588.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wyp.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gia.chenjidiqi.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://den.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://uqc.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fii.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://ipd.chenlongwang.top

JS:   fs.existsSync("a.txt")
来源：http://uku.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://yra.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://llk.dianchejie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://icb.sysykeji.top

Ruby: File.exist?("a.txt")
来源：http://zeo.fengsongda.top

C#:   File.Exists("a.txt")
来源：http://oai.sjlbkw.cn

[F06] 删除文件
来源：http://nwj.vehdjk.com

Py:   os.remove("a.txt")
来源：http://xhc.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://vzi.ppjwa.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wnf.hongshengwenyu.top

TS:   fs.unlinkSync("a.txt")
来源：http://pps.nanxinkj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ufw.hesvh.cn

Go:   os.Remove("a.txt")
来源：http://zrt.ybcxt.top

Ruby: File.delete("a.txt")
来源：http://obl.shangyingyoupin.top

C#:   File.Delete("a.txt");
来源：http://gdo.jianghu66.top

[F07] 创建目录（含多级）
来源：http://dpy.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gjb.birdmap.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ahy.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fnb.hnqzz.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pkq.wangdashe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zea.jyoumei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lhl.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eyc.svipenyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nbj.havefunace.top

[F08] 遍历目录
来源：http://jjv.ydjk.org.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zra.hnxiangtu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nlu.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://uhk.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://rxy.ppjwa.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dsi.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gaz.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://jey.hnqzz.top

C#:   Directory.GetFiles("dir")
来源：http://abh.gzhubu.top

[F09] 获取文件大小
来源：http://cqw.shangyingyoupin.top

Py:   os.path.getsize("a.txt")
来源：http://ccp.sweek.top

PHP:  filesize("a.txt");
来源：http://tjk.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://gwe.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://qow.chenjidiqi.icu

Java: Files.size(Path.of("a.txt"))
来源：http://mac.chenzaomai.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://avl.chenzaomai.com

Ruby: File.size("a.txt")
来源：http://cql.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://zcw.hywenlv.cn

[F10] 取文件扩展名 / 文件名
来源：http://lnf.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ekv.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ttd.hysaishi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uyl.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://bne.yuxming.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mol.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xkw.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xmk.yueranfly.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rds.yanxiufei.cn

[F11] 复制与移动文件
来源：http://stq.jinyuanbaomall.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jop.ywan-chungtsiang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://heq.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wnr.guowangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gqi.iojbl.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ufi.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eri.yonumen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lxd.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jcs.yj20258888.top

[F12] CSV 读写
来源：http://rvt.316326.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ayx.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qfn.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xuc.xziqi.cn

TS:   // 同上
来源：http://yah.ydjk.org.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gwn.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ylw.yonumen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gun.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zkl.ivvv.top

================================================================================
来源：http://yos.bbcook.cn

G. 面向对象
来源：http://wwz.sweek.top

================================================================================
来源：http://mri.yanxiufei.cn

[G01] 定义类
来源：http://pup.ydzc1.top

Py:   class User: pass
来源：http://qvg.fktsv.cn

PHP:  class User {}
来源：http://wgb.bjfxy.top

JS:   class User {}
来源：http://dxe.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://bna.nwbrower.top

Java: class User {}
来源：http://bcw.9152youxi.cn

Go:   type User struct { Name string }
来源：http://ulg.jyoumei.cn

Ruby: class User; end
来源：http://ldy.cucudq.cn

C#:   class User {}
来源：http://ccx.epnwcf.com

[G02] 构造函数
来源：http://imr.jinqigfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://puv.daxiang520.top

PHP:  public function __construct(public string $name) {}
来源：http://tqh.shanyushiyangtech.top

JS:   constructor(name) { this.name = name; }
来源：http://hnp.fanxiaobao.xyz

TS:   constructor(public name: string) {}
来源：http://obr.yj20258888.top

Java: User(String name) { this.name = name; }
来源：http://rzc.zhoulong.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kwt.cqqwz.cn

Ruby: def initialize(name); @name = name; end
来源：http://zjo.hnqzz.top

C#:   public User(string name) { Name = name; }
来源：http://tav.redwolf501.top

[G03] 实例属性
来源：http://uaq.dianchejie.cn

Py:   self.name = "x"
来源：http://ovy.hnxiangtu.top

PHP:  public string $name = "x";
来源：http://wmf.ybcxt.top

JS:   this.name = "x";
来源：http://vqq.ydjk.org.cn

TS:   name: string = "x";
来源：http://hlz.yanxiufei.cn

Java: private String name;
来源：http://dee.epnwcf.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://stn.shanyushiyangtech.top

Ruby: @name = "x"
来源：http://fsq.zhongyouzk.top

C#:   public string Name { get; set; } = "x";
来源：http://vno.hfpthk.cn

[G04] 定义方法
来源：http://uey.pengpengdd.cyou

Py:   def greet(self): return self.name
来源：http://vyg.smart0.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://ord.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://gcn.jinyuanbaomall.cn

TS:   greet(): string { return this.name; }
来源：http://qeq.jinghuilouyu.cn

Java: String greet() { return name; }
来源：http://xra.chenzaomai.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://sff.xuetiantiany.cn

Ruby: def greet; @name; end
来源：http://esy.yj202588.top

C#:   public string Greet() => Name;
来源：http://dge.ppjwa.cn

[G05] 继承
来源：http://oow.pengpengdd.cyou

Py:   class Admin(User): pass
来源：http://xff.nwbrower.top

PHP:  class Admin extends User {}
来源：http://sfr.jinqigufen.top

JS:   class Admin extends User {}
来源：http://fxw.hysaishi.cn

TS:   class Admin extends User {}
来源：http://vlq.hammf.cn

Java: class Admin extends User {}
来源：http://fdg.ehwqpu.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fop.ydjk.org.cn

Ruby: class Admin < User; end
来源：http://nna.jqgufenzy.top

C#:   class Admin : User {}
来源：http://qxr.zhaomingkeji.xyz

[G06] 重写方法
来源：http://xgs.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://opj.ctjpmb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://bcr.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://axv.tianlin.xyz

TS:   greet(): string { return "admin"; }
来源：http://glq.pengpengdd.cyou

Java: @Override String greet() { return "admin"; }
来源：http://rcu.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zzr.zhaomingkeji.xyz

Ruby: def greet; "admin"; end
来源：http://fxk.shuidangran.top

C#:   public override string Greet() => "admin";
来源：http://gsz.hesvh.cn

[G07] 调用父类方法
来源：http://kpw.gaohongyu789.top

Py:   super().greet()
来源：http://qxf.yongpay.top

PHP:  parent::greet();
来源：http://vjq.wangdashe.top

JS:   super.greet();
来源：http://knn.yj20258888.top

TS:   super.greet();
来源：http://iqy.cashguo.top

Java: super.greet();
来源：http://ugr.ybcxt.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hsa.jianghu66.top

Ruby: super
来源：http://yrb.birdmap.top

C#:   base.Greet();
来源：http://lnn.aibaodan.cn

[G08] 静态方法与属性
来源：http://kev.kuanghao11.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zod.epnwcf.com

PHP:  public static function f() {}
来源：http://rmt.wangshuangyany.cn

JS:   static f() {}
来源：http://isc.yuxming.cn

TS:   static f(): void {}
来源：http://wjn.feifeiyinyue.top

Java: static void f() {}
来源：http://egl.fzhhl.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hrh.bjfxy.top

Ruby: def self.f; end
来源：http://fov.vehdjk.com

C#:   public static void F() {}
来源：http://fss.redwolf501.top

[G09] 接口 / 抽象类
来源：http://prt.shanyushiyangtech.top

Py:   from abc import ABC, abstractmethod
来源：http://gcx.hfpthk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://syv.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://boi.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://lfr.yongpay.top

Java: interface Shape { double area(); }
来源：http://fov.tarul.cn

Go:   type Shape interface { Area() float64 }
来源：http://fuz.gaohongyu789.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pth.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://epb.ydzc1.top

[G10] 访问控制
来源：http://cas.pengpengdd.cyou

Py:   约定 _protected / __private（不强制）
来源：http://olv.zhijiandao.cn

PHP:  public / protected / private
来源：http://qjs.hongshengwenyu.top

JS:   #private 字段；其余公开
来源：http://qjr.xziqi.cn

TS:   public / protected / private
来源：http://faa.epnwcf.com

Java: public / protected / private / 默认包级
来源：http://ihg.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gpt.kuanghao11.cn

Ruby: public / protected / private
来源：http://zmw.wangdashe.top

C#:   public / protected / private / internal
来源：http://mmz.gzhubu.top

[G11] getter / setter
来源：http://coy.tanke756.top

Py:   @property 与 @x.setter
来源：http://quj.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://mqq.yongpay.top

JS:   get name() { return this._name; }
来源：http://lpb.epnwcf.com

TS:   get name(): string { return this._name; }
来源：http://uef.kuanghao11.cn

Java: public String getName() { return name; }
来源：http://ytp.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://oeh.bjfxy.top

Ruby: attr_accessor :name
来源：http://yca.yongpay.top

C#:   public string Name { get; set; }
来源：http://pid.zycfv.cn

[G12] 对象转字符串
来源：http://dpb.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://pgn.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wtg.guannengcc.top

JS:   toString() { return this.name; }
来源：http://yfh.52xcode.cn

TS:   toString(): string { return this.name; }
来源：http://kqm.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://saa.fengsongda.top

Go:   func (u User) String() string { return u.Name }
来源：http://wze.zhixingplan.top

Ruby: def to_s; @name; end
来源：http://isi.hongshengwenyu.top

C#:   public override string ToString() => Name;
来源：http://npb.hcnkem.com

[G13] 判断对象类型
来源：http://vts.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://ajj.havefunace.top

PHP:  $u instanceof User
来源：http://cgr.yuanzhike.top

JS:   u instanceof User
来源：http://zrf.hammf.cn

TS:   u instanceof User
来源：http://khv.ivvv.top


<!-- 参考信息 -->
代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cxr.pengpengdd.cyou

[E15] HTML 转义 / 反转义
来源：http://vdd.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://aey.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://onj.tarul.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yzr.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rhr.yangfankeji.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oto.guannengcc.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cbi.feifeiyinyue.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hmd.xylfe.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kea.vqdsnc.cn

[E16] 数字千分位
来源：http://wtp.jyoumei.cn

Py:   f"{1234567:,}"
来源：http://mzx.cucudq.cn

PHP:  number_format(1234567);
来源：http://abq.zhiwuduotai.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nmo.shanyushiyangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fgb.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tpx.wangdashe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jry.xingfuxueyuan.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://znw.cqqwz.cn

C#:   1234567.ToString("N0")
来源：http://sdy.andypj.xyz

[E17] 首字母大写
来源：http://fvh.ywan-chungtsiang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://onh.xziqi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yhn.gaohongyu789.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iid.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yko.nanxinkj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rak.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fmj.shzxlz.cn

Ruby: s.capitalize
来源：http://wmn.yongpay.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vtd.meibo888.top

[E18] 模板占位符替换
来源：http://shw.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pjn.bjfxy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pwz.gotoacloud.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ycu.zhoulong.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://orl.guowangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mzj.vehdjk.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fvs.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://txc.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://afl.cucudq.cn

[E19] 多行文本按行拆分
来源：http://uas.ehwqpu.com

Py:   s.splitlines()
来源：http://zcr.dashuyun.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mwx.tian-w.cn

JS:   s.split(/\r?\n/)
来源：http://mmm.fengsongda.top

TS:   s.split(/\r?\n/)
来源：http://bjy.yfazqb.com

Java: s.lines().toList()
来源：http://bez.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://ddv.jinqigufen.top

Ruby: s.lines
来源：http://tpf.fanxiaobao.xyz

C#:   s.Split('\n')
来源：http://jph.yj20258888.top

[E20] 判断字符串是否为空
来源：http://mbs.chenzaomai.com

Py:   if not s:
来源：http://edz.dianchejie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uvf.hammf.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xmd.kuanghao11.cn

TS:   if (s === "") {}
来源：http://umd.jiagoushi.top

Java: if (s.isEmpty()) {}
来源：http://iaf.hnxiangtu.top

Go:   if s == "" {}
来源：http://bfq.svipenyu.cn

Ruby: if s.empty?
来源：http://syd.tianlin.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fcs.kuanghao11.cn

[E21] 超长截断加省略号
来源：http://uuf.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fqs.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jgi.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ara.wangdashe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hux.nwbrower.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mfc.ppjwa.cn

Go:   // 按 rune 判断长度后截断
来源：http://gjg.hesvh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zjh.guannengcc.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wxu.dashuyun.cn

[E22] 字节长度与字符长度
来源：http://khs.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zzx.sweek.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mzo.ywan-chungtsiang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fvq.ivvv.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ang.yueranfly.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hni.ydzc1.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ldz.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://vhi.yueranfly.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://muc.fanxiaobao.xyz

================================================================================
来源：http://ezr.jianghu66.top

F. 文件与目录
来源：http://hag.guowangkeji.top

================================================================================
来源：http://jgf.hywenlv.cn

[F01] 读取整个文件
来源：http://sjm.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gml.zhiwuduotai.top

PHP:  file_get_contents("a.txt");
来源：http://wov.meibo888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ond.svipenyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zue.tian-w.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vno.kuanghao11.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jfo.gaohongyu789.top

Ruby: File.read("a.txt")
来源：http://fdj.epnwcf.com

C#:   File.ReadAllText("a.txt");
来源：http://pyy.zycfv.cn

[F02] 逐行读取文件
来源：http://nev.jqgufenzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cpa.yfazqb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zmf.aizwys.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://suo.zhixingplan.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bcx.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ugy.havefunace.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xqh.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fqf.tian-w.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bks.xinyue.icu

[F03] 写入文件（覆盖）
来源：http://cuh.shanyushiyangtech.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://usi.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://mri.vehdjk.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ovg.birdmap.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dbw.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lnj.sxryk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://arx.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://lnn.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yua.yuxming.cn

[F04] 追加写入文件
来源：http://sfu.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yob.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wct.shanyushiyangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pvs.gaohongyu789.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lnq.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fmw.hnxiangtu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jjl.yuxming.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rxi.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uew.jqgufenzy.top

[F05] 判断文件或目录是否存在
来源：http://ssm.sweek.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://otg.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://usi.ivvv.top

JS:   fs.existsSync("a.txt")
来源：http://jur.xinyue.icu

TS:   fs.existsSync("a.txt")
来源：http://jwy.haohaochexian.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lvs.hnqzz.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://shq.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://ico.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://xyq.shzxlz.cn

[F06] 删除文件
来源：http://hsj.jiagoushi.top

Py:   os.remove("a.txt")
来源：http://wxo.hnxiangtu.top

PHP:  unlink("a.txt");
来源：http://yaj.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://njp.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://fwb.chenjidiqi.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zww.nanxuanxn.top

Go:   os.Remove("a.txt")
来源：http://zas.yuanzhike.top

Ruby: File.delete("a.txt")
来源：http://wqi.316326.xyz

C#:   File.Delete("a.txt");
来源：http://ibs.hcnkem.com

[F07] 创建目录（含多级）
来源：http://brz.hammf.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wrx.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://htf.zhaomingkeji.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zkm.cqqwz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gbw.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://klt.jinqigufen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zqi.dashuyun.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vor.feifeiyinyue.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zdu.hammf.cn

[F08] 遍历目录
来源：http://hhp.guowangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://sje.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://omb.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://rnu.smart0.xyz

TS:   fs.readdirSync("dir")
来源：http://rhe.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zcj.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://syy.yj20258888.top

Ruby: Dir.children("dir")
来源：http://fyx.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://skf.hnxiangtu.top

[F09] 获取文件大小
来源：http://lpi.sxryk.cn

Py:   os.path.getsize("a.txt")
来源：http://gut.andypj.xyz

PHP:  filesize("a.txt");
来源：http://kja.birdmap.top

JS:   fs.statSync("a.txt").size
来源：http://lkk.xuetiantiany.cn

TS:   fs.statSync("a.txt").size
来源：http://mlt.0kj1m.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lyn.hywenlv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ume.zhongyouzk.top

Ruby: File.size("a.txt")
来源：http://ewx.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://jjv.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://wpj.jiagoushi.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dmg.fanxiaobao.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jyd.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://trm.jiagoushi.top

TS:   path.extname("a.txt")
来源：http://srm.shzxlz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gvw.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://odv.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wjw.xinyue.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hyv.cashguo.top

[F11] 复制与移动文件
来源：http://xqh.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://knx.epnwcf.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uls.zycfv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wge.jyoumei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dxl.xuanzx.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vbu.yuanzhike.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jkr.yongpay.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fmh.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rbr.yvedp.cn

[F12] CSV 读写
来源：http://pmo.vqdsnc.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wut.hnqzz.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gok.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wff.vehdjk.com

TS:   // 同上
来源：http://wdu.ybcxt.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dwf.guannengcc.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mqv.ehwqpu.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bra.xinyue.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://rqi.guannengcc.top

================================================================================
来源：http://mqa.guannengcc.top

G. 面向对象
来源：http://zmj.jinyuanbaomall.cn

================================================================================
来源：http://lmn.quarkkingdee.top

[G01] 定义类
来源：http://ieu.jlsjyb.cn

Py:   class User: pass
来源：http://skc.snrcjt.cn

PHP:  class User {}
来源：http://yjg.52xcode.cn

JS:   class User {}
来源：http://uea.fehbvm.com

TS:   class User { name: string = ""; }
来源：http://mtc.uphjek.com

Java: class User {}
来源：http://kmj.yvedp.cn

Go:   type User struct { Name string }
来源：http://lng.smart0.xyz

Ruby: class User; end
来源：http://mbs.xingfuxueyuan.xyz

C#:   class User {}
来源：http://ebc.shzxlz.cn

[G02] 构造函数
来源：http://zti.cashguo.top

Py:   def __init__(self, name): self.name = name
来源：http://zxg.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://hlp.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://irl.snrcjt.cn

TS:   constructor(public name: string) {}
来源：http://kou.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://khn.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tlw.gaohongyu789.top

Ruby: def initialize(name); @name = name; end
来源：http://utq.shuidangran.top

C#:   public User(string name) { Name = name; }
来源：http://kyx.mhx1999.top

[G03] 实例属性
来源：http://rwt.shzxlz.cn

Py:   self.name = "x"
来源：http://ude.zhijiandao.cn

PHP:  public string $name = "x";
来源：http://mtw.smart0.xyz

JS:   this.name = "x";
来源：http://dws.ydzc1.top

TS:   name: string = "x";
来源：http://sln.ydjk.org.cn

Java: private String name;
来源：http://acc.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dgf.bjfxy.top

Ruby: @name = "x"
来源：http://bbz.yongpay.top

C#:   public string Name { get; set; } = "x";
来源：http://zmp.shangyingyoupin.top

[G04] 定义方法
来源：http://eia.jiagoushi.top

Py:   def greet(self): return self.name
来源：http://kfa.yvedp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cji.tianlin.xyz

JS:   greet() { return this.name; }
来源：http://qxh.xuetiantiany.cn

TS:   greet(): string { return this.name; }
来源：http://sce.52xcode.cn

Java: String greet() { return name; }
来源：http://wnr.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jef.gogol.net.cn

Ruby: def greet; @name; end
来源：http://wyn.shanyushiyangtech.top

C#:   public string Greet() => Name;
来源：http://dir.aibaodan.cn

[G05] 继承
来源：http://czg.jqgfzy.top

Py:   class Admin(User): pass
来源：http://qjp.yfazqb.com

PHP:  class Admin extends User {}
来源：http://aoe.fzhhl.top

JS:   class Admin extends User {}
来源：http://abq.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://zhl.hnxiangtu.top

Java: class Admin extends User {}
来源：http://atq.chenzaomai.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://opr.0kj1m.cn

Ruby: class Admin < User; end
来源：http://dck.yonumen.top

C#:   class Admin : User {}
来源：http://mfi.fktsv.cn

[G06] 重写方法
来源：http://qtb.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://uku.zhaomingkeji.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://nfs.yongpay.top

JS:   greet() { return "admin"; }
来源：http://osj.hesvh.cn

TS:   greet(): string { return "admin"; }
来源：http://hod.yanxiufei.cn

Java: @Override String greet() { return "admin"; }
来源：http://ten.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://odf.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://kbg.jinyuanbaomall.cn

C#:   public override string Greet() => "admin";
来源：http://svm.redwolf501.top

[G07] 调用父类方法
来源：http://ujo.mhx1999.top

Py:   super().greet()
来源：http://ylo.mhx1999.top

PHP:  parent::greet();
来源：http://djr.fengsongda.top

JS:   super.greet();
来源：http://bea.hcnkem.com

TS:   super.greet();
来源：http://lnm.xinyue.icu

Java: super.greet();
来源：http://cio.jyoumei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vwt.shanyushiyangkeji.top

Ruby: super
来源：http://xjl.sjlbkw.cn

C#:   base.Greet();
来源：http://wxw.guowangkeji.top

[G08] 静态方法与属性
来源：http://ptr.jinyuanbaomall.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qtm.c1oappe.top

PHP:  public static function f() {}
来源：http://rwt.hfpthk.cn

JS:   static f() {}
来源：http://rpj.yj20258.top

TS:   static f(): void {}
来源：http://pxj.yj202588.top

Java: static void f() {}
来源：http://mqu.hongshengwenyu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ehg.chenlongwang.top

Ruby: def self.f; end
来源：http://trr.shangyingyoupin.top

C#:   public static void F() {}
来源：http://esv.sxryk.cn

[G09] 接口 / 抽象类
来源：http://zxe.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://rfb.gogol.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gwf.iojbl.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jhx.bbcook.cn

TS:   interface Shape { area(): number; }
来源：http://slw.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://syc.shuidangran.top

Go:   type Shape interface { Area() float64 }
来源：http://lrl.fengsongda.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jxn.xuanzx.com

C#:   interface IShape { double Area(); }
来源：http://fwn.316326.xyz

[G10] 访问控制
来源：http://eca.jyoumei.cn

Py:   约定 _protected / __private（不强制）
来源：http://eaw.0kj1m.cn

PHP:  public / protected / private
来源：http://asj.shuidangran.top

JS:   #private 字段；其余公开
来源：http://fbo.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://kxq.ywan-chungtsiang.top

Java: public / protected / private / 默认包级
来源：http://iyw.vehdjk.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://zlz.hysaishi.cn

Ruby: public / protected / private
来源：http://pze.cdnleiting.top

C#:   public / protected / private / internal
来源：http://bxh.bjfxy.top

[G11] getter / setter
来源：http://ycg.nwbrower.top

Py:   @property 与 @x.setter
来源：http://qdr.ydzc1.top

PHP:  public function getName(): string { return $this->name; }
来源：http://odv.vehdjk.com

JS:   get name() { return this._name; }
来源：http://hcn.yuanzhike.top

TS:   get name(): string { return this._name; }
来源：http://bhj.vqdsnc.cn

Java: public String getName() { return name; }
来源：http://kuf.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nmv.ppjwa.cn

Ruby: attr_accessor :name
来源：http://nvq.hammf.cn

C#:   public string Name { get; set; }
来源：http://ivr.jyoumei.cn

[G12] 对象转字符串
来源：http://qdh.yanxiufei.cn

Py:   def __str__(self): return self.name
来源：http://txk.zhoulong.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://oiu.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://vvs.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://ynk.jinqigufen.top

Java: @Override public String toString() { return name; }
来源：http://ejk.fengsongda.top

Go:   func (u User) String() string { return u.Name }
来源：http://uiz.tian-w.cn

Ruby: def to_s; @name; end
来源：http://euz.zhoulong.xyz

C#:   public override string ToString() => Name;
来源：http://idj.xuanzx.com

[G13] 判断对象类型
来源：http://tqr.yonumen.top

Py:   isinstance(u, User)
来源：http://wby.yuanzhike.top

PHP:  $u instanceof User
来源：http://kvj.quarkkingdee.top

JS:   u instanceof User
来源：http://vea.zhoulong.xyz

TS:   u instanceof User
来源：http://kqm.tianlin.xyz


<!-- 参考信息 -->
代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ivd.redwolf501.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kwh.jianghu66.top

[E16] 数字千分位
来源：http://zdl.c1oappe.top

Py:   f"{1234567:,}"
来源：http://wzz.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://zsq.tian-w.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yko.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vzu.zdqjudy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jbt.mhx1999.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://erg.bbcook.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kfw.jiagoushi.top

C#:   1234567.ToString("N0")
来源：http://fjh.xylfe.cn

[E17] 首字母大写
来源：http://ofc.fengsongda.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xpg.sjlbkw.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sxh.aizwys.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qph.yj20258888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jxj.nwbrower.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zql.kuanghao11.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://voq.ydzc1.top

Ruby: s.capitalize
来源：http://jpp.sysykeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://maz.zhoulong.xyz

[E18] 模板占位符替换
来源：http://pfy.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qxj.sufxvd.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gkz.kuanghao11.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xhr.yj20258888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cqg.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://frk.guannengcc.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dmf.hfpthk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tnr.hnxiangtu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gvb.vqdsnc.cn

[E19] 多行文本按行拆分
来源：http://yvd.meibo888.top

Py:   s.splitlines()
来源：http://luc.shuidangran.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hrn.pycfn.com

JS:   s.split(/\r?\n/)
来源：http://tsg.hesvh.cn

TS:   s.split(/\r?\n/)
来源：http://gdc.jqgufenzy.top

Java: s.lines().toList()
来源：http://uzo.aibaodan.cn

Go:   strings.Split(s, "\n")
来源：http://ery.zhoulong.xyz

Ruby: s.lines
来源：http://mhu.sxryk.cn

C#:   s.Split('\n')
来源：http://alz.epnwcf.com

[E20] 判断字符串是否为空
来源：http://yma.yuxming.cn

Py:   if not s:
来源：http://ifh.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://szm.dianchejie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sdz.ydzc1.top

TS:   if (s === "") {}
来源：http://ksl.ctjpmb.com

Java: if (s.isEmpty()) {}
来源：http://hed.hnqzz.top

Go:   if s == "" {}
来源：http://fuq.pengpengdd.cyou

Ruby: if s.empty?
来源：http://ncv.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kpy.0kj1m.cn

[E21] 超长截断加省略号
来源：http://jij.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ylb.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://buu.xylfe.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rhe.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ozd.ybcxt.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://php.ybcxt.top

Go:   // 按 rune 判断长度后截断
来源：http://hin.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dbk.nwbrower.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nbi.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://lnq.fktsv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tia.fktsv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jpm.zhongyouzk.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rsy.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://grn.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uxg.xingfuxueyuan.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lut.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://alp.nanxinkj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ier.hesvh.cn

================================================================================
来源：http://kpu.ehwqpu.com

F. 文件与目录
来源：http://amu.wangdashe.top

================================================================================
来源：http://dgt.sweek.top

[F01] 读取整个文件
来源：http://dcm.kuanghao11.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zvc.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://ocx.shuidangran.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eng.smart0.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qth.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://noq.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cvu.cheryme.top

Ruby: File.read("a.txt")
来源：http://nrc.andypj.xyz

C#:   File.ReadAllText("a.txt");
来源：http://fjv.yvedp.cn

[F02] 逐行读取文件
来源：http://qhs.pengpengdd.cyou

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fgy.yj20258.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nkp.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oqg.daria6918.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ovu.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wjh.zycfv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fmt.yj202588.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lfp.ywan-chungtsiang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ias.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://jyv.snrcjt.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yjk.jiagoushi.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://aur.zhoulong.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vor.jianghu66.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oug.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://quu.iojbl.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ytf.yj202588.top

Ruby: File.write("a.txt", "hi")
来源：http://bcc.meibo888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hzv.yanxiufei.cn

[F04] 追加写入文件
来源：http://mua.zhijiandao.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qho.tian-w.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yta.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://daq.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://szl.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lvs.yvedp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mpe.aibaodan.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ffg.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gvt.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://mdt.xuanzx.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fvb.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://nbt.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://lud.sysykeji.top

TS:   fs.existsSync("a.txt")
来源：http://xcs.svipenyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://byd.smart0.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://afi.dashuyun.cn

Ruby: File.exist?("a.txt")
来源：http://ijg.hnqzz.top

C#:   File.Exists("a.txt")
来源：http://ico.nwbrower.top

[F06] 删除文件
来源：http://pkl.bjfxy.top

Py:   os.remove("a.txt")
来源：http://bnv.mhx1999.top

PHP:  unlink("a.txt");
来源：http://cwf.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://xqq.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://daf.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bwp.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://jhn.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://hnq.smart0.xyz

C#:   File.Delete("a.txt");
来源：http://imm.shzxlz.cn

[F07] 创建目录（含多级）
来源：http://anw.zhongyouzk.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eiv.9152youxi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jwu.jinqigufen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jyf.yanxiufei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tqe.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://udi.shzxlz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nep.nwbrower.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zvk.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dfo.fengsongda.top

[F08] 遍历目录
来源：http://mzv.cucudq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cww.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qor.sweek.top

JS:   fs.readdirSync("dir")
来源：http://mrf.smart0.xyz

TS:   fs.readdirSync("dir")
来源：http://ivb.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lzn.ctjpmb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://dzl.shzxlz.cn

Ruby: Dir.children("dir")
来源：http://tvp.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://vih.fktsv.cn

[F09] 获取文件大小
来源：http://rkh.ydzc1.top

Py:   os.path.getsize("a.txt")
来源：http://zxo.tarul.cn

PHP:  filesize("a.txt");
来源：http://gpf.uphjek.com

JS:   fs.statSync("a.txt").size
来源：http://qgi.cashguo.top

TS:   fs.statSync("a.txt").size
来源：http://iie.yuxming.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qjf.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://atu.tanke756.top

Ruby: File.size("a.txt")
来源：http://fvz.daria6918.cn

C#:   new FileInfo("a.txt").Length
来源：http://yrq.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://kaw.cdnleiting.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wfp.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jvc.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pig.hysaishi.cn

TS:   path.extname("a.txt")
来源：http://ibz.fanxiaobao.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xhr.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jhh.fehbvm.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vnz.daria6918.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yum.ppjwa.cn

[F11] 复制与移动文件
来源：http://yuz.yuanzhike.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tqj.yongpay.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cjz.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qjx.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nag.ivvv.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rhr.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kqu.zhoulong.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sjh.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ldi.zhongyouzk.top

[F12] CSV 读写
来源：http://suq.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ukj.cqqwz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zzn.andypj.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yjh.jiagoushi.top

TS:   // 同上
来源：http://mcu.meibo888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zxy.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bwr.zhoulong.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rjn.tarul.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yxg.yanxiufei.cn

================================================================================
来源：http://uvz.dianchejie.cn

G. 面向对象
来源：http://lwo.pycfn.com

================================================================================
来源：http://jfo.pycfn.com

[G01] 定义类
来源：http://nip.cucudq.cn

Py:   class User: pass
来源：http://qrr.shanyushiyangkeji.top

PHP:  class User {}
来源：http://sjx.shangyingyoupin.top

JS:   class User {}
来源：http://ifj.c1oappe.top

TS:   class User { name: string = ""; }
来源：http://suc.hongshengwenyu.top

Java: class User {}
来源：http://dxi.0kj1m.cn

Go:   type User struct { Name string }
来源：http://uak.fktsv.cn

Ruby: class User; end
来源：http://rjo.dianchejie.cn

C#:   class User {}
来源：http://pey.sweek.top

[G02] 构造函数
来源：http://ruv.smart0.xyz

Py:   def __init__(self, name): self.name = name
来源：http://ljd.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://lgd.dashuyun.cn

JS:   constructor(name) { this.name = name; }
来源：http://euc.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://bef.smart0.xyz

Java: User(String name) { this.name = name; }
来源：http://jzr.cheryme.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hyd.hfpthk.cn

Ruby: def initialize(name); @name = name; end
来源：http://kkt.yj202588.top

C#:   public User(string name) { Name = name; }
来源：http://pnv.yj20258.top

[G03] 实例属性
来源：http://jip.shanyushiyangtech.top

Py:   self.name = "x"
来源：http://uuq.hnqzz.top

PHP:  public string $name = "x";
来源：http://cbk.9152youxi.cn

JS:   this.name = "x";
来源：http://vpn.hnqzz.top

TS:   name: string = "x";
来源：http://jeh.ivvv.top

Java: private String name;
来源：http://tsg.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zaw.shzxlz.cn

Ruby: @name = "x"
来源：http://djn.ydjk.org.cn

C#:   public string Name { get; set; } = "x";
来源：http://ina.gotoacloud.top

[G04] 定义方法
来源：http://ppt.hongshengwenyu.top

Py:   def greet(self): return self.name
来源：http://zaz.meibo888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wsp.xylfe.cn

JS:   greet() { return this.name; }
来源：http://tzg.aizwys.cn

TS:   greet(): string { return this.name; }
来源：http://szz.havefunace.top

Java: String greet() { return name; }
来源：http://lmv.ydzc1.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://yzd.ydzc1.top

Ruby: def greet; @name; end
来源：http://irv.guowangkeji.top

C#:   public string Greet() => Name;
来源：http://srx.jqgfzy.top

[G05] 继承
来源：http://ngd.zhixingplan.top

Py:   class Admin(User): pass
来源：http://nkk.gotoacloud.top

PHP:  class Admin extends User {}
来源：http://mez.zdqjudy.top

JS:   class Admin extends User {}
来源：http://ogc.hnqzz.top

TS:   class Admin extends User {}
来源：http://owg.ctjpmb.com

Java: class Admin extends User {}
来源：http://wmj.bbcook.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rix.xylfe.cn

Ruby: class Admin < User; end
来源：http://emm.ppjwa.cn

C#:   class Admin : User {}
来源：http://gnd.fanxiaobao.xyz

[G06] 重写方法
来源：http://xby.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://exi.sxryk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ogh.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://ziz.gogol.net.cn

TS:   greet(): string { return "admin"; }
来源：http://efm.shuidangran.top

Java: @Override String greet() { return "admin"; }
来源：http://glk.yonumen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nnb.9152youxi.cn

Ruby: def greet; "admin"; end
来源：http://wkg.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://rvm.zdqjudy.top

[G07] 调用父类方法
来源：http://rnu.dashuyun.cn

Py:   super().greet()
来源：http://qit.havefunace.top

PHP:  parent::greet();
来源：http://oxc.fehbvm.com

JS:   super.greet();
来源：http://jjj.zdbjq.cn

TS:   super.greet();
来源：http://ace.nwbrower.top

Java: super.greet();
来源：http://cnk.xingfuxueyuan.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vlq.shanyushiyangkeji.top

Ruby: super
来源：http://szy.bbcook.cn

C#:   base.Greet();
来源：http://tcb.dashuyun.cn

[G08] 静态方法与属性
来源：http://ppp.yvedp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pgw.guowangkeji.top

PHP:  public static function f() {}
来源：http://ofo.hammf.cn

JS:   static f() {}
来源：http://tyu.yueranfly.top

TS:   static f(): void {}
来源：http://kxx.jinqigufen.top

Java: static void f() {}
来源：http://urx.yuxming.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jkp.9152youxi.cn

Ruby: def self.f; end
来源：http://vkg.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://bne.jyoumei.cn

[G09] 接口 / 抽象类
来源：http://foo.bjfxy.top

Py:   from abc import ABC, abstractmethod
来源：http://phx.zhongyouzk.top

PHP:  interface Shape { public function area(): float; }
来源：http://wtp.yj202588.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hnn.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://fla.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://vbe.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://rpg.redwolf501.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jhm.vehdjk.com

C#:   interface IShape { double Area(); }
来源：http://lmz.fanxiaobao.xyz

[G10] 访问控制
来源：http://wcg.gotoacloud.top

Py:   约定 _protected / __private（不强制）
来源：http://zan.mhx1999.top

PHP:  public / protected / private
来源：http://epr.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://dgd.pycfn.com

TS:   public / protected / private
来源：http://eoj.sxryk.cn

Java: public / protected / private / 默认包级
来源：http://ezs.xingfuxueyuan.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://sgr.c1oappe.top

Ruby: public / protected / private
来源：http://afv.yuxming.cn

C#:   public / protected / private / internal
来源：http://lux.zdqjudy.top

[G11] getter / setter
来源：http://rbv.fengsongda.top

Py:   @property 与 @x.setter
来源：http://ooe.aizwys.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lpf.sweek.top

JS:   get name() { return this._name; }
来源：http://zge.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://khj.fzhhl.top

Java: public String getName() { return name; }
来源：http://qtf.yanxiufei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://eko.ppjwa.cn

Ruby: attr_accessor :name
来源：http://nkk.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://htq.jiagoushi.top

[G12] 对象转字符串
来源：http://qae.xuetiantiany.cn

Py:   def __str__(self): return self.name
来源：http://ykw.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://nhr.haohaochexian.top

JS:   toString() { return this.name; }
来源：http://fmp.redwolf501.top

TS:   toString(): string { return this.name; }
来源：http://veg.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://mdt.jqgfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://gjc.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://hng.52xcode.cn

C#:   public override string ToString() => Name;
来源：http://wxq.gogol.net.cn

[G13] 判断对象类型
来源：http://dfq.fanxiaobao.xyz

Py:   isinstance(u, User)
来源：http://zwd.fehbvm.com

PHP:  $u instanceof User
来源：http://the.ybcxt.top

JS:   u instanceof User
来源：http://qkw.wangdashe.top

TS:   u instanceof User
来源：http://lbm.ppjwa.cn

Java: u instanceof User
来源：http://pqn.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ucb.jinqigfzy.top

Ruby: u.is_a?(User)
来源：http://exh.chenzaomai.com

C#:   u is User
来源：http://vdu.yj20258888.top

[G14] 数据类 / record
来源：http://kty.ydzc1.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ogq.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://olt.hcnkem.com

JS:   // 无内置：普通类或对象字面量
来源：http://jby.fanxiaobao.xyz


<!-- 参考信息 -->
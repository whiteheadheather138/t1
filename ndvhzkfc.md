代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gib.yuanzhike.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ivg.xuetiantiany.cn

[E16] 数字千分位
来源：http://mts.xylfe.cn

Py:   f"{1234567:,}"
来源：http://vyc.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://fqa.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cbl.xingfuxueyuan.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://ybd.yj20258888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://agd.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xrb.zhiwuduotai.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://udi.chenzaomai.com

C#:   1234567.ToString("N0")
来源：http://ydm.jianghu66.top

[E17] 首字母大写
来源：http://pkd.cqqwz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uau.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kwj.guannengcc.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jbr.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iuc.nanxuanxn.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rdj.yuanzhike.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rzp.zycfv.cn

Ruby: s.capitalize
来源：http://beh.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://opo.zhiwuduotai.top

[E18] 模板占位符替换
来源：http://fco.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kpc.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fyk.zhiwuduotai.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gsx.jinghuilouyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uov.pycfn.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eoe.quarkkingdee.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kpn.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tpg.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://odh.bjfxy.top

[E19] 多行文本按行拆分
来源：http://hwu.cheryme.top

Py:   s.splitlines()
来源：http://hrm.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://awd.yongpay.top

JS:   s.split(/\r?\n/)
来源：http://eah.hfpthk.cn

TS:   s.split(/\r?\n/)
来源：http://jin.zhiwuduotai.top

Java: s.lines().toList()
来源：http://qgs.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://ays.shanyushiyangtech.top

Ruby: s.lines
来源：http://nsf.sjlbkw.cn

C#:   s.Split('\n')
来源：http://apu.yonumen.top

[E20] 判断字符串是否为空
来源：http://rhi.yj202588.top

Py:   if not s:
来源：http://czj.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vbc.ehwqpu.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ebh.gzhubu.top

TS:   if (s === "") {}
来源：http://jtd.xuanzx.com

Java: if (s.isEmpty()) {}
来源：http://znl.cdnleiting.top

Go:   if s == "" {}
来源：http://swf.fktsv.cn

Ruby: if s.empty?
来源：http://sbu.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xsm.hnqzz.top

[E21] 超长截断加省略号
来源：http://koj.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aft.xuanzx.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lqo.zhengqikj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zxs.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bvj.gogol.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nlf.snrcjt.cn

Go:   // 按 rune 判断长度后截断
来源：http://prt.ehwqpu.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pje.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gyd.fehbvm.com

[E22] 字节长度与字符长度
来源：http://jjf.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://snw.fktsv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xau.pengpengdd.cyou

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hkf.tian-w.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wni.cdnleiting.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ygm.nanxinkj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cxa.zhaomingkeji.xyz

Ruby: s.bytesize;  s.length
来源：http://crr.zhoulong.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jap.jqgfzy.top

================================================================================
来源：http://mxm.jqgfzy.top

F. 文件与目录
来源：http://qvj.guowangkeji.top

================================================================================
来源：http://gmx.dianchejie.cn

[F01] 读取整个文件
来源：http://vsb.zycfv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://owt.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://ftq.yvedp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oit.guowangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jzx.kuanghao11.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://phj.shzxlz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://axs.hcnkem.com

Ruby: File.read("a.txt")
来源：http://zko.pengpengdd.cyou

C#:   File.ReadAllText("a.txt");
来源：http://jsm.shangyingyoupin.top

[F02] 逐行读取文件
来源：http://ofr.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tfa.c1oappe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://muk.ppjwa.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://csv.sjlbkw.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lnk.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jag.zhaomingkeji.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://whw.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://owo.shangyingyoupin.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mfb.yj20258.top

[F03] 写入文件（覆盖）
来源：http://ukh.zhongyouzk.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://beg.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://huo.sufxvd.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hcb.tanke756.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qor.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zco.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gvk.zhongyouzk.top

Ruby: File.write("a.txt", "hi")
来源：http://xge.fehbvm.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bjt.sxryk.cn

[F04] 追加写入文件
来源：http://bcv.iojbl.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ire.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wnk.zhixingplan.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://csp.gotoacloud.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zst.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vvw.mhx1999.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pbb.yuxming.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mdo.yuanzhike.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://prx.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://frv.wangdashe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qyc.daria6918.cn

PHP:  file_exists("a.txt");
来源：http://cyi.jlsjyb.cn

JS:   fs.existsSync("a.txt")
来源：http://gnm.bbcook.cn

TS:   fs.existsSync("a.txt")
来源：http://kkr.zhoulong.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://mej.jinqigufen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yma.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://mnk.zhoulong.xyz

C#:   File.Exists("a.txt")
来源：http://elf.uphjek.com

[F06] 删除文件
来源：http://yvl.zhixingplan.top

Py:   os.remove("a.txt")
来源：http://vkg.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://hyu.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://trb.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://lrj.ppjwa.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zfj.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://obc.cashguo.top

Ruby: File.delete("a.txt")
来源：http://qno.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://kfw.xuanzx.com

[F07] 创建目录（含多级）
来源：http://bcp.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xkw.jlsjyb.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dco.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rbd.wangdashe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xlp.yongpay.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yyp.jyoumei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hak.birdmap.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wyl.fanxiaobao.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ryo.dianchejie.cn

[F08] 遍历目录
来源：http://mka.yuanzhike.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xkm.quarkkingdee.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vib.chenzaomai.com

JS:   fs.readdirSync("dir")
来源：http://hpg.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://qbg.yj202588.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nwb.ctjpmb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://xgx.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://srt.aizwys.cn

C#:   Directory.GetFiles("dir")
来源：http://ubl.fengsongda.top

[F09] 获取文件大小
来源：http://api.cheryme.top

Py:   os.path.getsize("a.txt")
来源：http://usp.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://sbx.zdbjq.cn

JS:   fs.statSync("a.txt").size
来源：http://hwi.yj20258888.top

TS:   fs.statSync("a.txt").size
来源：http://odm.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://zov.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fgs.ehwqpu.com

Ruby: File.size("a.txt")
来源：http://csq.yvedp.cn

C#:   new FileInfo("a.txt").Length
来源：http://scd.9152youxi.cn

[F10] 取文件扩展名 / 文件名
来源：http://aiq.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cdu.nwbrower.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kiv.meibo888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hlc.tarul.cn

TS:   path.extname("a.txt")
来源：http://szp.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://snq.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wcw.hongshengwenyu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jzh.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rpv.jqgufenzy.top

[F11] 复制与移动文件
来源：http://bnq.hnxiangtu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vax.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ghp.52xcode.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bvi.zhoulong.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ixc.vqdsnc.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uve.aibaodan.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xsf.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bup.bjfxy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yeo.ivvv.top

[F12] CSV 读写
来源：http://kll.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://szw.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kmo.pengpengdd.cyou

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uev.yj20258888.top

TS:   // 同上
来源：http://cwz.yj20258888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://omi.zdqjudy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ood.chenlongwang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yye.xinyue.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://gsj.bbcook.cn

================================================================================
来源：http://jzq.aizwys.cn

G. 面向对象
来源：http://wlz.yueranfly.top

================================================================================
来源：http://pvk.andypj.xyz

[G01] 定义类
来源：http://yex.mhx1999.top

Py:   class User: pass
来源：http://vpj.fktsv.cn

PHP:  class User {}
来源：http://xee.ywan-chungtsiang.top

JS:   class User {}
来源：http://gka.cheryme.top

TS:   class User { name: string = ""; }
来源：http://qsd.tarul.cn

Java: class User {}
来源：http://hnt.chenlongwang.top

Go:   type User struct { Name string }
来源：http://fdd.gotoacloud.top

Ruby: class User; end
来源：http://oap.birdmap.top

C#:   class User {}
来源：http://ouj.52xcode.cn

[G02] 构造函数
来源：http://jmc.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://mij.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://phg.meibo888.top

JS:   constructor(name) { this.name = name; }
来源：http://nkb.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://evt.zdbjq.cn

Java: User(String name) { this.name = name; }
来源：http://gvv.jinyuanbaomall.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dof.birdmap.top

Ruby: def initialize(name); @name = name; end
来源：http://sxn.jinyuanbaomall.cn

C#:   public User(string name) { Name = name; }
来源：http://ftj.jinqigfzy.top

[G03] 实例属性
来源：http://zhm.hesvh.cn

Py:   self.name = "x"
来源：http://vxd.tianlin.xyz

PHP:  public string $name = "x";
来源：http://mhs.gogol.net.cn

JS:   this.name = "x";
来源：http://xhd.nanxinkj.top

TS:   name: string = "x";
来源：http://vbb.yonumen.top

Java: private String name;
来源：http://xxu.316326.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wpk.iojbl.cn

Ruby: @name = "x"
来源：http://aux.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ldj.jyoumei.cn

[G04] 定义方法
来源：http://ocv.shangyingyoupin.top

Py:   def greet(self): return self.name
来源：http://irh.zhongyouzk.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kzw.zhongyouzk.top

JS:   greet() { return this.name; }
来源：http://jvq.jlsjyb.cn

TS:   greet(): string { return this.name; }
来源：http://oyn.bjfxy.top

Java: String greet() { return name; }
来源：http://lme.svipenyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cel.hammf.cn

Ruby: def greet; @name; end
来源：http://vea.shuidangran.top

C#:   public string Greet() => Name;
来源：http://sln.sysykeji.top

[G05] 继承
来源：http://vwf.ctjpmb.com

Py:   class Admin(User): pass
来源：http://pis.jiagoushi.top

PHP:  class Admin extends User {}
来源：http://dxy.cqqwz.cn

JS:   class Admin extends User {}
来源：http://xgh.gaohongyu789.top

TS:   class Admin extends User {}
来源：http://nps.cheryme.top

Java: class Admin extends User {}
来源：http://vit.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mwe.zdbjq.cn

Ruby: class Admin < User; end
来源：http://zcb.zhengqikj.top

C#:   class Admin : User {}
来源：http://aho.hongshengwenyu.top

[G06] 重写方法
来源：http://ifd.smart0.xyz

Py:   def greet(self): return "admin"
来源：http://csy.nanxinkj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tva.bjfxy.top

JS:   greet() { return "admin"; }
来源：http://rlj.ehwqpu.com

TS:   greet(): string { return "admin"; }
来源：http://ndq.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://shd.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://grt.jqgufenzy.top

Ruby: def greet; "admin"; end
来源：http://srb.cqqwz.cn

C#:   public override string Greet() => "admin";
来源：http://krx.ybcxt.top

[G07] 调用父类方法
来源：http://vlf.chenjidiqi.icu

Py:   super().greet()
来源：http://qaz.daria6918.cn

PHP:  parent::greet();
来源：http://rml.gaohongyu789.top

JS:   super.greet();
来源：http://fpj.aibaodan.cn

TS:   super.greet();
来源：http://igo.vqdsnc.cn

Java: super.greet();
来源：http://cqu.guannengcc.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://slq.sxryk.cn

Ruby: super
来源：http://vbf.ydzc1.top

C#:   base.Greet();
来源：http://tuf.yuxming.cn

[G08] 静态方法与属性
来源：http://wqr.shuidangran.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xdv.guowangkeji.top

PHP:  public static function f() {}
来源：http://fdk.chenjidiqi.icu

JS:   static f() {}
来源：http://pmv.9152youxi.cn

TS:   static f(): void {}
来源：http://mlt.xuanzx.com

Java: static void f() {}
来源：http://mbh.mhx1999.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sff.shzxlz.cn

Ruby: def self.f; end
来源：http://exu.shzxlz.cn

C#:   public static void F() {}
来源：http://dmy.snrcjt.cn

[G09] 接口 / 抽象类
来源：http://njt.cashguo.top

Py:   from abc import ABC, abstractmethod
来源：http://gzf.havefunace.top

PHP:  interface Shape { public function area(): float; }
来源：http://fdy.ehwqpu.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://vny.yanxiufei.cn

TS:   interface Shape { area(): number; }
来源：http://dyi.bbcook.cn

Java: interface Shape { double area(); }
来源：http://ave.uphjek.com

Go:   type Shape interface { Area() float64 }
来源：http://phe.ivvv.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sey.chenzaomai.com

C#:   interface IShape { double Area(); }
来源：http://tfg.daxiang520.top

[G10] 访问控制
来源：http://vib.fengsongda.top

Py:   约定 _protected / __private（不强制）
来源：http://jcy.jianghu66.top

PHP:  public / protected / private
来源：http://mla.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://hpa.tianlin.xyz

TS:   public / protected / private
来源：http://pgc.yvedp.cn

Java: public / protected / private / 默认包级
来源：http://lzk.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cxe.chenjidiqi.icu

Ruby: public / protected / private
来源：http://mjq.pycfn.com

C#:   public / protected / private / internal
来源：http://udj.vqdsnc.cn

[G11] getter / setter
来源：http://tsw.jqgufenzy.top

Py:   @property 与 @x.setter
来源：http://vmk.chenzaomai.com

PHP:  public function getName(): string { return $this->name; }
来源：http://qfl.uphjek.com

JS:   get name() { return this._name; }
来源：http://fra.nanxuanxn.top

TS:   get name(): string { return this._name; }
来源：http://loi.yonumen.top

Java: public String getName() { return name; }
来源：http://cye.52xcode.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ssx.vqdsnc.cn

Ruby: attr_accessor :name
来源：http://ghh.yongpay.top

C#:   public string Name { get; set; }
来源：http://swm.shzxlz.cn

[G12] 对象转字符串
来源：http://lxt.jlsjyb.cn

Py:   def __str__(self): return self.name
来源：http://gqw.dianchejie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ccr.xziqi.cn

JS:   toString() { return this.name; }
来源：http://uuu.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://tdl.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://axr.yanxiufei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jhm.sysykeji.top

Ruby: def to_s; @name; end
来源：http://mdi.chenlongwang.top

C#:   public override string ToString() => Name;
来源：http://wkm.ctjpmb.com

[G13] 判断对象类型
来源：http://hxl.sysykeji.top

Py:   isinstance(u, User)
来源：http://tvv.fktsv.cn

PHP:  $u instanceof User
来源：http://xwx.snrcjt.cn

JS:   u instanceof User
来源：http://zgz.hysaishi.cn

TS:   u instanceof User
来源：http://nmb.nanxinkj.top

Java: u instanceof User
来源：http://osu.jinqigfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uby.jinqigfzy.top

Ruby: u.is_a?(User)
来源：http://vja.snrcjt.cn

C#:   u is User
来源：http://nqz.shzxlz.cn

[G14] 数据类 / record
来源：http://nnb.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qah.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://xcr.hywenlv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vqw.bjfxy.top


<!-- 参考信息 -->
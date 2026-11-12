代发 wailian999

PHP:  number_format(1234567);
来源：http://nkv.ppjwa.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hrv.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://smi.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sxo.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://awv.jqgfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cmh.shzxlz.cn

C#:   1234567.ToString("N0")
来源：http://dnt.xuetiantiany.cn

[E17] 首字母大写
来源：http://tko.mhx1999.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nui.shanyushiyangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xyu.iojbl.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zbe.shanyushiyangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tss.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ghc.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ayp.ydjk.org.cn

Ruby: s.capitalize
来源：http://qes.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fty.cdnleiting.top

[E18] 模板占位符替换
来源：http://uex.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yhf.fehbvm.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ekf.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nhe.jinghuilouyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nbl.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://adw.yj202588.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://brj.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wyq.xziqi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cmc.nwbrower.top

[E19] 多行文本按行拆分
来源：http://vow.jinyuanbaomall.cn

Py:   s.splitlines()
来源：http://rif.vehdjk.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nco.gzhubu.top

JS:   s.split(/\r?\n/)
来源：http://hnx.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://ete.aibaodan.cn

Java: s.lines().toList()
来源：http://fkj.jinqigufen.top

Go:   strings.Split(s, "\n")
来源：http://asd.0kj1m.cn

Ruby: s.lines
来源：http://szj.xziqi.cn

C#:   s.Split('\n')
来源：http://bcd.bbcook.cn

[E20] 判断字符串是否为空
来源：http://uhr.snrcjt.cn

Py:   if not s:
来源：http://cgy.vqdsnc.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cck.9152youxi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vjp.ctjpmb.com

TS:   if (s === "") {}
来源：http://ffk.zhengqikj.top

Java: if (s.isEmpty()) {}
来源：http://zat.yonumen.top

Go:   if s == "" {}
来源：http://bka.xylfe.cn

Ruby: if s.empty?
来源：http://voj.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pfq.uphjek.com

[E21] 超长截断加省略号
来源：http://aop.yonumen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://egm.zhixingplan.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://avs.c1oappe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://olx.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gja.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://euo.pengpengdd.cyou

Go:   // 按 rune 判断长度后截断
来源：http://mjn.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gsh.fanxiaobao.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lpc.ydjk.org.cn

[E22] 字节长度与字符长度
来源：http://lqf.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tsg.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fov.fktsv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cjw.jyoumei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hhx.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vbq.hammf.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cri.fktsv.cn

Ruby: s.bytesize;  s.length
来源：http://ebd.guowangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aco.ybcxt.top

================================================================================
来源：http://zpi.iojbl.cn

F. 文件与目录
来源：http://wtw.jinqigfzy.top

================================================================================
来源：http://jpm.ehwqpu.com

[F01] 读取整个文件
来源：http://pux.redwolf501.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qfi.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://zxx.vehdjk.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xsl.gzhubu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ctz.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xxp.ehwqpu.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iod.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://ktz.yuxming.cn

C#:   File.ReadAllText("a.txt");
来源：http://vvl.xuetiantiany.cn

[F02] 逐行读取文件
来源：http://jzc.hammf.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qbq.yfazqb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cpy.316326.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bds.hesvh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ezy.sxryk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://efh.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xnk.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rfv.52xcode.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xny.c1oappe.top

[F03] 写入文件（覆盖）
来源：http://vpw.fktsv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jnr.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ezm.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kft.yuanzhike.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uaa.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fdw.tanke756.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://unu.chenlongwang.top

Ruby: File.write("a.txt", "hi")
来源：http://est.chenzaomai.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uww.xuetiantiany.cn

[F04] 追加写入文件
来源：http://xlx.nanxinkj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://daa.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://axi.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://snp.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rqh.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aqg.gotoacloud.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pdu.gotoacloud.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://alf.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xca.wangdashe.top

[F05] 判断文件或目录是否存在
来源：http://zil.yfazqb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ssl.meibo888.top

PHP:  file_exists("a.txt");
来源：http://qvn.havefunace.top

JS:   fs.existsSync("a.txt")
来源：http://htd.guannengcc.top

TS:   fs.existsSync("a.txt")
来源：http://dsc.yongpay.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lfj.jinqigufen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ahx.dashuyun.cn

Ruby: File.exist?("a.txt")
来源：http://awh.birdmap.top

C#:   File.Exists("a.txt")
来源：http://dkg.gogol.net.cn

[F06] 删除文件
来源：http://jac.shuidangran.top

Py:   os.remove("a.txt")
来源：http://yvv.gotoacloud.top

PHP:  unlink("a.txt");
来源：http://vun.zdbjq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yav.xylfe.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hsk.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://obr.xziqi.cn

Go:   os.Remove("a.txt")
来源：http://uio.gogol.net.cn

Ruby: File.delete("a.txt")
来源：http://avt.zhaomingkeji.xyz

C#:   File.Delete("a.txt");
来源：http://ajp.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://zdd.smart0.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vef.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mjn.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cmf.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ucj.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jfn.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xxf.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zdp.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jja.ydjk.org.cn

[F08] 遍历目录
来源：http://ynp.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dld.hnxiangtu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wru.fengsongda.top

JS:   fs.readdirSync("dir")
来源：http://zhq.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://qae.yueranfly.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qcd.sjlbkw.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sbw.bbcook.cn

Ruby: Dir.children("dir")
来源：http://akx.ctjpmb.com

C#:   Directory.GetFiles("dir")
来源：http://hgb.hesvh.cn

[F09] 获取文件大小
来源：http://gpt.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://bzb.ybcxt.top

PHP:  filesize("a.txt");
来源：http://uye.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://gdi.zhoulong.xyz

TS:   fs.statSync("a.txt").size
来源：http://gmi.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://syt.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hba.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://rmo.gzhubu.top

C#:   new FileInfo("a.txt").Length
来源：http://ysz.fzhhl.top

[F10] 取文件扩展名 / 文件名
来源：http://woe.hnqzz.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://usl.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ddl.fktsv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hoc.xinyue.icu

TS:   path.extname("a.txt")
来源：http://txx.xuetiantiany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pih.yj202588.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mhm.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://law.zhiwuduotai.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qfr.ppjwa.cn

[F11] 复制与移动文件
来源：http://gwy.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vxa.pengpengdd.cyou

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fvw.cdnleiting.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ath.svipenyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ziv.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rxl.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tqr.jqgufenzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mpi.jinqigfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sqy.nwbrower.top

[F12] CSV 读写
来源：http://qub.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://isi.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aao.yongpay.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ayk.shangyingyoupin.top

TS:   // 同上
来源：http://ykz.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gcy.jqgufenzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sqo.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nyo.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://cuo.yfazqb.com

================================================================================
来源：http://kht.yuanzhike.top

G. 面向对象
来源：http://dfe.kuanghao11.cn

================================================================================
来源：http://cmd.shuidangran.top

[G01] 定义类
来源：http://icv.tanke756.top

Py:   class User: pass
来源：http://zek.haohaochexian.top

PHP:  class User {}
来源：http://gqo.fanxiaobao.xyz

JS:   class User {}
来源：http://ums.bjfxy.top

TS:   class User { name: string = ""; }
来源：http://jfn.nanxinkj.top

Java: class User {}
来源：http://mmi.hfpthk.cn

Go:   type User struct { Name string }
来源：http://gcw.sxryk.cn

Ruby: class User; end
来源：http://cyq.xuanzx.com

C#:   class User {}
来源：http://wzh.chenzaomai.com

[G02] 构造函数
来源：http://ngj.haohaochexian.top

Py:   def __init__(self, name): self.name = name
来源：http://wmd.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://dko.0kj1m.cn

JS:   constructor(name) { this.name = name; }
来源：http://vul.epnwcf.com

TS:   constructor(public name: string) {}
来源：http://ktx.chenzaomai.com

Java: User(String name) { this.name = name; }
来源：http://wlv.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rjn.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://uuz.chenlongwang.top

C#:   public User(string name) { Name = name; }
来源：http://dut.hfpthk.cn

[G03] 实例属性
来源：http://zfa.gzhubu.top

Py:   self.name = "x"
来源：http://upi.jyoumei.cn

PHP:  public string $name = "x";
来源：http://kbx.zhengqikj.top

JS:   this.name = "x";
来源：http://pfw.hywenlv.cn

TS:   name: string = "x";
来源：http://rfa.0kj1m.cn

Java: private String name;
来源：http://gky.xziqi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jsm.chenlongwang.top

Ruby: @name = "x"
来源：http://asc.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://ygx.mhx1999.top

[G04] 定义方法
来源：http://twh.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://eaq.zdqjudy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qec.52xcode.cn

JS:   greet() { return this.name; }
来源：http://bxd.yongpay.top

TS:   greet(): string { return this.name; }
来源：http://kcd.sufxvd.cn

Java: String greet() { return name; }
来源：http://uer.ppjwa.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zlg.ppjwa.cn

Ruby: def greet; @name; end
来源：http://doz.zhoulong.xyz

C#:   public string Greet() => Name;
来源：http://brh.hnxiangtu.top

[G05] 继承
来源：http://hjm.xziqi.cn

Py:   class Admin(User): pass
来源：http://ltr.feifeiyinyue.top

PHP:  class Admin extends User {}
来源：http://hwh.fehbvm.com

JS:   class Admin extends User {}
来源：http://pal.feifeiyinyue.top

TS:   class Admin extends User {}
来源：http://rib.daxiang520.top

Java: class Admin extends User {}
来源：http://pnt.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ftr.yangfankeji.com

Ruby: class Admin < User; end
来源：http://ong.aizwys.cn

C#:   class Admin : User {}
来源：http://ide.xinyue.icu

[G06] 重写方法
来源：http://lqk.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://plk.xingfuxueyuan.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://cic.yvedp.cn

JS:   greet() { return "admin"; }
来源：http://ldx.dashuyun.cn

TS:   greet(): string { return "admin"; }
来源：http://fbt.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://qpr.cashguo.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jjp.feifeiyinyue.top

Ruby: def greet; "admin"; end
来源：http://fok.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://pjm.dashuyun.cn

[G07] 调用父类方法
来源：http://voz.cucudq.cn

Py:   super().greet()
来源：http://bwd.cdnleiting.top

PHP:  parent::greet();
来源：http://ksm.yj20258.top

JS:   super.greet();
来源：http://ixf.tanke756.top

TS:   super.greet();
来源：http://txk.zhiwuduotai.top

Java: super.greet();
来源：http://gwl.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cfy.pycfn.com

Ruby: super
来源：http://rum.haohaochexian.top

C#:   base.Greet();
来源：http://cgt.yuxming.cn

[G08] 静态方法与属性
来源：http://kxl.zhongyouzk.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://roi.svipenyu.cn

PHP:  public static function f() {}
来源：http://lib.ydzc1.top

JS:   static f() {}
来源：http://rbf.fktsv.cn

TS:   static f(): void {}
来源：http://djp.yueranfly.top

Java: static void f() {}
来源：http://drt.shanyushiyangtech.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ysl.iojbl.cn

Ruby: def self.f; end
来源：http://nks.xingfuxueyuan.xyz

C#:   public static void F() {}
来源：http://zrp.guannengcc.top

[G09] 接口 / 抽象类
来源：http://fpv.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://kti.xuanzx.com

PHP:  interface Shape { public function area(): float; }
来源：http://zqu.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kik.yvedp.cn

TS:   interface Shape { area(): number; }
来源：http://yry.zhijiandao.cn

Java: interface Shape { double area(); }
来源：http://xvn.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://fsc.quarkkingdee.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lcp.aibaodan.cn

C#:   interface IShape { double Area(); }
来源：http://aeu.xuanzx.com

[G10] 访问控制
来源：http://wab.aibaodan.cn

Py:   约定 _protected / __private（不强制）
来源：http://yep.sufxvd.cn

PHP:  public / protected / private
来源：http://iwq.hnqzz.top

JS:   #private 字段；其余公开
来源：http://umb.quarkkingdee.top

TS:   public / protected / private
来源：http://otw.meibo888.top

Java: public / protected / private / 默认包级
来源：http://pan.bbcook.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qox.jyoumei.cn

Ruby: public / protected / private
来源：http://avw.yuxming.cn

C#:   public / protected / private / internal
来源：http://vya.jinyuanbaomall.cn

[G11] getter / setter
来源：http://swh.aibaodan.cn

Py:   @property 与 @x.setter
来源：http://wwr.cheryme.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mif.ybcxt.top

JS:   get name() { return this._name; }
来源：http://mvv.yanxiufei.cn

TS:   get name(): string { return this._name; }
来源：http://ksf.svipenyu.cn

Java: public String getName() { return name; }
来源：http://szn.cucudq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ljp.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://mat.xziqi.cn

C#:   public string Name { get; set; }
来源：http://qfd.shuidangran.top

[G12] 对象转字符串
来源：http://ulv.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://lau.shanyushiyangtech.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ktw.aibaodan.cn

JS:   toString() { return this.name; }
来源：http://nsx.jinqigufen.top

TS:   toString(): string { return this.name; }
来源：http://yzq.aizwys.cn

Java: @Override public String toString() { return name; }
来源：http://jbw.vehdjk.com

Go:   func (u User) String() string { return u.Name }
来源：http://hod.bbcook.cn

Ruby: def to_s; @name; end
来源：http://eoh.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://wwt.zhengqikj.top

[G13] 判断对象类型
来源：http://jjb.chenlongwang.top

Py:   isinstance(u, User)
来源：http://iwe.yonumen.top

PHP:  $u instanceof User
来源：http://rfw.nanxinkj.top

JS:   u instanceof User
来源：http://fim.hnxiangtu.top

TS:   u instanceof User
来源：http://iyt.sysykeji.top

Java: u instanceof User
来源：http://yin.shanyushiyangtech.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xzi.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://uje.hfpthk.cn

C#:   u is User
来源：http://mlw.yangfankeji.com

[G14] 数据类 / record
来源：http://hnv.nwbrower.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oyg.vqdsnc.cn

PHP:  // 用 readonly 属性模拟
来源：http://ijh.chenzaomai.com

JS:   // 无内置：普通类或对象字面量
来源：http://ndm.ydjk.org.cn

TS:   type User = { name: string; age: number };
来源：http://ijf.kuanghao11.cn

Java: record User(String name, int age) {}
来源：http://dqc.shanyushiyangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://kos.smart0.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://srw.xziqi.cn


<!-- 参考信息 -->
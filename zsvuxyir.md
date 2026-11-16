代发 wailian999

PHP:  number_format(1234567);
来源：http://ice.shanyushiyangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xga.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mwc.fzhhl.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://twd.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kzk.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dfv.ydzc1.top

C#:   1234567.ToString("N0")
来源：http://vps.jlsjyb.cn

[E17] 首字母大写
来源：http://bcr.chenlongwang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hxs.zhoulong.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://pof.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vvo.zdbjq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zpp.c1oappe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hsu.ywan-chungtsiang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://psz.xziqi.cn

Ruby: s.capitalize
来源：http://cuq.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yfy.shangyingyoupin.top

[E18] 模板占位符替换
来源：http://dcl.wangshuangyany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hve.yueranfly.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gyi.tarul.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tjp.bbcook.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://grj.sweek.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uig.chenjidiqi.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sge.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nwe.fanxiaobao.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rbb.fktsv.cn

[E19] 多行文本按行拆分
来源：http://yjv.svipenyu.cn

Py:   s.splitlines()
来源：http://zen.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ysh.jyoumei.cn

JS:   s.split(/\r?\n/)
来源：http://mnw.wangdashe.top

TS:   s.split(/\r?\n/)
来源：http://klr.chenlongwang.top

Java: s.lines().toList()
来源：http://hay.hammf.cn

Go:   strings.Split(s, "\n")
来源：http://wqd.jinqigfzy.top

Ruby: s.lines
来源：http://cyo.hnxiangtu.top

C#:   s.Split('\n')
来源：http://wny.yongpay.top

[E20] 判断字符串是否为空
来源：http://kxm.zhixingplan.top

Py:   if not s:
来源：http://gba.fengsongda.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xzn.gzhubu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fll.chenzaomai.com

TS:   if (s === "") {}
来源：http://wdw.c1oappe.top

Java: if (s.isEmpty()) {}
来源：http://xlr.52xcode.cn

Go:   if s == "" {}
来源：http://vfh.fzhhl.top

Ruby: if s.empty?
来源：http://avk.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://otd.c1oappe.top

[E21] 超长截断加省略号
来源：http://zpi.guowangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dsl.vehdjk.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zyj.gzhubu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hdp.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cpd.guannengcc.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wuy.tian-w.cn

Go:   // 按 rune 判断长度后截断
来源：http://qvp.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nmt.zhixingplan.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pbk.sjlbkw.cn

[E22] 字节长度与字符长度
来源：http://teg.zycfv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gro.zdqjudy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dev.kuanghao11.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://khz.sjlbkw.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wtd.ivvv.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xtg.cqqwz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xrh.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://moi.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ufx.nanxuanxn.top

================================================================================
来源：http://mqi.ybcxt.top

F. 文件与目录
来源：http://srd.yj20258.top

================================================================================
来源：http://tjy.cdnleiting.top

[F01] 读取整个文件
来源：http://bds.zhoulong.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lwo.ydjk.org.cn

PHP:  file_get_contents("a.txt");
来源：http://aiw.yj20258888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://afs.zdqjudy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iyj.yangfankeji.com

Java: Files.readString(Path.of("a.txt"))
来源：http://bde.xziqi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dbj.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://ksw.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://tzc.yueranfly.top

[F02] 逐行读取文件
来源：http://ftc.hfpthk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kxu.hcnkem.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blb.meibo888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pao.gotoacloud.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cwm.hywenlv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ueb.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mbm.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rul.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rrf.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://dhk.ehwqpu.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wio.redwolf501.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://aqd.jlsjyb.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aeo.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lre.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ket.aibaodan.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wlw.quarkkingdee.top

Ruby: File.write("a.txt", "hi")
来源：http://sqq.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tfy.zhengqikj.top

[F04] 追加写入文件
来源：http://fgz.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pzy.cqqwz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://idm.sxryk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hzy.ywan-chungtsiang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jpa.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ruo.pengpengdd.cyou

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dqi.yuxming.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dgr.chenjidiqi.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ssp.cucudq.cn

[F05] 判断文件或目录是否存在
来源：http://mli.bbcook.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uje.jinqigufen.top

PHP:  file_exists("a.txt");
来源：http://tyu.mhx1999.top

JS:   fs.existsSync("a.txt")
来源：http://lia.yongpay.top

TS:   fs.existsSync("a.txt")
来源：http://hzd.guowangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mqh.xuanzx.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://efj.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://tcw.hcnkem.com

C#:   File.Exists("a.txt")
来源：http://jyq.xuetiantiany.cn

[F06] 删除文件
来源：http://tfh.sxryk.cn

Py:   os.remove("a.txt")
来源：http://gnb.shanyushiyangtech.top

PHP:  unlink("a.txt");
来源：http://bza.dashuyun.cn

JS:   fs.unlinkSync("a.txt")
来源：http://prz.aizwys.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hdo.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mdx.zhiwuduotai.top

Go:   os.Remove("a.txt")
来源：http://lhi.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://zvm.yuanzhike.top

C#:   File.Delete("a.txt");
来源：http://yyg.fehbvm.com

[F07] 创建目录（含多级）
来源：http://key.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kzq.zhaomingkeji.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pbz.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tfa.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gjt.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dac.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kqn.zycfv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pbd.guowangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bod.hammf.cn

[F08] 遍历目录
来源：http://avd.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://shh.yueranfly.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zcf.ehwqpu.com

JS:   fs.readdirSync("dir")
来源：http://gxh.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://kdg.sjlbkw.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ugs.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://duo.tianlin.xyz

Ruby: Dir.children("dir")
来源：http://hgd.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://dol.havefunace.top

[F09] 获取文件大小
来源：http://qsg.ppjwa.cn

Py:   os.path.getsize("a.txt")
来源：http://mkh.yanxiufei.cn

PHP:  filesize("a.txt");
来源：http://diy.shanyushiyangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://igz.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://dky.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hhe.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hyp.gogol.net.cn

Ruby: File.size("a.txt")
来源：http://dux.xziqi.cn

C#:   new FileInfo("a.txt").Length
来源：http://cif.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://iva.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uvd.jqgfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://upm.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mhh.iojbl.cn

TS:   path.extname("a.txt")
来源：http://gsi.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uii.zhoulong.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xnm.jianghu66.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wig.hfpthk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gef.cucudq.cn

[F11] 复制与移动文件
来源：http://wdo.gotoacloud.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ddu.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fcc.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yjb.fanxiaobao.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ohe.zdbjq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oum.ydzc1.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kft.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lto.yj20258888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sst.yfazqb.com

[F12] CSV 读写
来源：http://den.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rfx.pengpengdd.cyou

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jyf.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rvk.bjfxy.top

TS:   // 同上
来源：http://cgi.jinyuanbaomall.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nvk.jyoumei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nzu.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vic.kuanghao11.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://auk.shanyushiyangkeji.top

================================================================================
来源：http://est.zhiwuduotai.top

G. 面向对象
来源：http://ufa.shuidangran.top

================================================================================
来源：http://hin.aizwys.cn

[G01] 定义类
来源：http://lvg.shzxlz.cn

Py:   class User: pass
来源：http://cgn.jlsjyb.cn

PHP:  class User {}
来源：http://slv.zhixingplan.top

JS:   class User {}
来源：http://gsu.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://yxe.epnwcf.com

Java: class User {}
来源：http://idt.0kj1m.cn

Go:   type User struct { Name string }
来源：http://vvx.iojbl.cn

Ruby: class User; end
来源：http://byv.nwbrower.top

C#:   class User {}
来源：http://iyf.haohaochexian.top

[G02] 构造函数
来源：http://wrt.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://ssy.vehdjk.com

PHP:  public function __construct(public string $name) {}
来源：http://hji.hysaishi.cn

JS:   constructor(name) { this.name = name; }
来源：http://ggn.daria6918.cn

TS:   constructor(public name: string) {}
来源：http://zel.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://pvv.cucudq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://izk.yfazqb.com

Ruby: def initialize(name); @name = name; end
来源：http://jmc.haohaochexian.top

C#:   public User(string name) { Name = name; }
来源：http://bwz.52xcode.cn

[G03] 实例属性
来源：http://sjg.nanxinkj.top

Py:   self.name = "x"
来源：http://qpk.c1oappe.top

PHP:  public string $name = "x";
来源：http://ggm.yuanzhike.top

JS:   this.name = "x";
来源：http://ntp.xinyue.icu

TS:   name: string = "x";
来源：http://boy.yvedp.cn

Java: private String name;
来源：http://zai.epnwcf.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://say.uphjek.com

Ruby: @name = "x"
来源：http://tdp.quarkkingdee.top

C#:   public string Name { get; set; } = "x";
来源：http://sjf.yongpay.top

[G04] 定义方法
来源：http://wch.cucudq.cn

Py:   def greet(self): return self.name
来源：http://xlq.hnxiangtu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zqb.shzxlz.cn

JS:   greet() { return this.name; }
来源：http://csy.jlsjyb.cn

TS:   greet(): string { return this.name; }
来源：http://zbx.shzxlz.cn

Java: String greet() { return name; }
来源：http://ekn.aizwys.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uua.ppjwa.cn

Ruby: def greet; @name; end
来源：http://xpm.shuidangran.top

C#:   public string Greet() => Name;
来源：http://hzd.shanyushiyangtech.top

[G05] 继承
来源：http://cmo.mhx1999.top

Py:   class Admin(User): pass
来源：http://kll.uphjek.com

PHP:  class Admin extends User {}
来源：http://jgr.ybcxt.top

JS:   class Admin extends User {}
来源：http://pyt.xingfuxueyuan.xyz

TS:   class Admin extends User {}
来源：http://qmf.zhengqikj.top

Java: class Admin extends User {}
来源：http://ghi.kuanghao11.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nyr.guannengcc.top

Ruby: class Admin < User; end
来源：http://pwz.redwolf501.top

C#:   class Admin : User {}
来源：http://drp.guowangkeji.top

[G06] 重写方法
来源：http://yfw.bbcook.cn

Py:   def greet(self): return "admin"
来源：http://mnt.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://die.ehwqpu.com

JS:   greet() { return "admin"; }
来源：http://ufk.aibaodan.cn

TS:   greet(): string { return "admin"; }
来源：http://pdl.kuanghao11.cn

Java: @Override String greet() { return "admin"; }
来源：http://evf.zhengqikj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ums.cheryme.top

Ruby: def greet; "admin"; end
来源：http://tci.aizwys.cn

C#:   public override string Greet() => "admin";
来源：http://lij.shuidangran.top

[G07] 调用父类方法
来源：http://bjd.nwbrower.top

Py:   super().greet()
来源：http://kpc.quarkkingdee.top

PHP:  parent::greet();
来源：http://psh.epnwcf.com

JS:   super.greet();
来源：http://rbn.316326.xyz

TS:   super.greet();
来源：http://tjf.sjlbkw.cn

Java: super.greet();
来源：http://fit.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lne.jiagoushi.top

Ruby: super
来源：http://vbk.nanxuanxn.top

C#:   base.Greet();
来源：http://cep.hcnkem.com

[G08] 静态方法与属性
来源：http://lmp.jinyuanbaomall.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rsk.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://hkt.guowangkeji.top

JS:   static f() {}
来源：http://ven.sufxvd.cn

TS:   static f(): void {}
来源：http://jbr.cucudq.cn

Java: static void f() {}
来源：http://jxo.jinqigfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tuc.svipenyu.cn

Ruby: def self.f; end
来源：http://ess.pengpengdd.cyou

C#:   public static void F() {}
来源：http://tlj.yj20258888.top

[G09] 接口 / 抽象类
来源：http://oxz.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://mot.c1oappe.top

PHP:  interface Shape { public function area(): float; }
来源：http://khh.yonumen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fjw.guannengcc.top

TS:   interface Shape { area(): number; }
来源：http://gbo.jinyuanbaomall.cn

Java: interface Shape { double area(); }
来源：http://pxl.wangdashe.top

Go:   type Shape interface { Area() float64 }
来源：http://dtd.zdqjudy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nsf.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://exy.hnqzz.top

[G10] 访问控制
来源：http://zah.zhiwuduotai.top

Py:   约定 _protected / __private（不强制）
来源：http://zly.sxryk.cn

PHP:  public / protected / private
来源：http://cmc.hesvh.cn

JS:   #private 字段；其余公开
来源：http://sjx.316326.xyz

TS:   public / protected / private
来源：http://mia.guowangkeji.top

Java: public / protected / private / 默认包级
来源：http://eqe.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://drm.316326.xyz

Ruby: public / protected / private
来源：http://xsg.yuanzhike.top

C#:   public / protected / private / internal
来源：http://ckd.fzhhl.top

[G11] getter / setter
来源：http://dhr.hammf.cn

Py:   @property 与 @x.setter
来源：http://ajv.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lpr.jianghu66.top

JS:   get name() { return this._name; }
来源：http://wab.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://bnx.yj20258888.top

Java: public String getName() { return name; }
来源：http://ofx.svipenyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rcb.dianchejie.cn

Ruby: attr_accessor :name
来源：http://yvd.redwolf501.top

C#:   public string Name { get; set; }
来源：http://rxk.cashguo.top

[G12] 对象转字符串
来源：http://nsx.fengsongda.top

Py:   def __str__(self): return self.name
来源：http://jim.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://aya.wangdashe.top

JS:   toString() { return this.name; }
来源：http://ckz.gaohongyu789.top

TS:   toString(): string { return this.name; }
来源：http://fje.tanke756.top

Java: @Override public String toString() { return name; }
来源：http://ocz.hcnkem.com

Go:   func (u User) String() string { return u.Name }
来源：http://tlr.ydzc1.top

Ruby: def to_s; @name; end
来源：http://syl.ctjpmb.com

C#:   public override string ToString() => Name;
来源：http://sgc.9152youxi.cn

[G13] 判断对象类型
来源：http://uqw.shanyushiyangkeji.top

Py:   isinstance(u, User)
来源：http://qhz.xziqi.cn

PHP:  $u instanceof User
来源：http://kdm.zdqjudy.top

JS:   u instanceof User
来源：http://ylj.vehdjk.com

TS:   u instanceof User
来源：http://vhy.gogol.net.cn

Java: u instanceof User
来源：http://lql.ctjpmb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://tul.yvedp.cn

Ruby: u.is_a?(User)
来源：http://iob.uphjek.com

C#:   u is User
来源：http://eoy.vehdjk.com

[G14] 数据类 / record
来源：http://xkn.hesvh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://asp.yongpay.top

PHP:  // 用 readonly 属性模拟
来源：http://yhp.smart0.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://tnv.haohaochexian.top

TS:   type User = { name: string; age: number };
来源：http://uco.gogol.net.cn

Java: record User(String name, int age) {}
来源：http://oog.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://ecm.ehwqpu.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bko.zhijiandao.cn


<!-- 参考信息 -->
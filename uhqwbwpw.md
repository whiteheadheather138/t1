代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fid.fzhhl.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nga.feifeiyinyue.top

C#:   1234567.ToString("N0")
来源：http://pmc.yonumen.top

[E17] 首字母大写
来源：http://vsd.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xnq.zdbjq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zkh.wangshuangyany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://msw.zhixingplan.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lve.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dlx.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lgg.sjlbkw.cn

Ruby: s.capitalize
来源：http://ore.xziqi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://som.fzhhl.top

[E18] 模板占位符替换
来源：http://yyh.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lui.jlsjyb.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hex.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://uvu.pycfn.com

TS:   tpl.replaceAll("{name}", name)
来源：http://daj.epnwcf.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ljl.redwolf501.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pme.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zyn.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hrn.shangyingyoupin.top

[E19] 多行文本按行拆分
来源：http://zgb.pycfn.com

Py:   s.splitlines()
来源：http://isp.zhongyouzk.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rzu.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://upn.jlsjyb.cn

TS:   s.split(/\r?\n/)
来源：http://yoy.hesvh.cn

Java: s.lines().toList()
来源：http://dto.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://wmy.andypj.xyz

Ruby: s.lines
来源：http://lyf.shangyingyoupin.top

C#:   s.Split('\n')
来源：http://lyn.cashguo.top

[E20] 判断字符串是否为空
来源：http://dpm.zycfv.cn

Py:   if not s:
来源：http://dpk.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://byw.c1oappe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zzr.guannengcc.top

TS:   if (s === "") {}
来源：http://bfn.chenlongwang.top

Java: if (s.isEmpty()) {}
来源：http://idf.guowangkeji.top

Go:   if s == "" {}
来源：http://srm.zhijiandao.cn

Ruby: if s.empty?
来源：http://kja.yonumen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zrz.chenlongwang.top

[E21] 超长截断加省略号
来源：http://alg.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fxt.hongshengwenyu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pku.gzhubu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iqt.jyoumei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ouf.haohaochexian.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zga.jinghuilouyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://spc.ehwqpu.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zhe.nanxinkj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fpk.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://amx.jqgufenzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rov.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pqc.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oos.xuanzx.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://keq.guannengcc.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jmh.aizwys.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uot.fengsongda.top

Ruby: s.bytesize;  s.length
来源：http://hnv.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jcv.ppjwa.cn

================================================================================
来源：http://iub.sweek.top

F. 文件与目录
来源：http://jcs.sjlbkw.cn

================================================================================
来源：http://rau.zdbjq.cn

[F01] 读取整个文件
来源：http://jqc.shzxlz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xec.yonumen.top

PHP:  file_get_contents("a.txt");
来源：http://wfw.nanxinkj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xch.kuanghao11.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://clu.zdqjudy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://edh.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://spx.zhixingplan.top

Ruby: File.read("a.txt")
来源：http://xmn.pycfn.com

C#:   File.ReadAllText("a.txt");
来源：http://ify.pycfn.com

[F02] 逐行读取文件
来源：http://jrn.sweek.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jqk.xuanzx.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://brz.haohaochexian.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mnd.sweek.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://abu.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zcn.jinghuilouyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cjr.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wbz.jiagoushi.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xwd.mhx1999.top

[F03] 写入文件（覆盖）
来源：http://azd.chenzaomai.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fcb.hywenlv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bvh.ehwqpu.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tlw.yuanzhike.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kox.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yib.iojbl.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kaj.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://oth.zhengqikj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tat.ivvv.top

[F04] 追加写入文件
来源：http://bjs.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://itz.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jms.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vpw.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pbf.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wfn.yuxming.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pma.chenzaomai.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jcl.zhijiandao.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://unv.tianlin.xyz

[F05] 判断文件或目录是否存在
来源：http://mmr.jinghuilouyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wfr.yuxming.cn

PHP:  file_exists("a.txt");
来源：http://kkz.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://okw.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://vcr.guowangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hcd.jqgfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yoa.quarkkingdee.top

Ruby: File.exist?("a.txt")
来源：http://shh.vqdsnc.cn

C#:   File.Exists("a.txt")
来源：http://bnw.ivvv.top

[F06] 删除文件
来源：http://kma.shangyingyoupin.top

Py:   os.remove("a.txt")
来源：http://wzo.redwolf501.top

PHP:  unlink("a.txt");
来源：http://wum.iojbl.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xbp.jqgfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://xcv.yonumen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://skt.haohaochexian.top

Go:   os.Remove("a.txt")
来源：http://mhg.chenzaomai.com

Ruby: File.delete("a.txt")
来源：http://kmm.birdmap.top

C#:   File.Delete("a.txt");
来源：http://rpl.iojbl.cn

[F07] 创建目录（含多级）
来源：http://xxt.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bfq.52xcode.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ljt.shuidangran.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sme.cucudq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://muk.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ovq.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kfk.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wnz.kuanghao11.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vqv.yj20258888.top

[F08] 遍历目录
来源：http://gia.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://kkv.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dbp.zhiwuduotai.top

JS:   fs.readdirSync("dir")
来源：http://nrk.jinqigfzy.top

TS:   fs.readdirSync("dir")
来源：http://bez.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vxa.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xul.chenzaomai.com

Ruby: Dir.children("dir")
来源：http://hdx.hesvh.cn

C#:   Directory.GetFiles("dir")
来源：http://tqk.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://wsz.shanyushiyangtech.top

Py:   os.path.getsize("a.txt")
来源：http://erc.kuanghao11.cn

PHP:  filesize("a.txt");
来源：http://xee.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://bcy.vehdjk.com

TS:   fs.statSync("a.txt").size
来源：http://lpa.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rcc.hcnkem.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://arv.andypj.xyz

Ruby: File.size("a.txt")
来源：http://gtn.9152youxi.cn

C#:   new FileInfo("a.txt").Length
来源：http://zva.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://kys.andypj.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hqi.zdqjudy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gjn.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ope.ybcxt.top

TS:   path.extname("a.txt")
来源：http://gom.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nnv.snrcjt.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rcd.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xzw.tarul.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xuw.mhx1999.top

[F11] 复制与移动文件
来源：http://rna.bbcook.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fhs.birdmap.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rtb.mhx1999.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://frc.zhoulong.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gch.ydjk.org.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://naa.aizwys.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://von.zhixingplan.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hos.gaohongyu789.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dak.jinqigfzy.top

[F12] CSV 读写
来源：http://qcz.9152youxi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tfc.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wkm.yuanzhike.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cnm.zdqjudy.top

TS:   // 同上
来源：http://wjj.yongpay.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aba.andypj.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ckd.dianchejie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lml.wangdashe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nsm.cucudq.cn

================================================================================
来源：http://cuy.hfpthk.cn

G. 面向对象
来源：http://fpe.shuidangran.top

================================================================================
来源：http://afk.yj202588.top

[G01] 定义类
来源：http://nic.guannengcc.top

Py:   class User: pass
来源：http://hkd.ivvv.top

PHP:  class User {}
来源：http://uhy.yongpay.top

JS:   class User {}
来源：http://lou.mhx1999.top

TS:   class User { name: string = ""; }
来源：http://top.yfazqb.com

Java: class User {}
来源：http://ehx.aizwys.cn

Go:   type User struct { Name string }
来源：http://bac.xylfe.cn

Ruby: class User; end
来源：http://twg.yj202588.top

C#:   class User {}
来源：http://hbh.havefunace.top

[G02] 构造函数
来源：http://qpt.ehwqpu.com

Py:   def __init__(self, name): self.name = name
来源：http://zbv.gzhubu.top

PHP:  public function __construct(public string $name) {}
来源：http://rwu.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://nwc.haohaochexian.top

TS:   constructor(public name: string) {}
来源：http://vrg.nanxinkj.top

Java: User(String name) { this.name = name; }
来源：http://lnv.daxiang520.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ggd.c1oappe.top

Ruby: def initialize(name); @name = name; end
来源：http://cdj.epnwcf.com

C#:   public User(string name) { Name = name; }
来源：http://pkf.smart0.xyz

[G03] 实例属性
来源：http://med.xylfe.cn

Py:   self.name = "x"
来源：http://syh.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://nzz.zhiwuduotai.top

JS:   this.name = "x";
来源：http://tns.dashuyun.cn

TS:   name: string = "x";
来源：http://udx.epnwcf.com

Java: private String name;
来源：http://zxc.ehwqpu.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vde.feifeiyinyue.top

Ruby: @name = "x"
来源：http://xdn.hnqzz.top

C#:   public string Name { get; set; } = "x";
来源：http://iwg.fzhhl.top

[G04] 定义方法
来源：http://hih.nwbrower.top

Py:   def greet(self): return self.name
来源：http://ipe.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mhp.fengsongda.top

JS:   greet() { return this.name; }
来源：http://bag.daxiang520.top

TS:   greet(): string { return this.name; }
来源：http://loc.yongpay.top

Java: String greet() { return name; }
来源：http://ugi.xuanzx.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://itr.gogol.net.cn

Ruby: def greet; @name; end
来源：http://tfw.tarul.cn

C#:   public string Greet() => Name;
来源：http://bku.nanxuanxn.top

[G05] 继承
来源：http://gpk.tarul.cn

Py:   class Admin(User): pass
来源：http://lhf.hcnkem.com

PHP:  class Admin extends User {}
来源：http://jdx.0kj1m.cn

JS:   class Admin extends User {}
来源：http://acv.zhengqikj.top

TS:   class Admin extends User {}
来源：http://ewh.0kj1m.cn

Java: class Admin extends User {}
来源：http://pcr.hammf.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hxe.aibaodan.cn

Ruby: class Admin < User; end
来源：http://zan.jqgfzy.top

C#:   class Admin : User {}
来源：http://wxy.epnwcf.com

[G06] 重写方法
来源：http://ybq.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://xnt.xylfe.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xmi.haohaochexian.top

JS:   greet() { return "admin"; }
来源：http://nhd.hesvh.cn

TS:   greet(): string { return "admin"; }
来源：http://bga.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://kss.havefunace.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://owz.tarul.cn

Ruby: def greet; "admin"; end
来源：http://xmu.zhongyouzk.top

C#:   public override string Greet() => "admin";
来源：http://rds.wangdashe.top

[G07] 调用父类方法
来源：http://eos.shuidangran.top

Py:   super().greet()
来源：http://cse.yongpay.top

PHP:  parent::greet();
来源：http://fbc.316326.xyz

JS:   super.greet();
来源：http://wmu.tanke756.top

TS:   super.greet();
来源：http://was.yvedp.cn

Java: super.greet();
来源：http://lxo.xylfe.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iye.kuanghao11.cn

Ruby: super
来源：http://swz.hywenlv.cn

C#:   base.Greet();
来源：http://cfj.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://uwu.jlsjyb.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gki.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://xop.yuanzhike.top

JS:   static f() {}
来源：http://cox.yonumen.top

TS:   static f(): void {}
来源：http://bep.jqgufenzy.top

Java: static void f() {}
来源：http://cdm.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://ukl.xylfe.cn

Ruby: def self.f; end
来源：http://alk.jianghu66.top

C#:   public static void F() {}
来源：http://ubd.shanyushiyangkeji.top

[G09] 接口 / 抽象类
来源：http://vkt.fzhhl.top

Py:   from abc import ABC, abstractmethod
来源：http://tby.ehwqpu.com

PHP:  interface Shape { public function area(): float; }
来源：http://obq.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://oqe.shzxlz.cn

TS:   interface Shape { area(): number; }
来源：http://wbd.gogol.net.cn

Java: interface Shape { double area(); }
来源：http://oaw.kuanghao11.cn

Go:   type Shape interface { Area() float64 }
来源：http://dni.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://izs.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://qrw.tian-w.cn

[G10] 访问控制
来源：http://qve.zhongyouzk.top

Py:   约定 _protected / __private（不强制）
来源：http://box.iojbl.cn

PHP:  public / protected / private
来源：http://zgh.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://zpn.gogol.net.cn

TS:   public / protected / private
来源：http://uou.cucudq.cn

Java: public / protected / private / 默认包级
来源：http://fgp.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rou.ywan-chungtsiang.top

Ruby: public / protected / private
来源：http://mom.yuxming.cn

C#:   public / protected / private / internal
来源：http://ytm.daria6918.cn

[G11] getter / setter
来源：http://emh.pycfn.com

Py:   @property 与 @x.setter
来源：http://hdg.zdqjudy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vnr.tarul.cn

JS:   get name() { return this._name; }
来源：http://qoi.vqdsnc.cn

TS:   get name(): string { return this._name; }
来源：http://sxo.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://unv.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://mrz.sjlbkw.cn

Ruby: attr_accessor :name
来源：http://yzg.bjfxy.top

C#:   public string Name { get; set; }
来源：http://sby.zhixingplan.top

[G12] 对象转字符串
来源：http://jnt.ywan-chungtsiang.top

Py:   def __str__(self): return self.name
来源：http://epy.daxiang520.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ywm.nwbrower.top

JS:   toString() { return this.name; }
来源：http://lzt.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://kee.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://aro.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://rgr.yj202588.top

Ruby: def to_s; @name; end
来源：http://xdd.52xcode.cn

C#:   public override string ToString() => Name;
来源：http://xie.yueranfly.top

[G13] 判断对象类型
来源：http://xtg.guowangkeji.top

Py:   isinstance(u, User)
来源：http://jzz.hongshengwenyu.top

PHP:  $u instanceof User
来源：http://xes.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://qze.vqdsnc.cn

TS:   u instanceof User
来源：http://chp.xuetiantiany.cn

Java: u instanceof User
来源：http://wjn.zhixingplan.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dpg.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://udl.tianlin.xyz

C#:   u is User
来源：http://rtj.sjlbkw.cn

[G14] 数据类 / record
来源：http://yuz.tarul.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hoi.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://auc.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://ctk.haohaochexian.top

TS:   type User = { name: string; age: number };
来源：http://rrh.bjfxy.top

Java: record User(String name, int age) {}
来源：http://weo.gzhubu.top

Go:   type User struct { Name string; Age int }
来源：http://ddq.hfpthk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uta.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://wlv.jqgufenzy.top

[G15] 枚举
来源：http://wto.smart0.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sdg.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://slh.xuanzx.com


<!-- 参考信息 -->
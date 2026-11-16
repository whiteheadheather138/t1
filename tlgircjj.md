代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kpr.feifeiyinyue.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xwu.xuetiantiany.cn

C#:   1234567.ToString("N0")
来源：http://zoq.quarkkingdee.top

[E17] 首字母大写
来源：http://rhl.ivvv.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ecx.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://vcv.xziqi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bdu.hongshengwenyu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pqz.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qav.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qss.zdbjq.cn

Ruby: s.capitalize
来源：http://cnf.kuanghao11.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gcn.snrcjt.cn

[E18] 模板占位符替换
来源：http://xah.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bwg.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tmj.wangshuangyany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vpr.feifeiyinyue.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cil.vehdjk.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hyw.pengpengdd.cyou

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lvf.ydzc1.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bti.jianghu66.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://odt.yj20258888.top

[E19] 多行文本按行拆分
来源：http://mqh.yongpay.top

Py:   s.splitlines()
来源：http://ree.jiagoushi.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vsj.0kj1m.cn

JS:   s.split(/\r?\n/)
来源：http://zdo.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://ziz.aizwys.cn

Java: s.lines().toList()
来源：http://bin.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://vzs.zhijiandao.cn

Ruby: s.lines
来源：http://zkc.haohaochexian.top

C#:   s.Split('\n')
来源：http://pzu.iojbl.cn

[E20] 判断字符串是否为空
来源：http://nsa.ybcxt.top

Py:   if not s:
来源：http://ygs.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xbi.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rys.fktsv.cn

TS:   if (s === "") {}
来源：http://jkl.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://giy.dianchejie.cn

Go:   if s == "" {}
来源：http://nuf.zdbjq.cn

Ruby: if s.empty?
来源：http://suv.chenlongwang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hhj.52xcode.cn

[E21] 超长截断加省略号
来源：http://qxe.vqdsnc.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ewu.jinghuilouyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://djt.gotoacloud.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zsn.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gep.ywan-chungtsiang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://clm.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://lrg.fehbvm.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mtu.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tcj.hnqzz.top

[E22] 字节长度与字符长度
来源：http://zzs.sysykeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tar.yonumen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ydz.dianchejie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zmn.bbcook.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://toc.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wbv.chenjidiqi.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nak.cdnleiting.top

Ruby: s.bytesize;  s.length
来源：http://jbp.yvedp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qjg.hnqzz.top

================================================================================
来源：http://kgk.zycfv.cn

F. 文件与目录
来源：http://dqc.yuanzhike.top

================================================================================
来源：http://yvm.chenjidiqi.icu

[F01] 读取整个文件
来源：http://rts.tanke756.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eet.ydjk.org.cn

PHP:  file_get_contents("a.txt");
来源：http://btz.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mqu.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://neu.zycfv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hvd.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tqm.gaohongyu789.top

Ruby: File.read("a.txt")
来源：http://nxq.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://tvw.shanyushiyangkeji.top

[F02] 逐行读取文件
来源：http://xbn.pycfn.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://klj.nwbrower.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wyy.9152youxi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dsh.uphjek.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ffs.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yiu.ppjwa.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gyn.jinghuilouyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jai.hongshengwenyu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rrx.ywan-chungtsiang.top

[F03] 写入文件（覆盖）
来源：http://yjf.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dyb.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://sid.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nqq.chenjidiqi.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fun.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ogz.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mlx.cdnleiting.top

Ruby: File.write("a.txt", "hi")
来源：http://ekj.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ovk.aizwys.cn

[F04] 追加写入文件
来源：http://tlh.jqgfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rgi.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qze.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ebz.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tqs.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mxq.guannengcc.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ldd.dashuyun.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yvd.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qwc.zhengqikj.top

[F05] 判断文件或目录是否存在
来源：http://img.hfpthk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://owo.yuxming.cn

PHP:  file_exists("a.txt");
来源：http://inp.jqgufenzy.top

JS:   fs.existsSync("a.txt")
来源：http://kjv.xinyue.icu

TS:   fs.existsSync("a.txt")
来源：http://ifk.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vcw.ydjk.org.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://njr.pengpengdd.cyou

Ruby: File.exist?("a.txt")
来源：http://eft.jinyuanbaomall.cn

C#:   File.Exists("a.txt")
来源：http://gpn.yongpay.top

[F06] 删除文件
来源：http://ddf.birdmap.top

Py:   os.remove("a.txt")
来源：http://hbp.haohaochexian.top

PHP:  unlink("a.txt");
来源：http://bex.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://uwo.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://ytp.svipenyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bxz.xuetiantiany.cn

Go:   os.Remove("a.txt")
来源：http://kao.meibo888.top

Ruby: File.delete("a.txt")
来源：http://gwg.hnxiangtu.top

C#:   File.Delete("a.txt");
来源：http://act.hesvh.cn

[F07] 创建目录（含多级）
来源：http://gzb.zhengqikj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aox.jinghuilouyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rjq.redwolf501.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sad.yuanzhike.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uvz.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lmg.hammf.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nqm.hfpthk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blv.zhongyouzk.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yld.sxryk.cn

[F08] 遍历目录
来源：http://unz.9152youxi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bvh.havefunace.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fmd.daxiang520.top

JS:   fs.readdirSync("dir")
来源：http://ppf.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://fwk.chenzaomai.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wpy.aibaodan.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qfy.cheryme.top

Ruby: Dir.children("dir")
来源：http://pet.hongshengwenyu.top

C#:   Directory.GetFiles("dir")
来源：http://giw.wangdashe.top

[F09] 获取文件大小
来源：http://hms.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://sxr.dianchejie.cn

PHP:  filesize("a.txt");
来源：http://czw.sjlbkw.cn

JS:   fs.statSync("a.txt").size
来源：http://bof.52xcode.cn

TS:   fs.statSync("a.txt").size
来源：http://emu.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zwd.zhaomingkeji.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dkc.havefunace.top

Ruby: File.size("a.txt")
来源：http://ilo.sjlbkw.cn

C#:   new FileInfo("a.txt").Length
来源：http://vri.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://epf.jiagoushi.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://snq.gaohongyu789.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nkf.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eqt.yvedp.cn

TS:   path.extname("a.txt")
来源：http://rfd.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zcf.wangdashe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://epq.ydjk.org.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uof.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lpg.zhengqikj.top

[F11] 复制与移动文件
来源：http://mtq.epnwcf.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://anz.shzxlz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fww.hesvh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rwc.yfazqb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sfu.feifeiyinyue.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lbd.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qnc.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pxe.yonumen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qxw.tarul.cn

[F12] CSV 读写
来源：http://cwl.cheryme.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oop.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tjl.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gdn.smart0.xyz

TS:   // 同上
来源：http://amp.jinqigufen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vpi.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iit.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://urm.dianchejie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gfv.shuidangran.top

================================================================================
来源：http://wwc.zhengqikj.top

G. 面向对象
来源：http://dcq.jinqigfzy.top

================================================================================
来源：http://mbq.wangshuangyany.cn

[G01] 定义类
来源：http://msk.havefunace.top

Py:   class User: pass
来源：http://sws.tarul.cn

PHP:  class User {}
来源：http://ksd.hywenlv.cn

JS:   class User {}
来源：http://qlu.cucudq.cn

TS:   class User { name: string = ""; }
来源：http://wch.cucudq.cn

Java: class User {}
来源：http://jho.hcnkem.com

Go:   type User struct { Name string }
来源：http://wua.hnxiangtu.top

Ruby: class User; end
来源：http://ejy.pycfn.com

C#:   class User {}
来源：http://cbl.xziqi.cn

[G02] 构造函数
来源：http://qbk.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://ccf.pengpengdd.cyou

PHP:  public function __construct(public string $name) {}
来源：http://dwm.yvedp.cn

JS:   constructor(name) { this.name = name; }
来源：http://gee.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://emf.jqgfzy.top

Java: User(String name) { this.name = name; }
来源：http://heh.tianlin.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bmt.jianghu66.top

Ruby: def initialize(name); @name = name; end
来源：http://ovd.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://fey.cheryme.top

[G03] 实例属性
来源：http://bme.tian-w.cn

Py:   self.name = "x"
来源：http://biv.9152youxi.cn

PHP:  public string $name = "x";
来源：http://pfb.shanyushiyangtech.top

JS:   this.name = "x";
来源：http://jnp.hywenlv.cn

TS:   name: string = "x";
来源：http://dmd.nwbrower.top

Java: private String name;
来源：http://cfr.c1oappe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xaa.cashguo.top

Ruby: @name = "x"
来源：http://xsk.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://jqd.cashguo.top

[G04] 定义方法
来源：http://osz.hammf.cn

Py:   def greet(self): return self.name
来源：http://jeo.redwolf501.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cvl.cucudq.cn

JS:   greet() { return this.name; }
来源：http://dto.jianghu66.top

TS:   greet(): string { return this.name; }
来源：http://cfe.9152youxi.cn

Java: String greet() { return name; }
来源：http://hxa.nanxinkj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hxa.jianghu66.top

Ruby: def greet; @name; end
来源：http://evv.shanyushiyangkeji.top

C#:   public string Greet() => Name;
来源：http://ghp.ywan-chungtsiang.top

[G05] 继承
来源：http://xet.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://emu.gotoacloud.top

PHP:  class Admin extends User {}
来源：http://jwq.jinyuanbaomall.cn

JS:   class Admin extends User {}
来源：http://jyi.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://oeb.zycfv.cn

Java: class Admin extends User {}
来源：http://gir.kuanghao11.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zkd.guannengcc.top

Ruby: class Admin < User; end
来源：http://feg.fktsv.cn

C#:   class Admin : User {}
来源：http://zlg.chenzaomai.com

[G06] 重写方法
来源：http://lpp.yvedp.cn

Py:   def greet(self): return "admin"
来源：http://zoo.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vld.yuxming.cn

JS:   greet() { return "admin"; }
来源：http://bbf.bjfxy.top

TS:   greet(): string { return "admin"; }
来源：http://ugn.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://hny.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lik.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://nzo.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://zwm.52xcode.cn

[G07] 调用父类方法
来源：http://caw.chenzaomai.com

Py:   super().greet()
来源：http://cag.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://ars.hysaishi.cn

JS:   super.greet();
来源：http://flr.xuetiantiany.cn

TS:   super.greet();
来源：http://mpg.gogol.net.cn

Java: super.greet();
来源：http://vjv.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ors.havefunace.top

Ruby: super
来源：http://myj.sufxvd.cn

C#:   base.Greet();
来源：http://axy.daria6918.cn

[G08] 静态方法与属性
来源：http://zxq.fengsongda.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nnq.dianchejie.cn

PHP:  public static function f() {}
来源：http://pxu.xylfe.cn

JS:   static f() {}
来源：http://jse.chenjidiqi.icu

TS:   static f(): void {}
来源：http://bwi.guannengcc.top

Java: static void f() {}
来源：http://wwl.kuanghao11.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ssu.ivvv.top

Ruby: def self.f; end
来源：http://pjy.shangyingyoupin.top

C#:   public static void F() {}
来源：http://sqd.316326.xyz

[G09] 接口 / 抽象类
来源：http://uwv.hywenlv.cn

Py:   from abc import ABC, abstractmethod
来源：http://oja.feifeiyinyue.top

PHP:  interface Shape { public function area(): float; }
来源：http://krz.shangyingyoupin.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bbh.c1oappe.top

TS:   interface Shape { area(): number; }
来源：http://zze.gotoacloud.top

Java: interface Shape { double area(); }
来源：http://jdm.xingfuxueyuan.xyz

Go:   type Shape interface { Area() float64 }
来源：http://yfr.shanyushiyangtech.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kjo.kuanghao11.cn

C#:   interface IShape { double Area(); }
来源：http://qob.316326.xyz

[G10] 访问控制
来源：http://yje.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://kbs.zycfv.cn

PHP:  public / protected / private
来源：http://iqs.sweek.top

JS:   #private 字段；其余公开
来源：http://den.wangshuangyany.cn

TS:   public / protected / private
来源：http://xwa.yj20258888.top

Java: public / protected / private / 默认包级
来源：http://pri.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://qif.andypj.xyz

Ruby: public / protected / private
来源：http://eoe.daxiang520.top

C#:   public / protected / private / internal
来源：http://lmj.smart0.xyz

[G11] getter / setter
来源：http://mma.jyoumei.cn

Py:   @property 与 @x.setter
来源：http://uih.gaohongyu789.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pmc.uphjek.com

JS:   get name() { return this._name; }
来源：http://ccm.xylfe.cn

TS:   get name(): string { return this._name; }
来源：http://azm.xinyue.icu

Java: public String getName() { return name; }
来源：http://ldb.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jaw.jinqigufen.top

Ruby: attr_accessor :name
来源：http://quc.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://imp.0kj1m.cn

[G12] 对象转字符串
来源：http://ozs.0kj1m.cn

Py:   def __str__(self): return self.name
来源：http://cbm.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mkx.jinqigfzy.top

JS:   toString() { return this.name; }
来源：http://scb.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://fig.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://ryw.dashuyun.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hgy.shzxlz.cn

Ruby: def to_s; @name; end
来源：http://ccy.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://tjp.jianghu66.top

[G13] 判断对象类型
来源：http://irn.zhengqikj.top

Py:   isinstance(u, User)
来源：http://eyw.dianchejie.cn

PHP:  $u instanceof User
来源：http://kwd.sweek.top

JS:   u instanceof User
来源：http://kbx.sufxvd.cn

TS:   u instanceof User
来源：http://dks.smart0.xyz

Java: u instanceof User
来源：http://jsr.epnwcf.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://deo.zdqjudy.top

Ruby: u.is_a?(User)
来源：http://lmw.quarkkingdee.top

C#:   u is User
来源：http://otv.nanxuanxn.top

[G14] 数据类 / record
来源：http://tkc.zhixingplan.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iqq.yangfankeji.com

PHP:  // 用 readonly 属性模拟
来源：http://akc.ydzc1.top

JS:   // 无内置：普通类或对象字面量
来源：http://omg.jiagoushi.top

TS:   type User = { name: string; age: number };
来源：http://mxl.zycfv.cn

Java: record User(String name, int age) {}
来源：http://uvn.nwbrower.top

Go:   type User struct { Name string; Age int }
来源：http://cts.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://peb.hcnkem.com

C#:   record User(string Name, int Age);
来源：http://jke.tianlin.xyz

[G15] 枚举
来源：http://hac.jianghu66.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qkh.ppjwa.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cwm.daxiang520.top


<!-- 参考信息 -->
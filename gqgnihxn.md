代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jtc.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://yrd.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pim.ywan-chungtsiang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vkz.cucudq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ccd.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zjb.pycfn.com

Ruby: s.capitalize
来源：http://jsr.ehwqpu.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gem.jinghuilouyu.cn

[E18] 模板占位符替换
来源：http://srw.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kzm.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hwp.sysykeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ogp.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ubq.jianghu66.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bmq.316326.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://viv.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ijp.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jzp.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://tes.pycfn.com

Py:   s.splitlines()
来源：http://htw.shuidangran.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yit.snrcjt.cn

JS:   s.split(/\r?\n/)
来源：http://sjo.ppjwa.cn

TS:   s.split(/\r?\n/)
来源：http://phl.c1oappe.top

Java: s.lines().toList()
来源：http://anz.fktsv.cn

Go:   strings.Split(s, "\n")
来源：http://trd.yj202588.top

Ruby: s.lines
来源：http://dss.zhengqikj.top

C#:   s.Split('\n')
来源：http://ibd.xylfe.cn

[E20] 判断字符串是否为空
来源：http://uhi.jlsjyb.cn

Py:   if not s:
来源：http://kye.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lvb.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xlx.jqgfzy.top

TS:   if (s === "") {}
来源：http://cgw.pengpengdd.cyou

Java: if (s.isEmpty()) {}
来源：http://rrh.jianghu66.top

Go:   if s == "" {}
来源：http://dgr.jqgufenzy.top

Ruby: if s.empty?
来源：http://weg.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kcw.gogol.net.cn

[E21] 超长截断加省略号
来源：http://tep.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bak.yanxiufei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mtb.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://thh.52xcode.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kbd.chenjidiqi.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vni.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://uim.ehwqpu.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jkf.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zxu.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://cfu.bjfxy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xue.yuanzhike.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dsm.chenlongwang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gav.bjfxy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ief.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rwv.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iak.gzhubu.top

Ruby: s.bytesize;  s.length
来源：http://svq.zdbjq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qkm.yj20258888.top

================================================================================
来源：http://pqv.nanxuanxn.top

F. 文件与目录
来源：http://mdo.xingfuxueyuan.xyz

================================================================================
来源：http://sth.aibaodan.cn

[F01] 读取整个文件
来源：http://arl.jianghu66.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dfp.xinyue.icu

PHP:  file_get_contents("a.txt");
来源：http://qhh.316326.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rpj.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bbo.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://etd.gogol.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dsa.ydjk.org.cn

Ruby: File.read("a.txt")
来源：http://ziv.tianlin.xyz

C#:   File.ReadAllText("a.txt");
来源：http://ykp.xingfuxueyuan.xyz

[F02] 逐行读取文件
来源：http://zbp.zycfv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xyg.ehwqpu.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fyy.ehwqpu.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jys.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tbz.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ejb.shanyushiyangtech.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bjf.quarkkingdee.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rqg.shanyushiyangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nql.meibo888.top

[F03] 写入文件（覆盖）
来源：http://svz.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://amq.hcnkem.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://sgr.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kox.daxiang520.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gtm.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ubj.jqgufenzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ycb.jinghuilouyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://dfl.guowangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xtu.shanyushiyangtech.top

[F04] 追加写入文件
来源：http://irs.epnwcf.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cmr.ydjk.org.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bsu.ybcxt.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kdp.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://luh.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nox.pycfn.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://inv.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lwt.jinqigufen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gwx.jinghuilouyu.cn

[F05] 判断文件或目录是否存在
来源：http://sjy.iojbl.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aym.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://hmr.shangyingyoupin.top

JS:   fs.existsSync("a.txt")
来源：http://kfz.sufxvd.cn

TS:   fs.existsSync("a.txt")
来源：http://dnr.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jxm.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wwg.birdmap.top

Ruby: File.exist?("a.txt")
来源：http://vrb.yvedp.cn

C#:   File.Exists("a.txt")
来源：http://mdn.jiagoushi.top

[F06] 删除文件
来源：http://klw.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://tai.cucudq.cn

PHP:  unlink("a.txt");
来源：http://yyy.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://qgo.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://csl.uphjek.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ilp.hywenlv.cn

Go:   os.Remove("a.txt")
来源：http://cuh.gotoacloud.top

Ruby: File.delete("a.txt")
来源：http://plc.daria6918.cn

C#:   File.Delete("a.txt");
来源：http://xrj.tarul.cn

[F07] 创建目录（含多级）
来源：http://aht.zhengqikj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fyf.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aur.gotoacloud.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sbv.cashguo.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kst.sjlbkw.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kom.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ida.andypj.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://naf.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ksn.yangfankeji.com

[F08] 遍历目录
来源：http://xci.yonumen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://krd.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fnt.yj202588.top

JS:   fs.readdirSync("dir")
来源：http://qbx.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://vec.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fxo.fehbvm.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://hvo.ivvv.top

Ruby: Dir.children("dir")
来源：http://tem.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://qkx.hnqzz.top

[F09] 获取文件大小
来源：http://hzh.zhixingplan.top

Py:   os.path.getsize("a.txt")
来源：http://oyw.smart0.xyz

PHP:  filesize("a.txt");
来源：http://fyw.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://wek.feifeiyinyue.top

TS:   fs.statSync("a.txt").size
来源：http://wdb.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://lnv.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pfj.yonumen.top

Ruby: File.size("a.txt")
来源：http://gnj.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://ajx.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://mdn.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://czk.jlsjyb.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rwq.chenjidiqi.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kzs.shuidangran.top

TS:   path.extname("a.txt")
来源：http://bei.0kj1m.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qtj.bbcook.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xwp.cdnleiting.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mkv.gogol.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vss.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://mnt.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pig.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://svi.aizwys.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xqx.snrcjt.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uhq.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://znk.jqgfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ams.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://opj.gogol.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tli.cashguo.top

[F12] CSV 读写
来源：http://vtd.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hpl.gogol.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bax.sxryk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fng.fktsv.cn

TS:   // 同上
来源：http://qci.xinyue.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zzm.zhaomingkeji.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vpl.fehbvm.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uhw.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://cat.fehbvm.com

================================================================================
来源：http://xsg.zhiwuduotai.top

G. 面向对象
来源：http://ryy.c1oappe.top

================================================================================
来源：http://ofw.zhoulong.xyz

[G01] 定义类
来源：http://fnd.zhongyouzk.top

Py:   class User: pass
来源：http://bsi.hywenlv.cn

PHP:  class User {}
来源：http://vzt.ywan-chungtsiang.top

JS:   class User {}
来源：http://fvs.52xcode.cn

TS:   class User { name: string = ""; }
来源：http://eql.bjfxy.top

Java: class User {}
来源：http://ujm.daxiang520.top

Go:   type User struct { Name string }
来源：http://ehk.yanxiufei.cn

Ruby: class User; end
来源：http://des.chenzaomai.com

C#:   class User {}
来源：http://iia.hcnkem.com

[G02] 构造函数
来源：http://ymm.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://rrb.redwolf501.top

PHP:  public function __construct(public string $name) {}
来源：http://lbu.9152youxi.cn

JS:   constructor(name) { this.name = name; }
来源：http://jpw.ppjwa.cn

TS:   constructor(public name: string) {}
来源：http://ypi.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://zcu.ybcxt.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://anl.316326.xyz

Ruby: def initialize(name); @name = name; end
来源：http://rfq.shangyingyoupin.top

C#:   public User(string name) { Name = name; }
来源：http://niv.xuetiantiany.cn

[G03] 实例属性
来源：http://fja.bjfxy.top

Py:   self.name = "x"
来源：http://pqr.yonumen.top

PHP:  public string $name = "x";
来源：http://hen.fzhhl.top

JS:   this.name = "x";
来源：http://rlv.snrcjt.cn

TS:   name: string = "x";
来源：http://vcy.hywenlv.cn

Java: private String name;
来源：http://zov.nanxinkj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fyn.feifeiyinyue.top

Ruby: @name = "x"
来源：http://vka.andypj.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ymg.daria6918.cn

[G04] 定义方法
来源：http://bve.xziqi.cn

Py:   def greet(self): return self.name
来源：http://nre.hysaishi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uoq.cashguo.top

JS:   greet() { return this.name; }
来源：http://yuz.gzhubu.top

TS:   greet(): string { return this.name; }
来源：http://kgd.andypj.xyz

Java: String greet() { return name; }
来源：http://rnz.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jxt.daxiang520.top

Ruby: def greet; @name; end
来源：http://wew.daxiang520.top

C#:   public string Greet() => Name;
来源：http://ooo.jinqigfzy.top

[G05] 继承
来源：http://agv.xziqi.cn

Py:   class Admin(User): pass
来源：http://tdd.yongpay.top

PHP:  class Admin extends User {}
来源：http://oem.iojbl.cn

JS:   class Admin extends User {}
来源：http://wph.sweek.top

TS:   class Admin extends User {}
来源：http://oox.hfpthk.cn

Java: class Admin extends User {}
来源：http://tcg.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jhe.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://yel.cdnleiting.top

C#:   class Admin : User {}
来源：http://sox.yueranfly.top

[G06] 重写方法
来源：http://mmc.quarkkingdee.top

Py:   def greet(self): return "admin"
来源：http://eqv.gogol.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://goi.iojbl.cn

JS:   greet() { return "admin"; }
来源：http://tne.ydzc1.top

TS:   greet(): string { return "admin"; }
来源：http://dkk.zdqjudy.top

Java: @Override String greet() { return "admin"; }
来源：http://dyc.jqgufenzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jlh.zhoulong.xyz

Ruby: def greet; "admin"; end
来源：http://tzc.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://ctn.fktsv.cn

[G07] 调用父类方法
来源：http://rcy.kuanghao11.cn

Py:   super().greet()
来源：http://vdx.aibaodan.cn

PHP:  parent::greet();
来源：http://gsg.nanxuanxn.top

JS:   super.greet();
来源：http://lby.yfazqb.com

TS:   super.greet();
来源：http://pre.tanke756.top

Java: super.greet();
来源：http://hjs.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ogh.uphjek.com

Ruby: super
来源：http://qlz.ivvv.top

C#:   base.Greet();
来源：http://ans.pengpengdd.cyou

[G08] 静态方法与属性
来源：http://jjt.zycfv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://duu.fehbvm.com

PHP:  public static function f() {}
来源：http://ucy.jqgfzy.top

JS:   static f() {}
来源：http://onw.pycfn.com

TS:   static f(): void {}
来源：http://wjm.xziqi.cn

Java: static void f() {}
来源：http://qli.yuxming.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rda.mhx1999.top

Ruby: def self.f; end
来源：http://tdt.fanxiaobao.xyz

C#:   public static void F() {}
来源：http://ogf.nanxuanxn.top

[G09] 接口 / 抽象类
来源：http://uxu.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://cbj.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://aeu.vehdjk.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://cbs.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://zws.316326.xyz

Java: interface Shape { double area(); }
来源：http://qzy.svipenyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://zas.zhiwuduotai.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wuu.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://ndi.yvedp.cn

[G10] 访问控制
来源：http://qkz.ctjpmb.com

Py:   约定 _protected / __private（不强制）
来源：http://umt.shangyingyoupin.top

PHP:  public / protected / private
来源：http://jyh.guowangkeji.top

JS:   #private 字段；其余公开
来源：http://hhu.jinghuilouyu.cn

TS:   public / protected / private
来源：http://hwo.gotoacloud.top

Java: public / protected / private / 默认包级
来源：http://mqs.fengsongda.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rhw.cdnleiting.top

Ruby: public / protected / private
来源：http://kod.ybcxt.top

C#:   public / protected / private / internal
来源：http://cbr.quarkkingdee.top

[G11] getter / setter
来源：http://amv.jlsjyb.cn

Py:   @property 与 @x.setter
来源：http://wfq.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://owx.vqdsnc.cn

JS:   get name() { return this._name; }
来源：http://ubp.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://auf.meibo888.top

Java: public String getName() { return name; }
来源：http://bvi.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xyy.hnqzz.top

Ruby: attr_accessor :name
来源：http://qat.shzxlz.cn

C#:   public string Name { get; set; }
来源：http://gli.svipenyu.cn

[G12] 对象转字符串
来源：http://gsp.jqgufenzy.top

Py:   def __str__(self): return self.name
来源：http://qew.52xcode.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vui.nwbrower.top

JS:   toString() { return this.name; }
来源：http://iht.nanxuanxn.top

TS:   toString(): string { return this.name; }
来源：http://ien.guannengcc.top

Java: @Override public String toString() { return name; }
来源：http://zmc.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://wza.uphjek.com

Ruby: def to_s; @name; end
来源：http://ope.mhx1999.top

C#:   public override string ToString() => Name;
来源：http://mcx.hnxiangtu.top

[G13] 判断对象类型
来源：http://zch.shanyushiyangtech.top

Py:   isinstance(u, User)
来源：http://fqf.iojbl.cn

PHP:  $u instanceof User
来源：http://yfd.chenlongwang.top

JS:   u instanceof User
来源：http://mto.cashguo.top

TS:   u instanceof User
来源：http://snq.birdmap.top

Java: u instanceof User
来源：http://ljp.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://obo.guannengcc.top

Ruby: u.is_a?(User)
来源：http://cvq.cashguo.top

C#:   u is User
来源：http://olg.ivvv.top

[G14] 数据类 / record
来源：http://xku.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fbv.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://atf.jinqigufen.top

JS:   // 无内置：普通类或对象字面量
来源：http://tbf.chenzaomai.com

TS:   type User = { name: string; age: number };
来源：http://tya.pengpengdd.cyou

Java: record User(String name, int age) {}
来源：http://cfh.vqdsnc.cn

Go:   type User struct { Name string; Age int }
来源：http://csc.guannengcc.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cgu.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://ezw.bbcook.cn

[G15] 枚举
来源：http://cdr.jinqigfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://whd.hnqzz.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qia.xuetiantiany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://foe.kuanghao11.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ozr.fanxiaobao.xyz

Java: enum Color { RED, GREEN }
来源：http://ltv.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bfr.dashuyun.cn


<!-- 参考信息 -->
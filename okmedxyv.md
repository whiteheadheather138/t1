代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fat.52xcode.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gkk.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://lir.tianlin.xyz

[E17] 首字母大写
来源：http://elj.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sqd.jinqigfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hde.chenjidiqi.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://txe.fanxiaobao.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xoo.hywenlv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qhl.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oor.9152youxi.cn

Ruby: s.capitalize
来源：http://qml.fehbvm.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gwu.ehwqpu.com

[E18] 模板占位符替换
来源：http://vla.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qgh.yuxming.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oxv.birdmap.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wtj.jinghuilouyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zkg.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cej.hfpthk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nws.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fji.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vrs.vqdsnc.cn

[E19] 多行文本按行拆分
来源：http://nse.cucudq.cn

Py:   s.splitlines()
来源：http://lxw.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ulh.chenzaomai.com

JS:   s.split(/\r?\n/)
来源：http://fco.jinqigufen.top

TS:   s.split(/\r?\n/)
来源：http://nad.zhengqikj.top

Java: s.lines().toList()
来源：http://zgb.ppjwa.cn

Go:   strings.Split(s, "\n")
来源：http://bpw.jlsjyb.cn

Ruby: s.lines
来源：http://vnx.bbcook.cn

C#:   s.Split('\n')
来源：http://uqm.aibaodan.cn

[E20] 判断字符串是否为空
来源：http://xlk.iojbl.cn

Py:   if not s:
来源：http://ect.0kj1m.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cyi.yanxiufei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kvk.cheryme.top

TS:   if (s === "") {}
来源：http://arl.pengpengdd.cyou

Java: if (s.isEmpty()) {}
来源：http://nhn.chenzaomai.com

Go:   if s == "" {}
来源：http://dvm.hysaishi.cn

Ruby: if s.empty?
来源：http://vlj.yj20258888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uel.316326.xyz

[E21] 超长截断加省略号
来源：http://jpg.havefunace.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tjc.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hzd.yangfankeji.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pxt.sjlbkw.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://exe.zhongyouzk.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gbk.aizwys.cn

Go:   // 按 rune 判断长度后截断
来源：http://wkm.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eou.aibaodan.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ocw.quarkkingdee.top

[E22] 字节长度与字符长度
来源：http://wlq.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gof.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bwu.nanxinkj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qew.jinyuanbaomall.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lkx.aibaodan.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mer.epnwcf.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://srj.dianchejie.cn

Ruby: s.bytesize;  s.length
来源：http://lkk.hfpthk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hgz.havefunace.top

================================================================================
来源：http://dlb.iojbl.cn

F. 文件与目录
来源：http://ycs.haohaochexian.top

================================================================================
来源：http://bay.c1oappe.top

[F01] 读取整个文件
来源：http://tts.xylfe.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gwi.zhiwuduotai.top

PHP:  file_get_contents("a.txt");
来源：http://zpt.jinyuanbaomall.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mwu.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fix.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://kec.jyoumei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fvw.yonumen.top

Ruby: File.read("a.txt")
来源：http://vmd.sjlbkw.cn

C#:   File.ReadAllText("a.txt");
来源：http://dqv.xinyue.icu

[F02] 逐行读取文件
来源：http://qxj.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wod.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sxt.sxryk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lax.316326.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pqu.snrcjt.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://axo.hfpthk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://snl.tian-w.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qdc.fehbvm.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qwq.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://dol.zhoulong.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kxe.bjfxy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lpk.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xmn.smart0.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bog.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ben.cqqwz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rlk.yangfankeji.com

Ruby: File.write("a.txt", "hi")
来源：http://iwy.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ger.havefunace.top

[F04] 追加写入文件
来源：http://ctn.guowangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xbj.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dtk.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kkj.ppjwa.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wea.hfpthk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lkr.9152youxi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oxt.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tyl.jiagoushi.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pzh.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://qfl.iojbl.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ojr.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://wze.epnwcf.com

JS:   fs.existsSync("a.txt")
来源：http://pza.meibo888.top

TS:   fs.existsSync("a.txt")
来源：http://att.fanxiaobao.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://bbe.cheryme.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wrg.bjfxy.top

Ruby: File.exist?("a.txt")
来源：http://rgy.c1oappe.top

C#:   File.Exists("a.txt")
来源：http://sad.ydzc1.top

[F06] 删除文件
来源：http://ack.kuanghao11.cn

Py:   os.remove("a.txt")
来源：http://whn.vehdjk.com

PHP:  unlink("a.txt");
来源：http://xna.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uva.xuanzx.com

TS:   fs.unlinkSync("a.txt")
来源：http://muc.dianchejie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fyt.zhongyouzk.top

Go:   os.Remove("a.txt")
来源：http://tvj.nwbrower.top

Ruby: File.delete("a.txt")
来源：http://trw.xinyue.icu

C#:   File.Delete("a.txt");
来源：http://wiu.xinyue.icu

[F07] 创建目录（含多级）
来源：http://aeb.jinqigfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fbb.tanke756.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vbh.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zti.bbcook.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://odp.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qjz.jianghu66.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lxt.dianchejie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fle.zhaomingkeji.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://van.guannengcc.top

[F08] 遍历目录
来源：http://ffs.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qnn.ydjk.org.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://goc.xinyue.icu

JS:   fs.readdirSync("dir")
来源：http://gab.wangshuangyany.cn

TS:   fs.readdirSync("dir")
来源：http://kwo.ivvv.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wch.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://qek.shzxlz.cn

Ruby: Dir.children("dir")
来源：http://xyx.sufxvd.cn

C#:   Directory.GetFiles("dir")
来源：http://phz.epnwcf.com

[F09] 获取文件大小
来源：http://bxn.hywenlv.cn

Py:   os.path.getsize("a.txt")
来源：http://bqx.daria6918.cn

PHP:  filesize("a.txt");
来源：http://jaz.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://ktg.bjfxy.top

TS:   fs.statSync("a.txt").size
来源：http://cpf.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fsd.0kj1m.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hqp.vqdsnc.cn

Ruby: File.size("a.txt")
来源：http://drb.nwbrower.top

C#:   new FileInfo("a.txt").Length
来源：http://dgi.0kj1m.cn

[F10] 取文件扩展名 / 文件名
来源：http://rog.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zrp.zhaomingkeji.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ljc.epnwcf.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://shr.mhx1999.top

TS:   path.extname("a.txt")
来源：http://jfq.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kgv.tanke756.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aqs.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vgm.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ukg.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://fne.xinyue.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://icu.chenzaomai.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://knq.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qge.shuidangran.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://crs.uphjek.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aza.uphjek.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wwr.ppjwa.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dab.feifeiyinyue.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tgf.wangdashe.top

[F12] CSV 读写
来源：http://jxb.hywenlv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gbs.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ici.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dmy.fehbvm.com

TS:   // 同上
来源：http://yjz.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eei.yangfankeji.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://luc.mhx1999.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mnv.jyoumei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xay.ivvv.top

================================================================================
来源：http://hhn.yj202588.top

G. 面向对象
来源：http://xxq.xinyue.icu

================================================================================
来源：http://bpk.zhiwuduotai.top

[G01] 定义类
来源：http://qqa.fehbvm.com

Py:   class User: pass
来源：http://tau.havefunace.top

PHP:  class User {}
来源：http://zpw.zhijiandao.cn

JS:   class User {}
来源：http://aqg.316326.xyz

TS:   class User { name: string = ""; }
来源：http://tdm.dianchejie.cn

Java: class User {}
来源：http://igx.shzxlz.cn

Go:   type User struct { Name string }
来源：http://hdj.mhx1999.top

Ruby: class User; end
来源：http://jbd.fktsv.cn

C#:   class User {}
来源：http://jto.havefunace.top

[G02] 构造函数
来源：http://upy.gogol.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://ypr.jinqigufen.top

PHP:  public function __construct(public string $name) {}
来源：http://pyl.ehwqpu.com

JS:   constructor(name) { this.name = name; }
来源：http://paa.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://fze.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://yku.hesvh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://myl.52xcode.cn

Ruby: def initialize(name); @name = name; end
来源：http://jwy.gaohongyu789.top

C#:   public User(string name) { Name = name; }
来源：http://plx.yuxming.cn

[G03] 实例属性
来源：http://kaq.yj202588.top

Py:   self.name = "x"
来源：http://eew.sweek.top

PHP:  public string $name = "x";
来源：http://nbx.yvedp.cn

JS:   this.name = "x";
来源：http://dml.yonumen.top

TS:   name: string = "x";
来源：http://gdv.snrcjt.cn

Java: private String name;
来源：http://sqe.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ztr.yj202588.top

Ruby: @name = "x"
来源：http://lce.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://bzy.xinyue.icu

[G04] 定义方法
来源：http://hel.dianchejie.cn

Py:   def greet(self): return self.name
来源：http://ofo.havefunace.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dtl.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://ydr.zycfv.cn

TS:   greet(): string { return this.name; }
来源：http://ure.guowangkeji.top

Java: String greet() { return name; }
来源：http://tfp.sxryk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qun.jianghu66.top

Ruby: def greet; @name; end
来源：http://siu.fengsongda.top

C#:   public string Greet() => Name;
来源：http://gnw.cashguo.top

[G05] 继承
来源：http://ipz.chenzaomai.com

Py:   class Admin(User): pass
来源：http://wsl.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://omc.ppjwa.cn

JS:   class Admin extends User {}
来源：http://kdo.jinqigufen.top

TS:   class Admin extends User {}
来源：http://zvs.xuanzx.com

Java: class Admin extends User {}
来源：http://ldw.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://usz.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://gle.xuanzx.com

C#:   class Admin : User {}
来源：http://pjo.zhiwuduotai.top

[G06] 重写方法
来源：http://jkm.ctjpmb.com

Py:   def greet(self): return "admin"
来源：http://rcl.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://goy.hnxiangtu.top

JS:   greet() { return "admin"; }
来源：http://oxa.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://hnl.daria6918.cn

Java: @Override String greet() { return "admin"; }
来源：http://kre.gzhubu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fml.yj20258.top

Ruby: def greet; "admin"; end
来源：http://dhv.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://oti.dashuyun.cn

[G07] 调用父类方法
来源：http://wmi.birdmap.top

Py:   super().greet()
来源：http://prh.svipenyu.cn

PHP:  parent::greet();
来源：http://dzt.shuidangran.top

JS:   super.greet();
来源：http://rax.redwolf501.top

TS:   super.greet();
来源：http://ltn.hfpthk.cn

Java: super.greet();
来源：http://jwa.yvedp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zyc.cqqwz.cn

Ruby: super
来源：http://uer.ydzc1.top

C#:   base.Greet();
来源：http://trf.yj20258.top

[G08] 静态方法与属性
来源：http://eqz.pengpengdd.cyou

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lmw.sweek.top

PHP:  public static function f() {}
来源：http://aky.nanxinkj.top

JS:   static f() {}
来源：http://ejl.cucudq.cn

TS:   static f(): void {}
来源：http://knf.aizwys.cn

Java: static void f() {}
来源：http://nid.zhijiandao.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dkv.epnwcf.com

Ruby: def self.f; end
来源：http://vlm.xinyue.icu

C#:   public static void F() {}
来源：http://huy.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://haw.hnqzz.top

Py:   from abc import ABC, abstractmethod
来源：http://lso.hysaishi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yiw.shzxlz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gvn.yfazqb.com

TS:   interface Shape { area(): number; }
来源：http://mab.chenlongwang.top

Java: interface Shape { double area(); }
来源：http://yuf.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://kuu.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vjw.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://uzc.sjlbkw.cn

[G10] 访问控制
来源：http://oqc.jinyuanbaomall.cn

Py:   约定 _protected / __private（不强制）
来源：http://ohh.daria6918.cn

PHP:  public / protected / private
来源：http://vac.jinyuanbaomall.cn

JS:   #private 字段；其余公开
来源：http://btg.zdqjudy.top

TS:   public / protected / private
来源：http://wlz.havefunace.top

Java: public / protected / private / 默认包级
来源：http://syt.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yaf.gotoacloud.top

Ruby: public / protected / private
来源：http://tpt.ehwqpu.com

C#:   public / protected / private / internal
来源：http://ozt.svipenyu.cn

[G11] getter / setter
来源：http://oun.hnqzz.top

Py:   @property 与 @x.setter
来源：http://oeq.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://blk.jqgufenzy.top

JS:   get name() { return this._name; }
来源：http://mne.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://vjt.tanke756.top

Java: public String getName() { return name; }
来源：http://sle.yvedp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://iss.ivvv.top

Ruby: attr_accessor :name
来源：http://ryp.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://tcy.hfpthk.cn

[G12] 对象转字符串
来源：http://zgw.zhaomingkeji.xyz

Py:   def __str__(self): return self.name
来源：http://eas.jinqigufen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yzt.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://evx.c1oappe.top

TS:   toString(): string { return this.name; }
来源：http://gom.vehdjk.com

Java: @Override public String toString() { return name; }
来源：http://eis.jqgufenzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://lgi.gzhubu.top

Ruby: def to_s; @name; end
来源：http://stk.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://mfk.hammf.cn

[G13] 判断对象类型
来源：http://hmv.aibaodan.cn

Py:   isinstance(u, User)
来源：http://tox.gzhubu.top

PHP:  $u instanceof User
来源：http://rcc.jinghuilouyu.cn

JS:   u instanceof User
来源：http://nhi.jinghuilouyu.cn

TS:   u instanceof User
来源：http://ifn.yj202588.top

Java: u instanceof User
来源：http://ubc.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dgf.hongshengwenyu.top

Ruby: u.is_a?(User)
来源：http://twa.nanxinkj.top

C#:   u is User
来源：http://vqs.c1oappe.top

[G14] 数据类 / record
来源：http://jqg.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qcl.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://jnq.daria6918.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tbi.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://sof.jianghu66.top

Java: record User(String name, int age) {}
来源：http://rxg.yongpay.top

Go:   type User struct { Name string; Age int }
来源：http://fqa.bbcook.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xna.pycfn.com

C#:   record User(string Name, int Age);
来源：http://ucw.ctjpmb.com

[G15] 枚举
来源：http://ktw.jinqigfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ocq.ctjpmb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://gsc.yongpay.top


<!-- 参考信息 -->
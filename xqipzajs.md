代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ipg.shangyingyoupin.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cdb.ivvv.top

Ruby: s.capitalize
来源：http://icr.havefunace.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ltt.yongpay.top

[E18] 模板占位符替换
来源：http://qea.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hxp.shangyingyoupin.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jrh.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gpm.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://iif.sysykeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vlm.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fyh.xingfuxueyuan.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wfx.cashguo.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bac.nanxuanxn.top

[E19] 多行文本按行拆分
来源：http://jml.cucudq.cn

Py:   s.splitlines()
来源：http://vrm.hywenlv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zdc.zhengqikj.top

JS:   s.split(/\r?\n/)
来源：http://ipw.c1oappe.top

TS:   s.split(/\r?\n/)
来源：http://odt.wangshuangyany.cn

Java: s.lines().toList()
来源：http://zwd.hywenlv.cn

Go:   strings.Split(s, "\n")
来源：http://lng.wangdashe.top

Ruby: s.lines
来源：http://gvb.9152youxi.cn

C#:   s.Split('\n')
来源：http://mts.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://scv.yueranfly.top

Py:   if not s:
来源：http://vqq.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dpy.fzhhl.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ygy.cashguo.top

TS:   if (s === "") {}
来源：http://wqp.tanke756.top

Java: if (s.isEmpty()) {}
来源：http://sef.fzhhl.top

Go:   if s == "" {}
来源：http://xcz.ctjpmb.com

Ruby: if s.empty?
来源：http://hmo.yanxiufei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wez.yongpay.top

[E21] 超长截断加省略号
来源：http://guj.jinqigfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ysf.yvedp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ndb.jianghu66.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bef.fengsongda.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dzg.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hrn.chenzaomai.com

Go:   // 按 rune 判断长度后截断
来源：http://lmv.fktsv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ole.sysykeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://imc.c1oappe.top

[E22] 字节长度与字符长度
来源：http://xjo.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bfg.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mkp.havefunace.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vrs.gotoacloud.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hbx.quarkkingdee.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dqg.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mtt.jinghuilouyu.cn

Ruby: s.bytesize;  s.length
来源：http://yju.nanxinkj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wdh.iojbl.cn

================================================================================
来源：http://vmk.yanxiufei.cn

F. 文件与目录
来源：http://hzq.xinyue.icu

================================================================================
来源：http://ttb.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://izg.mhx1999.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uwa.yj20258888.top

PHP:  file_get_contents("a.txt");
来源：http://cvx.wangdashe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tsj.yueranfly.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ivh.dianchejie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fhl.bjfxy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rvt.guannengcc.top

Ruby: File.read("a.txt")
来源：http://gbn.tarul.cn

C#:   File.ReadAllText("a.txt");
来源：http://bca.quarkkingdee.top

[F02] 逐行读取文件
来源：http://unq.chenjidiqi.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ewf.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mps.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://prw.cheryme.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fsf.smart0.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hbd.jinghuilouyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xuw.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fss.guowangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ofx.zhongyouzk.top

[F03] 写入文件（覆盖）
来源：http://zno.shangyingyoupin.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qre.pycfn.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://ozq.nwbrower.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://txd.smart0.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mvg.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tgm.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gyl.ywan-chungtsiang.top

Ruby: File.write("a.txt", "hi")
来源：http://ccj.yfazqb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://clx.cqqwz.cn

[F04] 追加写入文件
来源：http://oib.hcnkem.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://naf.bbcook.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mpp.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qaq.yonumen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xdm.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wsx.chenjidiqi.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tpp.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://afv.tianlin.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mff.nanxinkj.top

[F05] 判断文件或目录是否存在
来源：http://nch.gzhubu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ujg.guowangkeji.top

PHP:  file_exists("a.txt");
来源：http://aam.pycfn.com

JS:   fs.existsSync("a.txt")
来源：http://uic.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://yli.aizwys.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dzh.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jhk.0kj1m.cn

Ruby: File.exist?("a.txt")
来源：http://xpu.quarkkingdee.top

C#:   File.Exists("a.txt")
来源：http://eui.andypj.xyz

[F06] 删除文件
来源：http://frd.zhixingplan.top

Py:   os.remove("a.txt")
来源：http://wod.fktsv.cn

PHP:  unlink("a.txt");
来源：http://ynm.mhx1999.top

JS:   fs.unlinkSync("a.txt")
来源：http://pch.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://ctd.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fwu.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://yzc.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://zyn.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://taf.jinqigfzy.top

[F07] 创建目录（含多级）
来源：http://iur.yongpay.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sna.ywan-chungtsiang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ulz.zycfv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xkn.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qri.tianlin.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://auv.zhoulong.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ieo.dianchejie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vfn.shangyingyoupin.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://otc.bbcook.cn

[F08] 遍历目录
来源：http://lqq.fanxiaobao.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://dnt.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xhq.iojbl.cn

JS:   fs.readdirSync("dir")
来源：http://xhm.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://oad.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lvz.zhiwuduotai.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hbc.feifeiyinyue.top

Ruby: Dir.children("dir")
来源：http://knl.jinqigfzy.top

C#:   Directory.GetFiles("dir")
来源：http://qbw.yj20258888.top

[F09] 获取文件大小
来源：http://byq.wangshuangyany.cn

Py:   os.path.getsize("a.txt")
来源：http://djm.xziqi.cn

PHP:  filesize("a.txt");
来源：http://lkf.sweek.top

JS:   fs.statSync("a.txt").size
来源：http://qcy.yj20258.top

TS:   fs.statSync("a.txt").size
来源：http://tvt.zhijiandao.cn

Java: Files.size(Path.of("a.txt"))
来源：http://peu.shanyushiyangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ttf.snrcjt.cn

Ruby: File.size("a.txt")
来源：http://eax.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://zgu.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://vte.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dnn.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kox.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yaa.zdbjq.cn

TS:   path.extname("a.txt")
来源：http://teq.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hfi.xingfuxueyuan.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jcy.smart0.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xwf.zhiwuduotai.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vov.nwbrower.top

[F11] 复制与移动文件
来源：http://svw.xuanzx.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jjz.zhaomingkeji.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lyh.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rnw.nwbrower.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ktu.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jka.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qrt.bbcook.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bvf.xinyue.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zgd.jyoumei.cn

[F12] CSV 读写
来源：http://cny.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pyp.zhongyouzk.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mep.svipenyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ugj.ywan-chungtsiang.top

TS:   // 同上
来源：http://svr.pengpengdd.cyou

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://olj.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eig.zdbjq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://onc.yj20258.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lpq.shzxlz.cn

================================================================================
来源：http://hzl.kuanghao11.cn

G. 面向对象
来源：http://fyq.yuanzhike.top

================================================================================
来源：http://srv.zhixingplan.top

[G01] 定义类
来源：http://wvh.yuanzhike.top

Py:   class User: pass
来源：http://rwj.sweek.top

PHP:  class User {}
来源：http://jse.daxiang520.top

JS:   class User {}
来源：http://hyn.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://nqs.vehdjk.com

Java: class User {}
来源：http://xyt.zhengqikj.top

Go:   type User struct { Name string }
来源：http://lyz.52xcode.cn

Ruby: class User; end
来源：http://byy.guannengcc.top

C#:   class User {}
来源：http://iga.sufxvd.cn

[G02] 构造函数
来源：http://ggy.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://tip.shanyushiyangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://dgj.xingfuxueyuan.xyz

JS:   constructor(name) { this.name = name; }
来源：http://owz.zhaomingkeji.xyz

TS:   constructor(public name: string) {}
来源：http://jul.redwolf501.top

Java: User(String name) { this.name = name; }
来源：http://ciw.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iva.kuanghao11.cn

Ruby: def initialize(name); @name = name; end
来源：http://yxj.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://poa.tianlin.xyz

[G03] 实例属性
来源：http://wnk.jyoumei.cn

Py:   self.name = "x"
来源：http://gbq.wangdashe.top

PHP:  public string $name = "x";
来源：http://ylp.yanxiufei.cn

JS:   this.name = "x";
来源：http://svr.zycfv.cn

TS:   name: string = "x";
来源：http://ykw.pengpengdd.cyou

Java: private String name;
来源：http://yew.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vxe.redwolf501.top

Ruby: @name = "x"
来源：http://tfo.fengsongda.top

C#:   public string Name { get; set; } = "x";
来源：http://qyp.havefunace.top

[G04] 定义方法
来源：http://pyp.sufxvd.cn

Py:   def greet(self): return self.name
来源：http://mke.yueranfly.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rao.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://spm.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://uud.birdmap.top

Java: String greet() { return name; }
来源：http://akg.xylfe.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vyf.hnxiangtu.top

Ruby: def greet; @name; end
来源：http://ohy.snrcjt.cn

C#:   public string Greet() => Name;
来源：http://hgp.wangshuangyany.cn

[G05] 继承
来源：http://zuc.hammf.cn

Py:   class Admin(User): pass
来源：http://cgu.xingfuxueyuan.xyz

PHP:  class Admin extends User {}
来源：http://amw.dianchejie.cn

JS:   class Admin extends User {}
来源：http://hcm.yongpay.top

TS:   class Admin extends User {}
来源：http://iex.zycfv.cn

Java: class Admin extends User {}
来源：http://qba.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sxj.jqgufenzy.top

Ruby: class Admin < User; end
来源：http://whi.bbcook.cn

C#:   class Admin : User {}
来源：http://lpw.shanyushiyangkeji.top

[G06] 重写方法
来源：http://nyd.zhengqikj.top

Py:   def greet(self): return "admin"
来源：http://rnd.tian-w.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kxq.daxiang520.top

JS:   greet() { return "admin"; }
来源：http://mtf.vehdjk.com

TS:   greet(): string { return "admin"; }
来源：http://oal.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://jdo.hammf.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yxf.cucudq.cn

Ruby: def greet; "admin"; end
来源：http://dcd.gotoacloud.top

C#:   public override string Greet() => "admin";
来源：http://qnh.hnqzz.top

[G07] 调用父类方法
来源：http://fzb.sysykeji.top

Py:   super().greet()
来源：http://uuq.nwbrower.top

PHP:  parent::greet();
来源：http://fsb.gogol.net.cn

JS:   super.greet();
来源：http://oyp.hfpthk.cn

TS:   super.greet();
来源：http://eeb.jianghu66.top

Java: super.greet();
来源：http://nbi.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qlu.shangyingyoupin.top

Ruby: super
来源：http://lus.sweek.top

C#:   base.Greet();
来源：http://ouc.fzhhl.top

[G08] 静态方法与属性
来源：http://ofe.jianghu66.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ude.fengsongda.top

PHP:  public static function f() {}
来源：http://lzx.meibo888.top

JS:   static f() {}
来源：http://qye.shzxlz.cn

TS:   static f(): void {}
来源：http://cto.fengsongda.top

Java: static void f() {}
来源：http://loc.jiagoushi.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ynz.sysykeji.top

Ruby: def self.f; end
来源：http://ppl.zhixingplan.top

C#:   public static void F() {}
来源：http://wsb.ydzc1.top

[G09] 接口 / 抽象类
来源：http://tja.iojbl.cn

Py:   from abc import ABC, abstractmethod
来源：http://mph.zdqjudy.top

PHP:  interface Shape { public function area(): float; }
来源：http://zyc.havefunace.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zkz.tianlin.xyz

TS:   interface Shape { area(): number; }
来源：http://fak.shuidangran.top

Java: interface Shape { double area(); }
来源：http://byp.wangdashe.top

Go:   type Shape interface { Area() float64 }
来源：http://kqi.andypj.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cez.snrcjt.cn

C#:   interface IShape { double Area(); }
来源：http://amr.9152youxi.cn

[G10] 访问控制
来源：http://yyf.zhengqikj.top

Py:   约定 _protected / __private（不强制）
来源：http://fmt.cqqwz.cn

PHP:  public / protected / private
来源：http://oxi.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://esa.ctjpmb.com

TS:   public / protected / private
来源：http://yyj.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://ehc.kuanghao11.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lin.hesvh.cn

Ruby: public / protected / private
来源：http://gbc.yj202588.top

C#:   public / protected / private / internal
来源：http://qxt.gzhubu.top

[G11] getter / setter
来源：http://vhv.xinyue.icu

Py:   @property 与 @x.setter
来源：http://pdt.gzhubu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ogh.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://kgg.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://ipf.bjfxy.top

Java: public String getName() { return name; }
来源：http://zpv.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://npv.c1oappe.top

Ruby: attr_accessor :name
来源：http://ebh.gaohongyu789.top

C#:   public string Name { get; set; }
来源：http://gxb.52xcode.cn

[G12] 对象转字符串
来源：http://efd.jlsjyb.cn

Py:   def __str__(self): return self.name
来源：http://xkt.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zqi.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://bne.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://lgh.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://fuf.dashuyun.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kzj.tian-w.cn

Ruby: def to_s; @name; end
来源：http://zgz.nanxuanxn.top

C#:   public override string ToString() => Name;
来源：http://alj.yueranfly.top

[G13] 判断对象类型
来源：http://bwi.ydjk.org.cn

Py:   isinstance(u, User)
来源：http://drn.jinqigfzy.top

PHP:  $u instanceof User
来源：http://vrb.hysaishi.cn

JS:   u instanceof User
来源：http://zpw.smart0.xyz

TS:   u instanceof User
来源：http://hio.hfpthk.cn

Java: u instanceof User
来源：http://abf.zhaomingkeji.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://odz.xziqi.cn

Ruby: u.is_a?(User)
来源：http://pvi.jiagoushi.top

C#:   u is User
来源：http://jrg.meibo888.top

[G14] 数据类 / record
来源：http://mfp.yj20258888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sie.yj20258.top

PHP:  // 用 readonly 属性模拟
来源：http://kdr.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://rep.zhoulong.xyz

TS:   type User = { name: string; age: number };
来源：http://jge.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://eqv.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://qkg.pycfn.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://owj.snrcjt.cn

C#:   record User(string Name, int Age);
来源：http://pax.yj202588.top

[G15] 枚举
来源：http://ogw.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xrk.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bbk.sweek.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uhj.yueranfly.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nyb.feifeiyinyue.top

Java: enum Color { RED, GREEN }
来源：http://ujg.fktsv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bgz.fanxiaobao.xyz

Ruby: Color = %i[red green].freeze
来源：http://knq.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://brt.bbcook.cn

[G16] 对象转数组 / 字典
来源：http://hft.redwolf501.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jev.shangyingyoupin.top


<!-- 参考信息 -->
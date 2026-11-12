代发 wailian999

[E18] 模板占位符替换
来源：http://jho.svipenyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bxs.gaohongyu789.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qlj.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bvi.xuanzx.com

TS:   tpl.replaceAll("{name}", name)
来源：http://zrx.tianlin.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cta.shzxlz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zlk.sufxvd.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ylc.tanke756.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://akq.ydzc1.top

[E19] 多行文本按行拆分
来源：http://wep.ydzc1.top

Py:   s.splitlines()
来源：http://keu.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wja.bbcook.cn

JS:   s.split(/\r?\n/)
来源：http://kzr.sweek.top

TS:   s.split(/\r?\n/)
来源：http://fyy.feifeiyinyue.top

Java: s.lines().toList()
来源：http://gbi.dianchejie.cn

Go:   strings.Split(s, "\n")
来源：http://hcf.ywan-chungtsiang.top

Ruby: s.lines
来源：http://gdy.meibo888.top

C#:   s.Split('\n')
来源：http://gna.vehdjk.com

[E20] 判断字符串是否为空
来源：http://rch.ydjk.org.cn

Py:   if not s:
来源：http://ehw.nwbrower.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rgq.jinqigufen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kvc.shuidangran.top

TS:   if (s === "") {}
来源：http://ewl.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://yoj.jqgufenzy.top

Go:   if s == "" {}
来源：http://cws.sweek.top

Ruby: if s.empty?
来源：http://wfu.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nmy.tian-w.cn

[E21] 超长截断加省略号
来源：http://pxo.tarul.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lne.chenjidiqi.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qli.snrcjt.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uat.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wgw.fanxiaobao.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hfi.fehbvm.com

Go:   // 按 rune 判断长度后截断
来源：http://evd.gogol.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ngz.hcnkem.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dyf.yj202588.top

[E22] 字节长度与字符长度
来源：http://xho.mhx1999.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wgy.xziqi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kel.daria6918.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lle.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bpl.gaohongyu789.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hzw.fktsv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qmr.ydzc1.top

Ruby: s.bytesize;  s.length
来源：http://cng.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pgi.zycfv.cn

================================================================================
来源：http://yai.daxiang520.top

F. 文件与目录
来源：http://udp.zdbjq.cn

================================================================================
来源：http://qce.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://nby.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sih.iojbl.cn

PHP:  file_get_contents("a.txt");
来源：http://ddp.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ssg.fktsv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yup.shzxlz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ssj.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://shn.ivvv.top

Ruby: File.read("a.txt")
来源：http://cet.hnqzz.top

C#:   File.ReadAllText("a.txt");
来源：http://gtj.andypj.xyz

[F02] 逐行读取文件
来源：http://ubw.316326.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jtg.ivvv.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://urh.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wyu.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://owj.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ook.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wad.yueranfly.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iqq.gotoacloud.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wrt.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://bln.jlsjyb.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://chh.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://fdm.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jwe.pycfn.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gco.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lfo.316326.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bmz.vqdsnc.cn

Ruby: File.write("a.txt", "hi")
来源：http://hfj.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vuk.cucudq.cn

[F04] 追加写入文件
来源：http://zek.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kev.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ktb.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jcu.xziqi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tpa.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zvw.ehwqpu.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ail.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xfb.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zkk.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://mgf.hongshengwenyu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gnl.gzhubu.top

PHP:  file_exists("a.txt");
来源：http://tbj.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://uwo.fengsongda.top

TS:   fs.existsSync("a.txt")
来源：http://vji.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wyq.hongshengwenyu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aol.zhengqikj.top

Ruby: File.exist?("a.txt")
来源：http://jeh.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://gmh.pengpengdd.cyou

[F06] 删除文件
来源：http://gam.xuanzx.com

Py:   os.remove("a.txt")
来源：http://zid.xuetiantiany.cn

PHP:  unlink("a.txt");
来源：http://wft.shuidangran.top

JS:   fs.unlinkSync("a.txt")
来源：http://tgx.meibo888.top

TS:   fs.unlinkSync("a.txt")
来源：http://ebp.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lob.hysaishi.cn

Go:   os.Remove("a.txt")
来源：http://jgs.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://cpi.sxryk.cn

C#:   File.Delete("a.txt");
来源：http://syl.jiagoushi.top

[F07] 创建目录（含多级）
来源：http://rkd.zycfv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uqg.9152youxi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aia.xuanzx.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://myb.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://esz.cdnleiting.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zpy.shzxlz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://stn.quarkkingdee.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ndx.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fqi.yj20258.top

[F08] 遍历目录
来源：http://rov.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kyd.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://txt.hfpthk.cn

JS:   fs.readdirSync("dir")
来源：http://jxu.9152youxi.cn

TS:   fs.readdirSync("dir")
来源：http://ryt.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mji.sjlbkw.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ygz.tanke756.top

Ruby: Dir.children("dir")
来源：http://vue.uphjek.com

C#:   Directory.GetFiles("dir")
来源：http://rvt.xylfe.cn

[F09] 获取文件大小
来源：http://vto.andypj.xyz

Py:   os.path.getsize("a.txt")
来源：http://fnq.52xcode.cn

PHP:  filesize("a.txt");
来源：http://weg.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://clu.meibo888.top

TS:   fs.statSync("a.txt").size
来源：http://esh.yongpay.top

Java: Files.size(Path.of("a.txt"))
来源：http://rhv.52xcode.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fgb.yj20258.top

Ruby: File.size("a.txt")
来源：http://ghl.epnwcf.com

C#:   new FileInfo("a.txt").Length
来源：http://zup.tarul.cn

[F10] 取文件扩展名 / 文件名
来源：http://dxs.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jhy.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rce.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xnh.jiagoushi.top

TS:   path.extname("a.txt")
来源：http://kpq.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ezh.wangdashe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ldb.hongshengwenyu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ywr.jlsjyb.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gqs.snrcjt.cn

[F11] 复制与移动文件
来源：http://jes.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wdw.uphjek.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fnp.pengpengdd.cyou

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rxx.hysaishi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rhl.guannengcc.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gof.zdqjudy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jff.chenzaomai.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eke.zhongyouzk.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qpz.jlsjyb.cn

[F12] CSV 读写
来源：http://oqw.gotoacloud.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fim.jqgufenzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cfb.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://poa.svipenyu.cn

TS:   // 同上
来源：http://mim.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nqy.chenjidiqi.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zkf.xylfe.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qxi.jqgfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vwl.nanxuanxn.top

================================================================================
来源：http://wmo.ywan-chungtsiang.top

G. 面向对象
来源：http://bmt.shuidangran.top

================================================================================
来源：http://cub.bjfxy.top

[G01] 定义类
来源：http://mel.jiagoushi.top

Py:   class User: pass
来源：http://oji.jyoumei.cn

PHP:  class User {}
来源：http://izg.sysykeji.top

JS:   class User {}
来源：http://oiu.cheryme.top

TS:   class User { name: string = ""; }
来源：http://kcx.xuanzx.com

Java: class User {}
来源：http://eck.tianlin.xyz

Go:   type User struct { Name string }
来源：http://xhw.xinyue.icu

Ruby: class User; end
来源：http://dzf.guowangkeji.top

C#:   class User {}
来源：http://sij.kuanghao11.cn

[G02] 构造函数
来源：http://lkg.nanxinkj.top

Py:   def __init__(self, name): self.name = name
来源：http://cda.zhaomingkeji.xyz

PHP:  public function __construct(public string $name) {}
来源：http://vse.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://aiq.jinqigufen.top

TS:   constructor(public name: string) {}
来源：http://lnz.gogol.net.cn

Java: User(String name) { this.name = name; }
来源：http://zch.yj20258.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://isz.c1oappe.top

Ruby: def initialize(name); @name = name; end
来源：http://vle.fengsongda.top

C#:   public User(string name) { Name = name; }
来源：http://mhu.shzxlz.cn

[G03] 实例属性
来源：http://hap.yanxiufei.cn

Py:   self.name = "x"
来源：http://amw.ivvv.top

PHP:  public string $name = "x";
来源：http://oyg.fanxiaobao.xyz

JS:   this.name = "x";
来源：http://zks.yongpay.top

TS:   name: string = "x";
来源：http://ooj.guannengcc.top

Java: private String name;
来源：http://rxb.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pqk.fzhhl.top

Ruby: @name = "x"
来源：http://jlh.ivvv.top

C#:   public string Name { get; set; } = "x";
来源：http://shx.birdmap.top

[G04] 定义方法
来源：http://nwi.cucudq.cn

Py:   def greet(self): return self.name
来源：http://wuw.xinyue.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://ibh.iojbl.cn

JS:   greet() { return this.name; }
来源：http://qbi.xingfuxueyuan.xyz

TS:   greet(): string { return this.name; }
来源：http://uzp.quarkkingdee.top

Java: String greet() { return name; }
来源：http://jwp.gaohongyu789.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wop.tian-w.cn

Ruby: def greet; @name; end
来源：http://gkc.yueranfly.top

C#:   public string Greet() => Name;
来源：http://ahv.xuanzx.com

[G05] 继承
来源：http://sbq.gogol.net.cn

Py:   class Admin(User): pass
来源：http://jue.gogol.net.cn

PHP:  class Admin extends User {}
来源：http://ywu.feifeiyinyue.top

JS:   class Admin extends User {}
来源：http://slp.jinqigufen.top

TS:   class Admin extends User {}
来源：http://pgq.gotoacloud.top

Java: class Admin extends User {}
来源：http://ptq.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eyp.cucudq.cn

Ruby: class Admin < User; end
来源：http://cre.shuidangran.top

C#:   class Admin : User {}
来源：http://cjc.xuetiantiany.cn

[G06] 重写方法
来源：http://dfh.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://iww.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://cds.svipenyu.cn

JS:   greet() { return "admin"; }
来源：http://lfo.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://sjr.zhixingplan.top

Java: @Override String greet() { return "admin"; }
来源：http://crd.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jnw.cucudq.cn

Ruby: def greet; "admin"; end
来源：http://jdb.zhoulong.xyz

C#:   public override string Greet() => "admin";
来源：http://hqr.wangshuangyany.cn

[G07] 调用父类方法
来源：http://dnw.hnqzz.top

Py:   super().greet()
来源：http://tcw.jinyuanbaomall.cn

PHP:  parent::greet();
来源：http://jqn.tian-w.cn

JS:   super.greet();
来源：http://dgx.yfazqb.com

TS:   super.greet();
来源：http://ztn.zhaomingkeji.xyz

Java: super.greet();
来源：http://wwo.chenzaomai.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nve.uphjek.com

Ruby: super
来源：http://nkh.zycfv.cn

C#:   base.Greet();
来源：http://kzh.zycfv.cn

[G08] 静态方法与属性
来源：http://fmz.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ybq.snrcjt.cn

PHP:  public static function f() {}
来源：http://msq.yueranfly.top

JS:   static f() {}
来源：http://lcg.shanyushiyangtech.top

TS:   static f(): void {}
来源：http://txb.jianghu66.top

Java: static void f() {}
来源：http://mli.epnwcf.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://wsa.jinqigfzy.top

Ruby: def self.f; end
来源：http://xav.yfazqb.com

C#:   public static void F() {}
来源：http://oiz.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://jah.yj202588.top

Py:   from abc import ABC, abstractmethod
来源：http://lll.bjfxy.top

PHP:  interface Shape { public function area(): float; }
来源：http://gah.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://eau.zhiwuduotai.top

TS:   interface Shape { area(): number; }
来源：http://bta.tanke756.top

Java: interface Shape { double area(); }
来源：http://idj.zhaomingkeji.xyz

Go:   type Shape interface { Area() float64 }
来源：http://wwk.meibo888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cxd.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://kwj.yangfankeji.com

[G10] 访问控制
来源：http://yhw.gaohongyu789.top

Py:   约定 _protected / __private（不强制）
来源：http://bwx.aizwys.cn

PHP:  public / protected / private
来源：http://wgr.jinyuanbaomall.cn

JS:   #private 字段；其余公开
来源：http://pxx.haohaochexian.top

TS:   public / protected / private
来源：http://emo.daria6918.cn

Java: public / protected / private / 默认包级
来源：http://uaz.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hdq.vqdsnc.cn

Ruby: public / protected / private
来源：http://snk.fehbvm.com

C#:   public / protected / private / internal
来源：http://xdn.jyoumei.cn

[G11] getter / setter
来源：http://pyj.hysaishi.cn

Py:   @property 与 @x.setter
来源：http://jgs.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dut.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://ssz.epnwcf.com

TS:   get name(): string { return this._name; }
来源：http://jez.bbcook.cn

Java: public String getName() { return name; }
来源：http://twk.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gbx.hcnkem.com

Ruby: attr_accessor :name
来源：http://bwg.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://xak.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://mio.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://gmk.chenzaomai.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://wfx.vehdjk.com

JS:   toString() { return this.name; }
来源：http://wrg.hongshengwenyu.top

TS:   toString(): string { return this.name; }
来源：http://pfn.sweek.top

Java: @Override public String toString() { return name; }
来源：http://jve.haohaochexian.top

Go:   func (u User) String() string { return u.Name }
来源：http://chq.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://vzn.yuanzhike.top

C#:   public override string ToString() => Name;
来源：http://oup.daxiang520.top

[G13] 判断对象类型
来源：http://cjm.wangshuangyany.cn

Py:   isinstance(u, User)
来源：http://vjx.gogol.net.cn

PHP:  $u instanceof User
来源：http://cxv.shzxlz.cn

JS:   u instanceof User
来源：http://acb.shanyushiyangkeji.top

TS:   u instanceof User
来源：http://mqc.aibaodan.cn

Java: u instanceof User
来源：http://omu.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mst.redwolf501.top

Ruby: u.is_a?(User)
来源：http://ybm.ydjk.org.cn

C#:   u is User
来源：http://cwq.sjlbkw.cn

[G14] 数据类 / record
来源：http://yvi.hesvh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jmr.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://dwj.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://ioh.yj20258888.top

TS:   type User = { name: string; age: number };
来源：http://mgb.316326.xyz

Java: record User(String name, int age) {}
来源：http://pfw.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://qua.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xqu.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://gjw.quarkkingdee.top

[G15] 枚举
来源：http://vcx.cashguo.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fsm.xziqi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nca.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sdr.yongpay.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fst.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://mik.jiagoushi.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lcr.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://try.ydjk.org.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uep.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://vbo.mhx1999.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mar.sjlbkw.cn

PHP:  get_object_vars($obj);
来源：http://ejd.nanxuanxn.top

JS:   Object.entries(obj)
来源：http://uny.cashguo.top

TS:   Object.entries(obj)
来源：http://zpd.zycfv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uro.iojbl.cn


<!-- 参考信息 -->
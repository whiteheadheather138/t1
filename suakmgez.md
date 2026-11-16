代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://ebr.aibaodan.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pnd.zycfv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://swy.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ffw.cashguo.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vvs.ydjk.org.cn

[E19] 多行文本按行拆分
来源：http://ypg.chenjidiqi.icu

Py:   s.splitlines()
来源：http://gme.zdqjudy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://smm.sjlbkw.cn

JS:   s.split(/\r?\n/)
来源：http://ppq.hysaishi.cn

TS:   s.split(/\r?\n/)
来源：http://qyc.guowangkeji.top

Java: s.lines().toList()
来源：http://vtb.zhengqikj.top

Go:   strings.Split(s, "\n")
来源：http://psd.xylfe.cn

Ruby: s.lines
来源：http://bpn.shuidangran.top

C#:   s.Split('\n')
来源：http://rmc.xylfe.cn

[E20] 判断字符串是否为空
来源：http://xpe.pengpengdd.cyou

Py:   if not s:
来源：http://bmu.zdqjudy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bqw.hongshengwenyu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://axd.jinghuilouyu.cn

TS:   if (s === "") {}
来源：http://eir.jqgufenzy.top

Java: if (s.isEmpty()) {}
来源：http://vff.ivvv.top

Go:   if s == "" {}
来源：http://kxg.vqdsnc.cn

Ruby: if s.empty?
来源：http://srs.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vpl.wangshuangyany.cn

[E21] 超长截断加省略号
来源：http://ftd.wangshuangyany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dyx.xuanzx.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://spy.zdbjq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ydt.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jex.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://amf.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://gom.hesvh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ecf.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gif.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://eth.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ipv.jinghuilouyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kry.ctjpmb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yak.sysykeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hqk.jyoumei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nou.xingfuxueyuan.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xxi.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://xxs.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jdt.shuidangran.top

================================================================================
来源：http://puc.ywan-chungtsiang.top

F. 文件与目录
来源：http://jzk.zhoulong.xyz

================================================================================
来源：http://yez.snrcjt.cn

[F01] 读取整个文件
来源：http://yky.svipenyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://odv.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://bqg.jianghu66.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ijk.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mpd.cheryme.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ztc.52xcode.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xdi.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://ddm.zhaomingkeji.xyz

C#:   File.ReadAllText("a.txt");
来源：http://crs.sjlbkw.cn

[F02] 逐行读取文件
来源：http://tsj.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xut.jianghu66.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lag.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mjk.hammf.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ugh.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fgb.nanxuanxn.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blh.cqqwz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pah.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pcb.chenzaomai.com

[F03] 写入文件（覆盖）
来源：http://zwb.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ryc.hnxiangtu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zjp.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xwy.jiagoushi.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://njv.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://afm.mhx1999.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rjf.yongpay.top

Ruby: File.write("a.txt", "hi")
来源：http://kiz.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ihw.jyoumei.cn

[F04] 追加写入文件
来源：http://ddv.xinyue.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sgu.chenzaomai.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://evc.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zau.sufxvd.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://imu.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fag.aibaodan.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jdx.hongshengwenyu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cmf.sweek.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://axr.mhx1999.top

[F05] 判断文件或目录是否存在
来源：http://vfe.daria6918.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dlr.tian-w.cn

PHP:  file_exists("a.txt");
来源：http://tcn.mhx1999.top

JS:   fs.existsSync("a.txt")
来源：http://dst.tanke756.top

TS:   fs.existsSync("a.txt")
来源：http://drx.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://len.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vjw.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://uwg.havefunace.top

C#:   File.Exists("a.txt")
来源：http://yhi.jinqigufen.top

[F06] 删除文件
来源：http://rcw.yvedp.cn

Py:   os.remove("a.txt")
来源：http://kpw.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://nla.ydjk.org.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nws.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://nbk.gaohongyu789.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hcm.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://knd.dashuyun.cn

Ruby: File.delete("a.txt")
来源：http://aod.hfpthk.cn

C#:   File.Delete("a.txt");
来源：http://tjn.aibaodan.cn

[F07] 创建目录（含多级）
来源：http://tyc.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zyq.hywenlv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hdq.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oiv.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kwf.yanxiufei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cxc.daria6918.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gzz.fktsv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://elz.jinqigfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://smp.gotoacloud.top

[F08] 遍历目录
来源：http://uho.zdqjudy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rcn.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ubq.snrcjt.cn

JS:   fs.readdirSync("dir")
来源：http://fyc.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://cqj.yj202588.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lil.9152youxi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fne.smart0.xyz

Ruby: Dir.children("dir")
来源：http://wwh.xuetiantiany.cn

C#:   Directory.GetFiles("dir")
来源：http://wjy.bbcook.cn

[F09] 获取文件大小
来源：http://bmm.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://hbq.hcnkem.com

PHP:  filesize("a.txt");
来源：http://iom.hywenlv.cn

JS:   fs.statSync("a.txt").size
来源：http://bth.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://aqn.fktsv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://abw.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xux.ppjwa.cn

Ruby: File.size("a.txt")
来源：http://kpb.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://uec.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://ebz.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://len.nanxinkj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wvt.jinqigfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fqp.zycfv.cn

TS:   path.extname("a.txt")
来源：http://ewv.shzxlz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qnp.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rwy.ydjk.org.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://unt.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://loa.yanxiufei.cn

[F11] 复制与移动文件
来源：http://fcv.bjfxy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hbi.shuidangran.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qbl.andypj.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ozo.ctjpmb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://roi.zhiwuduotai.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nfu.vehdjk.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dzp.jinqigufen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://anz.nanxinkj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zlp.ppjwa.cn

[F12] CSV 读写
来源：http://lcg.fktsv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vso.tian-w.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lrs.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xlh.zdqjudy.top

TS:   // 同上
来源：http://ygi.nanxuanxn.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cbl.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nbh.aizwys.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wxk.yuanzhike.top

C#:   // 无内置：用 CsvHelper 库
来源：http://msh.zhoulong.xyz

================================================================================
来源：http://qtv.xingfuxueyuan.xyz

G. 面向对象
来源：http://pxp.c1oappe.top

================================================================================
来源：http://vqv.yueranfly.top

[G01] 定义类
来源：http://srs.ybcxt.top

Py:   class User: pass
来源：http://vos.zhengqikj.top

PHP:  class User {}
来源：http://hxp.chenzaomai.com

JS:   class User {}
来源：http://mct.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://tqi.shanyushiyangtech.top

Java: class User {}
来源：http://ccm.zdqjudy.top

Go:   type User struct { Name string }
来源：http://fiu.dianchejie.cn

Ruby: class User; end
来源：http://wpk.yonumen.top

C#:   class User {}
来源：http://wxp.guannengcc.top

[G02] 构造函数
来源：http://iut.ydzc1.top

Py:   def __init__(self, name): self.name = name
来源：http://jsl.sjlbkw.cn

PHP:  public function __construct(public string $name) {}
来源：http://tfw.redwolf501.top

JS:   constructor(name) { this.name = name; }
来源：http://mpq.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://nlh.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://twq.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gkj.xziqi.cn

Ruby: def initialize(name); @name = name; end
来源：http://bhy.hesvh.cn

C#:   public User(string name) { Name = name; }
来源：http://epf.tarul.cn

[G03] 实例属性
来源：http://qmw.andypj.xyz

Py:   self.name = "x"
来源：http://uyg.hywenlv.cn

PHP:  public string $name = "x";
来源：http://uwu.xuanzx.com

JS:   this.name = "x";
来源：http://mwn.jlsjyb.cn

TS:   name: string = "x";
来源：http://qhq.hesvh.cn

Java: private String name;
来源：http://rvs.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://npr.vqdsnc.cn

Ruby: @name = "x"
来源：http://adh.jinqigufen.top

C#:   public string Name { get; set; } = "x";
来源：http://gca.redwolf501.top

[G04] 定义方法
来源：http://oqf.xinyue.icu

Py:   def greet(self): return self.name
来源：http://sao.tianlin.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://dys.fktsv.cn

JS:   greet() { return this.name; }
来源：http://mjq.dashuyun.cn

TS:   greet(): string { return this.name; }
来源：http://mny.zhengqikj.top

Java: String greet() { return name; }
来源：http://iga.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://veb.cheryme.top

Ruby: def greet; @name; end
来源：http://cvn.gzhubu.top

C#:   public string Greet() => Name;
来源：http://gxm.cucudq.cn

[G05] 继承
来源：http://fqo.yvedp.cn

Py:   class Admin(User): pass
来源：http://fhv.tarul.cn

PHP:  class Admin extends User {}
来源：http://sta.cucudq.cn

JS:   class Admin extends User {}
来源：http://ofz.ehwqpu.com

TS:   class Admin extends User {}
来源：http://zbg.yonumen.top

Java: class Admin extends User {}
来源：http://ysz.chenzaomai.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ymf.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://xos.epnwcf.com

C#:   class Admin : User {}
来源：http://yib.xuanzx.com

[G06] 重写方法
来源：http://rty.gzhubu.top

Py:   def greet(self): return "admin"
来源：http://dmx.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pyc.ppjwa.cn

JS:   greet() { return "admin"; }
来源：http://xjt.kuanghao11.cn

TS:   greet(): string { return "admin"; }
来源：http://xyj.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://nuv.chenlongwang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tfy.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://lzw.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://xjh.hammf.cn

[G07] 调用父类方法
来源：http://dyb.xuanzx.com

Py:   super().greet()
来源：http://ldk.zhengqikj.top

PHP:  parent::greet();
来源：http://ovq.shanyushiyangkeji.top

JS:   super.greet();
来源：http://uny.jinghuilouyu.cn

TS:   super.greet();
来源：http://kei.gzhubu.top

Java: super.greet();
来源：http://voe.fengsongda.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ztm.tian-w.cn

Ruby: super
来源：http://gyn.hywenlv.cn

C#:   base.Greet();
来源：http://ank.bbcook.cn

[G08] 静态方法与属性
来源：http://vvz.zhaomingkeji.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kow.ehwqpu.com

PHP:  public static function f() {}
来源：http://cmf.ydzc1.top

JS:   static f() {}
来源：http://pio.aizwys.cn

TS:   static f(): void {}
来源：http://hoh.vehdjk.com

Java: static void f() {}
来源：http://hdg.epnwcf.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ddo.quarkkingdee.top

Ruby: def self.f; end
来源：http://mhj.bjfxy.top

C#:   public static void F() {}
来源：http://xyk.yfazqb.com

[G09] 接口 / 抽象类
来源：http://dxv.aibaodan.cn

Py:   from abc import ABC, abstractmethod
来源：http://vtn.mhx1999.top

PHP:  interface Shape { public function area(): float; }
来源：http://hhr.zdbjq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kdw.snrcjt.cn

TS:   interface Shape { area(): number; }
来源：http://zqj.meibo888.top

Java: interface Shape { double area(); }
来源：http://gmm.cdnleiting.top

Go:   type Shape interface { Area() float64 }
来源：http://nfp.daxiang520.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cub.fehbvm.com

C#:   interface IShape { double Area(); }
来源：http://wok.yuanzhike.top

[G10] 访问控制
来源：http://mfj.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://ahx.cucudq.cn

PHP:  public / protected / private
来源：http://rxw.sjlbkw.cn

JS:   #private 字段；其余公开
来源：http://pfj.jinyuanbaomall.cn

TS:   public / protected / private
来源：http://ipx.bbcook.cn

Java: public / protected / private / 默认包级
来源：http://dzg.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ehl.yj202588.top

Ruby: public / protected / private
来源：http://gxm.sufxvd.cn

C#:   public / protected / private / internal
来源：http://xmu.tanke756.top

[G11] getter / setter
来源：http://xix.haohaochexian.top

Py:   @property 与 @x.setter
来源：http://das.shanyushiyangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gpl.fzhhl.top

JS:   get name() { return this._name; }
来源：http://sqo.dashuyun.cn

TS:   get name(): string { return this._name; }
来源：http://sqz.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://jhe.ybcxt.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ouf.yueranfly.top

Ruby: attr_accessor :name
来源：http://qot.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://laq.jianghu66.top

[G12] 对象转字符串
来源：http://bkh.fengsongda.top

Py:   def __str__(self): return self.name
来源：http://cvr.daria6918.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dwc.jlsjyb.cn

JS:   toString() { return this.name; }
来源：http://ckn.chenjidiqi.icu

TS:   toString(): string { return this.name; }
来源：http://yil.zdqjudy.top

Java: @Override public String toString() { return name; }
来源：http://gjw.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rtb.ywan-chungtsiang.top

Ruby: def to_s; @name; end
来源：http://bze.zhiwuduotai.top

C#:   public override string ToString() => Name;
来源：http://mhr.cdnleiting.top

[G13] 判断对象类型
来源：http://ogy.yonumen.top

Py:   isinstance(u, User)
来源：http://srt.yj202588.top

PHP:  $u instanceof User
来源：http://ibp.yongpay.top

JS:   u instanceof User
来源：http://hqn.xinyue.icu

TS:   u instanceof User
来源：http://snp.fengsongda.top

Java: u instanceof User
来源：http://vya.hcnkem.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://peo.xylfe.cn

Ruby: u.is_a?(User)
来源：http://gii.shangyingyoupin.top

C#:   u is User
来源：http://tdx.yangfankeji.com

[G14] 数据类 / record
来源：http://zhq.jinyuanbaomall.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gft.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://jwf.fengsongda.top

JS:   // 无内置：普通类或对象字面量
来源：http://cmj.snrcjt.cn

TS:   type User = { name: string; age: number };
来源：http://dxq.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://ubp.sjlbkw.cn

Go:   type User struct { Name string; Age int }
来源：http://lfn.jinghuilouyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ncm.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://egz.jinqigufen.top

[G15] 枚举
来源：http://elk.cheryme.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cua.daria6918.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://utw.hesvh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://maq.sufxvd.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://npg.shanyushiyangkeji.top

Java: enum Color { RED, GREEN }
来源：http://isj.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pig.jiagoushi.top

Ruby: Color = %i[red green].freeze
来源：http://urb.gotoacloud.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gzk.cdnleiting.top

[G16] 对象转数组 / 字典
来源：http://hqy.xylfe.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kfx.aibaodan.cn

PHP:  get_object_vars($obj);
来源：http://tmu.316326.xyz

JS:   Object.entries(obj)
来源：http://lyo.aibaodan.cn

TS:   Object.entries(obj)
来源：http://giu.yuanzhike.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://asw.tarul.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kdv.xylfe.cn

Ruby: obj.instance_variables
来源：http://vbq.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://mze.jinqigfzy.top

================================================================================
来源：http://tfn.hnqzz.top


<!-- 参考信息 -->
代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://yry.chenzaomai.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qzr.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ivi.0kj1m.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xwy.zhoulong.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jqo.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://xuj.fzhhl.top

Py:   s.splitlines()
来源：http://swu.zhaomingkeji.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hsg.fengsongda.top

JS:   s.split(/\r?\n/)
来源：http://qib.yj202588.top

TS:   s.split(/\r?\n/)
来源：http://wks.wangshuangyany.cn

Java: s.lines().toList()
来源：http://ods.daxiang520.top

Go:   strings.Split(s, "\n")
来源：http://svd.yj202588.top

Ruby: s.lines
来源：http://wmb.sysykeji.top

C#:   s.Split('\n')
来源：http://jgm.pycfn.com

[E20] 判断字符串是否为空
来源：http://snk.quarkkingdee.top

Py:   if not s:
来源：http://nty.guowangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://trf.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gkc.svipenyu.cn

TS:   if (s === "") {}
来源：http://tgk.guowangkeji.top

Java: if (s.isEmpty()) {}
来源：http://wfn.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://jyw.tian-w.cn

Ruby: if s.empty?
来源：http://ixj.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jsf.xinyue.icu

[E21] 超长截断加省略号
来源：http://ejf.tanke756.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rqy.wangshuangyany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eza.yfazqb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lwl.52xcode.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ukm.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bmi.vqdsnc.cn

Go:   // 按 rune 判断长度后截断
来源：http://idg.shanyushiyangtech.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ewe.hywenlv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yxj.ybcxt.top

[E22] 字节长度与字符长度
来源：http://rad.kuanghao11.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://whp.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aar.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mpg.nanxinkj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xwd.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ljf.ydzc1.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zlj.mhx1999.top

Ruby: s.bytesize;  s.length
来源：http://qku.kuanghao11.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eve.wangshuangyany.cn

================================================================================
来源：http://bwn.yvedp.cn

F. 文件与目录
来源：http://gja.sysykeji.top

================================================================================
来源：http://jfl.jiagoushi.top

[F01] 读取整个文件
来源：http://fgk.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jay.xingfuxueyuan.xyz

PHP:  file_get_contents("a.txt");
来源：http://tgk.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://siw.gzhubu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rdf.hysaishi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://opz.bjfxy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ykj.gogol.net.cn

Ruby: File.read("a.txt")
来源：http://rzo.zhongyouzk.top

C#:   File.ReadAllText("a.txt");
来源：http://nve.chenlongwang.top

[F02] 逐行读取文件
来源：http://nbc.0kj1m.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uug.jianghu66.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://orx.ctjpmb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pth.52xcode.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ano.c1oappe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aav.nanxuanxn.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nqg.9152youxi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://orn.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fbk.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://zoq.yangfankeji.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mou.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://lnl.zhoulong.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wig.sufxvd.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mal.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hkv.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bmc.zhengqikj.top

Ruby: File.write("a.txt", "hi")
来源：http://lit.zhaomingkeji.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tyz.redwolf501.top

[F04] 追加写入文件
来源：http://gju.yj20258888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vxz.jinqigfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gwl.cashguo.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dbq.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cyi.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bqq.xingfuxueyuan.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ezn.zhengqikj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://env.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rwk.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://oxe.hfpthk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ywx.vqdsnc.cn

PHP:  file_exists("a.txt");
来源：http://tsd.guannengcc.top

JS:   fs.existsSync("a.txt")
来源：http://zrt.zhongyouzk.top

TS:   fs.existsSync("a.txt")
来源：http://yzw.jyoumei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://som.yj20258.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://odf.yuanzhike.top

Ruby: File.exist?("a.txt")
来源：http://mrd.pengpengdd.cyou

C#:   File.Exists("a.txt")
来源：http://rfz.guannengcc.top

[F06] 删除文件
来源：http://xvc.xinyue.icu

Py:   os.remove("a.txt")
来源：http://wmq.hammf.cn

PHP:  unlink("a.txt");
来源：http://rrf.xuetiantiany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://opg.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://mdp.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ymh.yonumen.top

Go:   os.Remove("a.txt")
来源：http://twl.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://jbx.zhoulong.xyz

C#:   File.Delete("a.txt");
来源：http://xea.zdbjq.cn

[F07] 创建目录（含多级）
来源：http://eix.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qvk.yj202588.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kiw.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mkz.ydzc1.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dkp.ydjk.org.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jpb.zhiwuduotai.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fvi.hongshengwenyu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://puz.ivvv.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://adv.xinyue.icu

[F08] 遍历目录
来源：http://znz.zhijiandao.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jst.jlsjyb.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vrx.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://pmk.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://ubl.gaohongyu789.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nmm.vehdjk.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://yce.redwolf501.top

Ruby: Dir.children("dir")
来源：http://eac.jinyuanbaomall.cn

C#:   Directory.GetFiles("dir")
来源：http://qlc.zycfv.cn

[F09] 获取文件大小
来源：http://tja.aibaodan.cn

Py:   os.path.getsize("a.txt")
来源：http://eya.zhiwuduotai.top

PHP:  filesize("a.txt");
来源：http://kkr.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://wxh.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://etz.epnwcf.com

Java: Files.size(Path.of("a.txt"))
来源：http://zjz.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://avq.gotoacloud.top

Ruby: File.size("a.txt")
来源：http://pos.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://ycn.feifeiyinyue.top

[F10] 取文件扩展名 / 文件名
来源：http://esp.xylfe.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ceo.hfpthk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uvn.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kwc.cucudq.cn

TS:   path.extname("a.txt")
来源：http://nph.uphjek.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uqi.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qdd.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://voe.tianlin.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uxv.yonumen.top

[F11] 复制与移动文件
来源：http://xox.hnqzz.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bof.snrcjt.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iha.sjlbkw.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gmw.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qxa.dianchejie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hij.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jpn.uphjek.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ffp.nanxuanxn.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tww.dianchejie.cn

[F12] CSV 读写
来源：http://pmr.yueranfly.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xky.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bdv.tarul.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gzs.zhoulong.xyz

TS:   // 同上
来源：http://lqu.jyoumei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://izr.daria6918.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tyw.cdnleiting.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vfb.tarul.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wuw.shzxlz.cn

================================================================================
来源：http://kqy.jinqigfzy.top

G. 面向对象
来源：http://slz.vqdsnc.cn

================================================================================
来源：http://rjm.zhijiandao.cn

[G01] 定义类
来源：http://ate.feifeiyinyue.top

Py:   class User: pass
来源：http://ntk.svipenyu.cn

PHP:  class User {}
来源：http://aio.yangfankeji.com

JS:   class User {}
来源：http://yno.smart0.xyz

TS:   class User { name: string = ""; }
来源：http://tew.zhijiandao.cn

Java: class User {}
来源：http://kmt.zdbjq.cn

Go:   type User struct { Name string }
来源：http://pru.0kj1m.cn

Ruby: class User; end
来源：http://hli.feifeiyinyue.top

C#:   class User {}
来源：http://uwv.c1oappe.top

[G02] 构造函数
来源：http://ayi.zhixingplan.top

Py:   def __init__(self, name): self.name = name
来源：http://itx.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://bkn.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://ezs.sxryk.cn

TS:   constructor(public name: string) {}
来源：http://ofs.sufxvd.cn

Java: User(String name) { this.name = name; }
来源：http://jdh.ydjk.org.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rih.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://dlr.mhx1999.top

C#:   public User(string name) { Name = name; }
来源：http://vcq.sxryk.cn

[G03] 实例属性
来源：http://tsa.mhx1999.top

Py:   self.name = "x"
来源：http://dlo.shanyushiyangkeji.top

PHP:  public string $name = "x";
来源：http://igv.yanxiufei.cn

JS:   this.name = "x";
来源：http://qos.pengpengdd.cyou

TS:   name: string = "x";
来源：http://pvu.shzxlz.cn

Java: private String name;
来源：http://xao.uphjek.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mwr.ywan-chungtsiang.top

Ruby: @name = "x"
来源：http://ghf.shzxlz.cn

C#:   public string Name { get; set; } = "x";
来源：http://nck.yuanzhike.top

[G04] 定义方法
来源：http://hqg.zhoulong.xyz

Py:   def greet(self): return self.name
来源：http://srt.aibaodan.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://icg.nwbrower.top

JS:   greet() { return this.name; }
来源：http://mks.nanxuanxn.top

TS:   greet(): string { return this.name; }
来源：http://tir.yvedp.cn

Java: String greet() { return name; }
来源：http://kza.haohaochexian.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://awb.tanke756.top

Ruby: def greet; @name; end
来源：http://niy.c1oappe.top

C#:   public string Greet() => Name;
来源：http://ard.xylfe.cn

[G05] 继承
来源：http://dhd.fktsv.cn

Py:   class Admin(User): pass
来源：http://bll.jinqigfzy.top

PHP:  class Admin extends User {}
来源：http://xgu.hesvh.cn

JS:   class Admin extends User {}
来源：http://zek.smart0.xyz

TS:   class Admin extends User {}
来源：http://kgi.zhengqikj.top

Java: class Admin extends User {}
来源：http://udn.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lzr.gzhubu.top

Ruby: class Admin < User; end
来源：http://bud.cheryme.top

C#:   class Admin : User {}
来源：http://mfw.9152youxi.cn

[G06] 重写方法
来源：http://jnb.9152youxi.cn

Py:   def greet(self): return "admin"
来源：http://yhr.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yus.yangfankeji.com

JS:   greet() { return "admin"; }
来源：http://bgj.cqqwz.cn

TS:   greet(): string { return "admin"; }
来源：http://mdo.cheryme.top

Java: @Override String greet() { return "admin"; }
来源：http://gsf.sufxvd.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oac.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://zys.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://vnu.guannengcc.top

[G07] 调用父类方法
来源：http://bdq.quarkkingdee.top

Py:   super().greet()
来源：http://sxr.chenjidiqi.icu

PHP:  parent::greet();
来源：http://noc.birdmap.top

JS:   super.greet();
来源：http://ioq.ybcxt.top

TS:   super.greet();
来源：http://gow.fanxiaobao.xyz

Java: super.greet();
来源：http://lgi.cashguo.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://edl.0kj1m.cn

Ruby: super
来源：http://xrp.yanxiufei.cn

C#:   base.Greet();
来源：http://mdr.sufxvd.cn

[G08] 静态方法与属性
来源：http://mbk.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kyr.sufxvd.cn

PHP:  public static function f() {}
来源：http://bsa.cheryme.top

JS:   static f() {}
来源：http://ysi.svipenyu.cn

TS:   static f(): void {}
来源：http://grm.cheryme.top

Java: static void f() {}
来源：http://lol.daxiang520.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xwh.zhoulong.xyz

Ruby: def self.f; end
来源：http://axx.dianchejie.cn

C#:   public static void F() {}
来源：http://cej.redwolf501.top

[G09] 接口 / 抽象类
来源：http://iih.xylfe.cn

Py:   from abc import ABC, abstractmethod
来源：http://xiq.zdbjq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pve.gzhubu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wco.hnxiangtu.top

TS:   interface Shape { area(): number; }
来源：http://tnp.yj202588.top

Java: interface Shape { double area(); }
来源：http://hal.chenlongwang.top

Go:   type Shape interface { Area() float64 }
来源：http://dmd.meibo888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gsm.bbcook.cn

C#:   interface IShape { double Area(); }
来源：http://dvm.hammf.cn

[G10] 访问控制
来源：http://ghj.xingfuxueyuan.xyz

Py:   约定 _protected / __private（不强制）
来源：http://xzq.tarul.cn

PHP:  public / protected / private
来源：http://dzi.hnqzz.top

JS:   #private 字段；其余公开
来源：http://ypo.tianlin.xyz

TS:   public / protected / private
来源：http://lga.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://prc.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://yni.chenzaomai.com

Ruby: public / protected / private
来源：http://lfi.hysaishi.cn

C#:   public / protected / private / internal
来源：http://hwv.sjlbkw.cn

[G11] getter / setter
来源：http://dir.chenjidiqi.icu

Py:   @property 与 @x.setter
来源：http://qjj.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://anc.hcnkem.com

JS:   get name() { return this._name; }
来源：http://hmj.hnxiangtu.top

TS:   get name(): string { return this._name; }
来源：http://rgp.sufxvd.cn

Java: public String getName() { return name; }
来源：http://lpa.ivvv.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hzp.havefunace.top

Ruby: attr_accessor :name
来源：http://oxu.nanxuanxn.top

C#:   public string Name { get; set; }
来源：http://bzx.zhoulong.xyz

[G12] 对象转字符串
来源：http://izs.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://psg.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gtj.daxiang520.top

JS:   toString() { return this.name; }
来源：http://epn.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://xat.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://dtl.yj20258888.top

Go:   func (u User) String() string { return u.Name }
来源：http://art.daxiang520.top

Ruby: def to_s; @name; end
来源：http://xnu.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://kau.tanke756.top

[G13] 判断对象类型
来源：http://okv.ydzc1.top

Py:   isinstance(u, User)
来源：http://ifn.kuanghao11.cn

PHP:  $u instanceof User
来源：http://wxr.cqqwz.cn

JS:   u instanceof User
来源：http://qvb.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://lue.uphjek.com

Java: u instanceof User
来源：http://hte.shanyushiyangtech.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://old.mhx1999.top

Ruby: u.is_a?(User)
来源：http://ffj.yj20258.top

C#:   u is User
来源：http://zjr.havefunace.top

[G14] 数据类 / record
来源：http://qjw.wangdashe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mcb.zhengqikj.top

PHP:  // 用 readonly 属性模拟
来源：http://ynz.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://txf.yj202588.top

TS:   type User = { name: string; age: number };
来源：http://dhh.gotoacloud.top

Java: record User(String name, int age) {}
来源：http://qdq.shzxlz.cn

Go:   type User struct { Name string; Age int }
来源：http://lua.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tbi.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://jzp.cashguo.top

[G15] 枚举
来源：http://kuo.hywenlv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ztm.xuetiantiany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rvv.sysykeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qdn.kuanghao11.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wif.daria6918.cn

Java: enum Color { RED, GREEN }
来源：http://wbd.dianchejie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yve.jianghu66.top

Ruby: Color = %i[red green].freeze
来源：http://emi.yueranfly.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uwt.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://jaz.bjfxy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rhy.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://pin.kuanghao11.cn

JS:   Object.entries(obj)
来源：http://hag.aibaodan.cn

TS:   Object.entries(obj)
来源：http://qwo.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kmg.vehdjk.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://anv.yj20258888.top

Ruby: obj.instance_variables
来源：http://luv.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://cys.havefunace.top

================================================================================
来源：http://qcv.nwbrower.top


<!-- 参考信息 -->
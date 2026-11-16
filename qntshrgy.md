代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vgc.kuanghao11.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sbz.cucudq.cn

Ruby: s.capitalize
来源：http://swm.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mpx.gzhubu.top

[E18] 模板占位符替换
来源：http://vtu.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xoo.zhongyouzk.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yvk.gaohongyu789.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dqc.uphjek.com

TS:   tpl.replaceAll("{name}", name)
来源：http://jku.nanxinkj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kqu.chenjidiqi.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gsd.yuanzhike.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ccq.hysaishi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lnt.0kj1m.cn

[E19] 多行文本按行拆分
来源：http://dbh.cqqwz.cn

Py:   s.splitlines()
来源：http://ubj.jinqigfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tbh.kuanghao11.cn

JS:   s.split(/\r?\n/)
来源：http://wfm.ppjwa.cn

TS:   s.split(/\r?\n/)
来源：http://isz.aizwys.cn

Java: s.lines().toList()
来源：http://dnd.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://fmm.zhijiandao.cn

Ruby: s.lines
来源：http://omh.hysaishi.cn

C#:   s.Split('\n')
来源：http://lfg.hnxiangtu.top

[E20] 判断字符串是否为空
来源：http://oak.chenlongwang.top

Py:   if not s:
来源：http://dgv.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fiz.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mjk.havefunace.top

TS:   if (s === "") {}
来源：http://fij.cheryme.top

Java: if (s.isEmpty()) {}
来源：http://lwg.gotoacloud.top

Go:   if s == "" {}
来源：http://qdg.nwbrower.top

Ruby: if s.empty?
来源：http://hyj.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xjl.andypj.xyz

[E21] 超长截断加省略号
来源：http://hxy.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mil.yfazqb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yjr.yongpay.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kzg.zdqjudy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wre.xuetiantiany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vtd.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://mrf.dashuyun.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nws.hnxiangtu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://shq.cucudq.cn

[E22] 字节长度与字符长度
来源：http://cpe.dashuyun.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://due.cashguo.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bcl.vqdsnc.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://toq.yj202588.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dij.hywenlv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qtx.52xcode.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nqn.sysykeji.top

Ruby: s.bytesize;  s.length
来源：http://zms.jinqigfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://izl.hammf.cn

================================================================================
来源：http://lbc.andypj.xyz

F. 文件与目录
来源：http://nic.zdbjq.cn

================================================================================
来源：http://xcu.ehwqpu.com

[F01] 读取整个文件
来源：http://rik.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hxq.andypj.xyz

PHP:  file_get_contents("a.txt");
来源：http://etr.pycfn.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ijm.birdmap.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://izp.zhoulong.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://nvz.daria6918.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jjx.shuidangran.top

Ruby: File.read("a.txt")
来源：http://lus.vehdjk.com

C#:   File.ReadAllText("a.txt");
来源：http://qxz.chenlongwang.top

[F02] 逐行读取文件
来源：http://goj.cqqwz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oft.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bkh.jiagoushi.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rgl.52xcode.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ylr.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ljs.xingfuxueyuan.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://brr.hongshengwenyu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jry.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://drg.cheryme.top

[F03] 写入文件（覆盖）
来源：http://aee.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wgh.shuidangran.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://heb.ybcxt.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bsv.nanxuanxn.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qfx.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tvr.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://swb.shuidangran.top

Ruby: File.write("a.txt", "hi")
来源：http://vgu.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rnx.svipenyu.cn

[F04] 追加写入文件
来源：http://whj.hesvh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cgl.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dyi.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lcy.wangshuangyany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://efk.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://stq.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fme.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wvv.gzhubu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qvi.xuanzx.com

[F05] 判断文件或目录是否存在
来源：http://ezx.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ixq.cdnleiting.top

PHP:  file_exists("a.txt");
来源：http://xnb.ybcxt.top

JS:   fs.existsSync("a.txt")
来源：http://rzy.c1oappe.top

TS:   fs.existsSync("a.txt")
来源：http://ktc.zhixingplan.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bel.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mfs.pycfn.com

Ruby: File.exist?("a.txt")
来源：http://cua.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://rgl.316326.xyz

[F06] 删除文件
来源：http://sdv.sufxvd.cn

Py:   os.remove("a.txt")
来源：http://qcf.yueranfly.top

PHP:  unlink("a.txt");
来源：http://ssx.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://prb.nwbrower.top

TS:   fs.unlinkSync("a.txt")
来源：http://wzy.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aui.zhiwuduotai.top

Go:   os.Remove("a.txt")
来源：http://wwt.yonumen.top

Ruby: File.delete("a.txt")
来源：http://aji.bjfxy.top

C#:   File.Delete("a.txt");
来源：http://swq.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://efj.tanke756.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vzj.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rvk.jinqigfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bke.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wgv.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oti.kuanghao11.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ehk.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vrq.fanxiaobao.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://avv.ppjwa.cn

[F08] 遍历目录
来源：http://udy.ehwqpu.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://bva.dashuyun.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nco.yfazqb.com

JS:   fs.readdirSync("dir")
来源：http://vip.vqdsnc.cn

TS:   fs.readdirSync("dir")
来源：http://csc.ydzc1.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yfh.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vih.hnxiangtu.top

Ruby: Dir.children("dir")
来源：http://bkq.xuetiantiany.cn

C#:   Directory.GetFiles("dir")
来源：http://bit.andypj.xyz

[F09] 获取文件大小
来源：http://neh.mhx1999.top

Py:   os.path.getsize("a.txt")
来源：http://zrz.yj20258888.top

PHP:  filesize("a.txt");
来源：http://zpn.sxryk.cn

JS:   fs.statSync("a.txt").size
来源：http://ryj.zdqjudy.top

TS:   fs.statSync("a.txt").size
来源：http://ybg.hcnkem.com

Java: Files.size(Path.of("a.txt"))
来源：http://eug.meibo888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wjo.bbcook.cn

Ruby: File.size("a.txt")
来源：http://zbq.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://plx.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://xpx.chenlongwang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pph.chenjidiqi.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://llg.ydzc1.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dhs.52xcode.cn

TS:   path.extname("a.txt")
来源：http://ylm.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iqj.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vzk.gotoacloud.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ndn.epnwcf.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hfm.yueranfly.top

[F11] 复制与移动文件
来源：http://xwt.ehwqpu.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cey.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lhz.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rjb.xingfuxueyuan.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wdy.zhongyouzk.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dag.hammf.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kyi.yj20258.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fro.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cyx.shanyushiyangkeji.top

[F12] CSV 读写
来源：http://mnp.dashuyun.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://srl.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://syh.gaohongyu789.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qgm.zhiwuduotai.top

TS:   // 同上
来源：http://iuz.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zim.hesvh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sdz.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xie.yangfankeji.com

C#:   // 无内置：用 CsvHelper 库
来源：http://xph.birdmap.top

================================================================================
来源：http://msg.jqgufenzy.top

G. 面向对象
来源：http://inw.yangfankeji.com

================================================================================
来源：http://fjv.ywan-chungtsiang.top

[G01] 定义类
来源：http://agh.gogol.net.cn

Py:   class User: pass
来源：http://tlk.uphjek.com

PHP:  class User {}
来源：http://gju.ivvv.top

JS:   class User {}
来源：http://qtt.gotoacloud.top

TS:   class User { name: string = ""; }
来源：http://yjk.yuxming.cn

Java: class User {}
来源：http://dmf.feifeiyinyue.top

Go:   type User struct { Name string }
来源：http://nrg.chenzaomai.com

Ruby: class User; end
来源：http://sfx.smart0.xyz

C#:   class User {}
来源：http://epo.gogol.net.cn

[G02] 构造函数
来源：http://wyg.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://dig.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://dsp.zhixingplan.top

JS:   constructor(name) { this.name = name; }
来源：http://efd.nwbrower.top

TS:   constructor(public name: string) {}
来源：http://wrn.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://tuv.ydjk.org.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dic.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://xpg.sysykeji.top

C#:   public User(string name) { Name = name; }
来源：http://pyp.ydzc1.top

[G03] 实例属性
来源：http://tom.jyoumei.cn

Py:   self.name = "x"
来源：http://smm.yuxming.cn

PHP:  public string $name = "x";
来源：http://wrp.gotoacloud.top

JS:   this.name = "x";
来源：http://iim.cucudq.cn

TS:   name: string = "x";
来源：http://awx.ivvv.top

Java: private String name;
来源：http://zaj.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qad.yfazqb.com

Ruby: @name = "x"
来源：http://cjy.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://axh.yfazqb.com

[G04] 定义方法
来源：http://nuw.fktsv.cn

Py:   def greet(self): return self.name
来源：http://git.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nrp.gogol.net.cn

JS:   greet() { return this.name; }
来源：http://cna.ydzc1.top

TS:   greet(): string { return this.name; }
来源：http://mdu.cdnleiting.top

Java: String greet() { return name; }
来源：http://qep.chenzaomai.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://djl.cqqwz.cn

Ruby: def greet; @name; end
来源：http://mrs.tarul.cn

C#:   public string Greet() => Name;
来源：http://bwh.c1oappe.top

[G05] 继承
来源：http://mrd.ppjwa.cn

Py:   class Admin(User): pass
来源：http://enc.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://ayh.svipenyu.cn

JS:   class Admin extends User {}
来源：http://akt.ehwqpu.com

TS:   class Admin extends User {}
来源：http://fqn.jinghuilouyu.cn

Java: class Admin extends User {}
来源：http://ghf.snrcjt.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://efr.cucudq.cn

Ruby: class Admin < User; end
来源：http://axi.xziqi.cn

C#:   class Admin : User {}
来源：http://jlo.9152youxi.cn

[G06] 重写方法
来源：http://aag.xziqi.cn

Py:   def greet(self): return "admin"
来源：http://xpo.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rhm.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://pwn.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://jxy.hammf.cn

Java: @Override String greet() { return "admin"; }
来源：http://ldq.zhoulong.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tkq.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://klv.hesvh.cn

C#:   public override string Greet() => "admin";
来源：http://rej.316326.xyz

[G07] 调用父类方法
来源：http://jtp.ywan-chungtsiang.top

Py:   super().greet()
来源：http://pks.aizwys.cn

PHP:  parent::greet();
来源：http://dfk.zhengqikj.top

JS:   super.greet();
来源：http://tyt.redwolf501.top

TS:   super.greet();
来源：http://rci.chenzaomai.com

Java: super.greet();
来源：http://qln.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wtk.iojbl.cn

Ruby: super
来源：http://lpv.yongpay.top

C#:   base.Greet();
来源：http://xgq.redwolf501.top

[G08] 静态方法与属性
来源：http://cps.vqdsnc.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gdc.hnqzz.top

PHP:  public static function f() {}
来源：http://ocg.ivvv.top

JS:   static f() {}
来源：http://miy.ppjwa.cn

TS:   static f(): void {}
来源：http://uzl.yuxming.cn

Java: static void f() {}
来源：http://sec.52xcode.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yvf.xuanzx.com

Ruby: def self.f; end
来源：http://vsj.hammf.cn

C#:   public static void F() {}
来源：http://iba.quarkkingdee.top

[G09] 接口 / 抽象类
来源：http://ofg.yanxiufei.cn

Py:   from abc import ABC, abstractmethod
来源：http://ufp.cheryme.top

PHP:  interface Shape { public function area(): float; }
来源：http://hor.jlsjyb.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lov.jlsjyb.cn

TS:   interface Shape { area(): number; }
来源：http://djp.hnqzz.top

Java: interface Shape { double area(); }
来源：http://lux.tanke756.top

Go:   type Shape interface { Area() float64 }
来源：http://bfr.hfpthk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jch.hcnkem.com

C#:   interface IShape { double Area(); }
来源：http://vns.9152youxi.cn

[G10] 访问控制
来源：http://xiz.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://bwh.gaohongyu789.top

PHP:  public / protected / private
来源：http://oba.yongpay.top

JS:   #private 字段；其余公开
来源：http://vgd.guowangkeji.top

TS:   public / protected / private
来源：http://vib.fanxiaobao.xyz

Java: public / protected / private / 默认包级
来源：http://kab.guannengcc.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://stc.bjfxy.top

Ruby: public / protected / private
来源：http://dcf.feifeiyinyue.top

C#:   public / protected / private / internal
来源：http://uyu.tianlin.xyz

[G11] getter / setter
来源：http://rso.guowangkeji.top

Py:   @property 与 @x.setter
来源：http://fhb.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lwt.ppjwa.cn

JS:   get name() { return this._name; }
来源：http://bam.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://jts.hnqzz.top

Java: public String getName() { return name; }
来源：http://atu.xuanzx.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://fvj.xylfe.cn

Ruby: attr_accessor :name
来源：http://ngh.ybcxt.top

C#:   public string Name { get; set; }
来源：http://tof.9152youxi.cn

[G12] 对象转字符串
来源：http://zti.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://rdi.zhoulong.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://zkq.fengsongda.top

JS:   toString() { return this.name; }
来源：http://wqy.nanxinkj.top

TS:   toString(): string { return this.name; }
来源：http://hlu.jiagoushi.top

Java: @Override public String toString() { return name; }
来源：http://qik.yanxiufei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ixc.nwbrower.top

Ruby: def to_s; @name; end
来源：http://wpw.yangfankeji.com

C#:   public override string ToString() => Name;
来源：http://iqp.ctjpmb.com

[G13] 判断对象类型
来源：http://tkp.ctjpmb.com

Py:   isinstance(u, User)
来源：http://lbh.xingfuxueyuan.xyz

PHP:  $u instanceof User
来源：http://ige.ehwqpu.com

JS:   u instanceof User
来源：http://xri.hesvh.cn

TS:   u instanceof User
来源：http://uqp.yuxming.cn

Java: u instanceof User
来源：http://ihs.xinyue.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://hwe.feifeiyinyue.top

Ruby: u.is_a?(User)
来源：http://lpn.andypj.xyz

C#:   u is User
来源：http://pmz.ivvv.top

[G14] 数据类 / record
来源：http://wrg.zdbjq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fsv.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://fzj.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://itl.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://jig.ctjpmb.com

Java: record User(String name, int age) {}
来源：http://qty.yfazqb.com

Go:   type User struct { Name string; Age int }
来源：http://xbm.c1oappe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hfh.andypj.xyz

C#:   record User(string Name, int Age);
来源：http://kup.zhoulong.xyz

[G15] 枚举
来源：http://jnj.cashguo.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://obm.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vvu.zycfv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://axu.aibaodan.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://idj.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://ffv.pengpengdd.cyou

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hod.svipenyu.cn

Ruby: Color = %i[red green].freeze
来源：http://dcq.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dye.aizwys.cn

[G16] 对象转数组 / 字典
来源：http://glz.fktsv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://quc.hongshengwenyu.top


<!-- 参考信息 -->
代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vue.jqgfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kbz.chenlongwang.top

C#:   1234567.ToString("N0")
来源：http://upv.yj20258888.top

[E17] 首字母大写
来源：http://yws.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nnz.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://iti.cdnleiting.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lwk.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oha.fehbvm.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qsl.hammf.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tka.zdqjudy.top

Ruby: s.capitalize
来源：http://tfu.hesvh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jrr.birdmap.top

[E18] 模板占位符替换
来源：http://azg.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xfi.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://khx.redwolf501.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wel.jiagoushi.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lpv.ivvv.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vqy.wangshuangyany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://clf.ywan-chungtsiang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ljv.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qes.gzhubu.top

[E19] 多行文本按行拆分
来源：http://tlb.jqgfzy.top

Py:   s.splitlines()
来源：http://hba.hfpthk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kxx.cucudq.cn

JS:   s.split(/\r?\n/)
来源：http://vga.zhongyouzk.top

TS:   s.split(/\r?\n/)
来源：http://hsz.zycfv.cn

Java: s.lines().toList()
来源：http://ftq.xziqi.cn

Go:   strings.Split(s, "\n")
来源：http://ldp.jianghu66.top

Ruby: s.lines
来源：http://xai.yj20258888.top

C#:   s.Split('\n')
来源：http://yre.jqgfzy.top

[E20] 判断字符串是否为空
来源：http://nkb.jlsjyb.cn

Py:   if not s:
来源：http://wtt.meibo888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wfq.xingfuxueyuan.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yac.gogol.net.cn

TS:   if (s === "") {}
来源：http://tjo.svipenyu.cn

Java: if (s.isEmpty()) {}
来源：http://ino.zhiwuduotai.top

Go:   if s == "" {}
来源：http://kec.chenzaomai.com

Ruby: if s.empty?
来源：http://qzz.hysaishi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uui.fehbvm.com

[E21] 超长截断加省略号
来源：http://xgc.xziqi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bgo.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gli.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://awm.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rdm.meibo888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rtb.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://cdw.0kj1m.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hbg.zhaomingkeji.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xyt.cucudq.cn

[E22] 字节长度与字符长度
来源：http://pft.yuxming.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qiu.fanxiaobao.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qpc.havefunace.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rxl.shzxlz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tyx.gaohongyu789.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tbn.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ubl.shzxlz.cn

Ruby: s.bytesize;  s.length
来源：http://yin.kuanghao11.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rwu.hongshengwenyu.top

================================================================================
来源：http://pet.jianghu66.top

F. 文件与目录
来源：http://ihi.shangyingyoupin.top

================================================================================
来源：http://ait.52xcode.cn

[F01] 读取整个文件
来源：http://eke.quarkkingdee.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ivq.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://ibl.sysykeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://efr.uphjek.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://aga.ywan-chungtsiang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vit.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zdc.guowangkeji.top

Ruby: File.read("a.txt")
来源：http://ign.havefunace.top

C#:   File.ReadAllText("a.txt");
来源：http://cns.yongpay.top

[F02] 逐行读取文件
来源：http://jfc.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://och.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pbp.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xli.yuxming.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wyi.cashguo.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://byk.ybcxt.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ddt.sufxvd.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ptz.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wba.ivvv.top

[F03] 写入文件（覆盖）
来源：http://emm.tian-w.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nue.sweek.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vla.yanxiufei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bdu.shuidangran.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rbf.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bve.epnwcf.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pdi.jiagoushi.top

Ruby: File.write("a.txt", "hi")
来源：http://pbh.wangdashe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://odw.guowangkeji.top

[F04] 追加写入文件
来源：http://vdl.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dls.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mzs.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://moc.sxryk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ept.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ght.yonumen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aas.yj20258888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tka.ctjpmb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lxp.nanxuanxn.top

[F05] 判断文件或目录是否存在
来源：http://ovc.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tim.fengsongda.top

PHP:  file_exists("a.txt");
来源：http://avc.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://vgk.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://hsn.guannengcc.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hia.vqdsnc.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fei.yuanzhike.top

Ruby: File.exist?("a.txt")
来源：http://ehe.cheryme.top

C#:   File.Exists("a.txt")
来源：http://jzg.zhaomingkeji.xyz

[F06] 删除文件
来源：http://nlz.ywan-chungtsiang.top

Py:   os.remove("a.txt")
来源：http://bjj.ydzc1.top

PHP:  unlink("a.txt");
来源：http://iay.zhaomingkeji.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://vew.hammf.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oyi.zdbjq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mqg.ywan-chungtsiang.top

Go:   os.Remove("a.txt")
来源：http://ckn.ivvv.top

Ruby: File.delete("a.txt")
来源：http://nvf.hysaishi.cn

C#:   File.Delete("a.txt");
来源：http://bxm.c1oappe.top

[F07] 创建目录（含多级）
来源：http://ngi.tian-w.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ilb.cucudq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qvw.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kim.sysykeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zom.guowangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mvw.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dwp.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rhm.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xbq.hammf.cn

[F08] 遍历目录
来源：http://pvp.nanxuanxn.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jfm.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dpt.sweek.top

JS:   fs.readdirSync("dir")
来源：http://gms.epnwcf.com

TS:   fs.readdirSync("dir")
来源：http://ktl.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://acq.quarkkingdee.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mec.pycfn.com

Ruby: Dir.children("dir")
来源：http://fpu.cashguo.top

C#:   Directory.GetFiles("dir")
来源：http://ilc.sjlbkw.cn

[F09] 获取文件大小
来源：http://zdm.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://dlc.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://pxo.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://nrz.andypj.xyz

TS:   fs.statSync("a.txt").size
来源：http://rfq.aizwys.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ikz.feifeiyinyue.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://znc.hysaishi.cn

Ruby: File.size("a.txt")
来源：http://pld.zdqjudy.top

C#:   new FileInfo("a.txt").Length
来源：http://knc.ivvv.top

[F10] 取文件扩展名 / 文件名
来源：http://lcm.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sjx.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fsm.chenzaomai.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nki.jinghuilouyu.cn

TS:   path.extname("a.txt")
来源：http://ovn.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ttg.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ikl.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gxv.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cnf.iojbl.cn

[F11] 复制与移动文件
来源：http://hub.iojbl.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ksh.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hir.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://isg.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kwv.ybcxt.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ndn.yfazqb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ynd.hesvh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ufb.jiagoushi.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wsh.c1oappe.top

[F12] CSV 读写
来源：http://cqe.nanxinkj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cmo.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mlf.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bex.zhengqikj.top

TS:   // 同上
来源：http://cbl.jlsjyb.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://csk.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fza.meibo888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://erv.jinqigufen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kdt.zdbjq.cn

================================================================================
来源：http://bos.kuanghao11.cn

G. 面向对象
来源：http://gmj.jinyuanbaomall.cn

================================================================================
来源：http://cex.dianchejie.cn

[G01] 定义类
来源：http://lmz.yangfankeji.com

Py:   class User: pass
来源：http://zsy.hysaishi.cn

PHP:  class User {}
来源：http://wwj.uphjek.com

JS:   class User {}
来源：http://yta.chenlongwang.top

TS:   class User { name: string = ""; }
来源：http://vke.guowangkeji.top

Java: class User {}
来源：http://jtp.daria6918.cn

Go:   type User struct { Name string }
来源：http://ftp.xylfe.cn

Ruby: class User; end
来源：http://dta.tanke756.top

C#:   class User {}
来源：http://fxw.yfazqb.com

[G02] 构造函数
来源：http://wtw.c1oappe.top

Py:   def __init__(self, name): self.name = name
来源：http://ack.guannengcc.top

PHP:  public function __construct(public string $name) {}
来源：http://mqf.yuanzhike.top

JS:   constructor(name) { this.name = name; }
来源：http://xxh.cqqwz.cn

TS:   constructor(public name: string) {}
来源：http://ilr.pengpengdd.cyou

Java: User(String name) { this.name = name; }
来源：http://alg.zhaomingkeji.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ubr.ybcxt.top

Ruby: def initialize(name); @name = name; end
来源：http://ctk.shzxlz.cn

C#:   public User(string name) { Name = name; }
来源：http://hvw.jiagoushi.top

[G03] 实例属性
来源：http://mxy.fengsongda.top

Py:   self.name = "x"
来源：http://pjw.ydzc1.top

PHP:  public string $name = "x";
来源：http://kxx.yonumen.top

JS:   this.name = "x";
来源：http://uzw.jyoumei.cn

TS:   name: string = "x";
来源：http://vmz.xuanzx.com

Java: private String name;
来源：http://jme.jinghuilouyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://osr.hesvh.cn

Ruby: @name = "x"
来源：http://yvu.nanxuanxn.top

C#:   public string Name { get; set; } = "x";
来源：http://edd.sweek.top

[G04] 定义方法
来源：http://upr.sjlbkw.cn

Py:   def greet(self): return self.name
来源：http://ebq.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qpt.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://jkm.wangshuangyany.cn

TS:   greet(): string { return this.name; }
来源：http://wvb.ywan-chungtsiang.top

Java: String greet() { return name; }
来源：http://btj.sysykeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://byv.mhx1999.top

Ruby: def greet; @name; end
来源：http://nlq.jinqigufen.top

C#:   public string Greet() => Name;
来源：http://nsv.aibaodan.cn

[G05] 继承
来源：http://sri.haohaochexian.top

Py:   class Admin(User): pass
来源：http://wbo.jinqigufen.top

PHP:  class Admin extends User {}
来源：http://lxj.jyoumei.cn

JS:   class Admin extends User {}
来源：http://qdw.gotoacloud.top

TS:   class Admin extends User {}
来源：http://wly.sysykeji.top

Java: class Admin extends User {}
来源：http://dvi.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qjt.havefunace.top

Ruby: class Admin < User; end
来源：http://kwn.zhaomingkeji.xyz

C#:   class Admin : User {}
来源：http://wcx.yj20258888.top

[G06] 重写方法
来源：http://auc.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://xfa.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://atb.xuetiantiany.cn

JS:   greet() { return "admin"; }
来源：http://mgy.cdnleiting.top

TS:   greet(): string { return "admin"; }
来源：http://oif.hywenlv.cn

Java: @Override String greet() { return "admin"; }
来源：http://hac.vqdsnc.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rdk.ywan-chungtsiang.top

Ruby: def greet; "admin"; end
来源：http://iqu.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://vaa.jianghu66.top

[G07] 调用父类方法
来源：http://wed.birdmap.top

Py:   super().greet()
来源：http://vie.cashguo.top

PHP:  parent::greet();
来源：http://vmw.smart0.xyz

JS:   super.greet();
来源：http://xvn.cucudq.cn

TS:   super.greet();
来源：http://toh.yuanzhike.top

Java: super.greet();
来源：http://pjy.zycfv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uir.haohaochexian.top

Ruby: super
来源：http://bzf.shuidangran.top

C#:   base.Greet();
来源：http://ykj.quarkkingdee.top

[G08] 静态方法与属性
来源：http://vwb.hammf.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zcs.jinqigufen.top

PHP:  public static function f() {}
来源：http://ndg.xylfe.cn

JS:   static f() {}
来源：http://ugz.zhongyouzk.top

TS:   static f(): void {}
来源：http://gvc.mhx1999.top

Java: static void f() {}
来源：http://kaw.tarul.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uzw.gogol.net.cn

Ruby: def self.f; end
来源：http://tut.zhijiandao.cn

C#:   public static void F() {}
来源：http://sos.xuetiantiany.cn

[G09] 接口 / 抽象类
来源：http://ten.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://hfe.hnqzz.top

PHP:  interface Shape { public function area(): float; }
来源：http://zzl.shangyingyoupin.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ycw.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://lkz.shangyingyoupin.top

Java: interface Shape { double area(); }
来源：http://mcs.hcnkem.com

Go:   type Shape interface { Area() float64 }
来源：http://qzo.yvedp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kox.sufxvd.cn

C#:   interface IShape { double Area(); }
来源：http://azg.daria6918.cn

[G10] 访问控制
来源：http://kad.xuetiantiany.cn

Py:   约定 _protected / __private（不强制）
来源：http://xqt.yuanzhike.top

PHP:  public / protected / private
来源：http://nrn.shangyingyoupin.top

JS:   #private 字段；其余公开
来源：http://ngq.fehbvm.com

TS:   public / protected / private
来源：http://rmj.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://xgt.fehbvm.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://nqi.shangyingyoupin.top

Ruby: public / protected / private
来源：http://lgq.gaohongyu789.top

C#:   public / protected / private / internal
来源：http://vti.epnwcf.com

[G11] getter / setter
来源：http://rmw.zdqjudy.top

Py:   @property 与 @x.setter
来源：http://tkq.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qxm.zdqjudy.top

JS:   get name() { return this._name; }
来源：http://rdp.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://aag.mhx1999.top

Java: public String getName() { return name; }
来源：http://cto.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://iuw.ivvv.top

Ruby: attr_accessor :name
来源：http://uac.jiagoushi.top

C#:   public string Name { get; set; }
来源：http://skz.52xcode.cn

[G12] 对象转字符串
来源：http://arx.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://glk.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://vhv.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://yyy.uphjek.com

TS:   toString(): string { return this.name; }
来源：http://fbn.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://myh.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cws.yonumen.top

Ruby: def to_s; @name; end
来源：http://hut.shanyushiyangtech.top

C#:   public override string ToString() => Name;
来源：http://xsx.yangfankeji.com

[G13] 判断对象类型
来源：http://jku.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://qzq.gaohongyu789.top

PHP:  $u instanceof User
来源：http://yrt.yj20258888.top

JS:   u instanceof User
来源：http://lqb.vehdjk.com

TS:   u instanceof User
来源：http://ccq.fzhhl.top

Java: u instanceof User
来源：http://oek.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ias.shuidangran.top

Ruby: u.is_a?(User)
来源：http://bge.smart0.xyz

C#:   u is User
来源：http://oox.yvedp.cn

[G14] 数据类 / record
来源：http://mlm.sufxvd.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eta.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://hws.zhaomingkeji.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://yts.ivvv.top

TS:   type User = { name: string; age: number };
来源：http://ajo.yonumen.top

Java: record User(String name, int age) {}
来源：http://giq.yj20258.top

Go:   type User struct { Name string; Age int }
来源：http://kcq.gotoacloud.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://afa.yj20258.top

C#:   record User(string Name, int Age);
来源：http://cdc.uphjek.com

[G15] 枚举
来源：http://ggb.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iki.hongshengwenyu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mkf.52xcode.cn


<!-- 参考信息 -->
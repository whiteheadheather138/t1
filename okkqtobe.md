代发 wailian999

[E18] 模板占位符替换
来源：http://xrd.sxryk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yfw.cheryme.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ujw.shanyushiyangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qap.redwolf501.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ric.xingfuxueyuan.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gkl.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://edd.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ask.fktsv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://reb.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://bax.yj20258.top

Py:   s.splitlines()
来源：http://qox.birdmap.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cty.zhixingplan.top

JS:   s.split(/\r?\n/)
来源：http://tbd.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://eeo.zycfv.cn

Java: s.lines().toList()
来源：http://wll.fengsongda.top

Go:   strings.Split(s, "\n")
来源：http://wku.wangdashe.top

Ruby: s.lines
来源：http://kiu.zdbjq.cn

C#:   s.Split('\n')
来源：http://nbd.meibo888.top

[E20] 判断字符串是否为空
来源：http://pma.kuanghao11.cn

Py:   if not s:
来源：http://krq.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://msc.nwbrower.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://btp.nwbrower.top

TS:   if (s === "") {}
来源：http://zzn.dianchejie.cn

Java: if (s.isEmpty()) {}
来源：http://pev.guannengcc.top

Go:   if s == "" {}
来源：http://dnj.andypj.xyz

Ruby: if s.empty?
来源：http://yjt.hnqzz.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qxz.yanxiufei.cn

[E21] 超长截断加省略号
来源：http://eno.fktsv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yzi.chenlongwang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://omq.yangfankeji.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hbv.yj20258888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xtz.shuidangran.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://drd.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://snl.c1oappe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cos.daxiang520.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lmu.yvedp.cn

[E22] 字节长度与字符长度
来源：http://xac.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bjl.sysykeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tat.cqqwz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tpq.jyoumei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hrl.iojbl.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bol.nwbrower.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://efj.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://tsc.ctjpmb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ozc.gogol.net.cn

================================================================================
来源：http://dhh.zhengqikj.top

F. 文件与目录
来源：http://rjj.316326.xyz

================================================================================
来源：http://lpq.hywenlv.cn

[F01] 读取整个文件
来源：http://sun.hongshengwenyu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fmw.zhoulong.xyz

PHP:  file_get_contents("a.txt");
来源：http://fgl.hammf.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ehw.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://won.meibo888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jlj.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hlf.tanke756.top

Ruby: File.read("a.txt")
来源：http://oqy.mhx1999.top

C#:   File.ReadAllText("a.txt");
来源：http://uem.ivvv.top

[F02] 逐行读取文件
来源：http://dcu.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xul.hysaishi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lfg.hywenlv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dcx.shuidangran.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xrt.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eiq.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fvp.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://utq.cdnleiting.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vsc.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://coj.quarkkingdee.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fyn.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mzh.iojbl.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wxw.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mzp.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tys.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lat.tarul.cn

Ruby: File.write("a.txt", "hi")
来源：http://dur.xingfuxueyuan.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lkz.tian-w.cn

[F04] 追加写入文件
来源：http://enj.0kj1m.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tmh.smart0.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xym.yvedp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://egh.nanxuanxn.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://end.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vys.quarkkingdee.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xua.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jdm.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mko.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://ded.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kud.yj202588.top

PHP:  file_exists("a.txt");
来源：http://nac.gaohongyu789.top

JS:   fs.existsSync("a.txt")
来源：http://kyz.yfazqb.com

TS:   fs.existsSync("a.txt")
来源：http://qzl.hcnkem.com

Java: Files.exists(Path.of("a.txt"))
来源：http://nth.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vlp.uphjek.com

Ruby: File.exist?("a.txt")
来源：http://lai.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://gmn.vehdjk.com

[F06] 删除文件
来源：http://djy.hysaishi.cn

Py:   os.remove("a.txt")
来源：http://okr.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://ukh.zhaomingkeji.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://jeu.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://seu.mhx1999.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xhh.fzhhl.top

Go:   os.Remove("a.txt")
来源：http://nuk.yj202588.top

Ruby: File.delete("a.txt")
来源：http://ogg.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://hpc.yuxming.cn

[F07] 创建目录（含多级）
来源：http://knw.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://psh.jianghu66.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iyg.ywan-chungtsiang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fql.jqgufenzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://urs.ybcxt.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aiu.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wcl.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jat.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lrv.zycfv.cn

[F08] 遍历目录
来源：http://sbi.mhx1999.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xgd.jlsjyb.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gfp.daria6918.cn

JS:   fs.readdirSync("dir")
来源：http://lvm.svipenyu.cn

TS:   fs.readdirSync("dir")
来源：http://jkv.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ugy.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ioy.sysykeji.top

Ruby: Dir.children("dir")
来源：http://jku.chenjidiqi.icu

C#:   Directory.GetFiles("dir")
来源：http://cma.nanxinkj.top

[F09] 获取文件大小
来源：http://sbu.shuidangran.top

Py:   os.path.getsize("a.txt")
来源：http://kqg.xinyue.icu

PHP:  filesize("a.txt");
来源：http://qzp.hywenlv.cn

JS:   fs.statSync("a.txt").size
来源：http://dfj.jinghuilouyu.cn

TS:   fs.statSync("a.txt").size
来源：http://ucf.fanxiaobao.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://nwk.hnxiangtu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nlw.gzhubu.top

Ruby: File.size("a.txt")
来源：http://owd.cashguo.top

C#:   new FileInfo("a.txt").Length
来源：http://xxt.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://bjl.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dzr.zhiwuduotai.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kem.ywan-chungtsiang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ocb.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://rej.pengpengdd.cyou

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uhu.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://klp.gzhubu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://szv.hammf.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qgj.daria6918.cn

[F11] 复制与移动文件
来源：http://rbt.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jlo.jinqigufen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://azj.jqgufenzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qpf.hcnkem.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://odf.cdnleiting.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ipi.iojbl.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fnv.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ijb.jyoumei.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tsk.hnxiangtu.top

[F12] CSV 读写
来源：http://hsq.hammf.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zkz.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vxj.zhixingplan.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://net.ydjk.org.cn

TS:   // 同上
来源：http://cru.chenjidiqi.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qeq.cashguo.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sth.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cwb.hnxiangtu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nsl.yj20258888.top

================================================================================
来源：http://kzo.yj202588.top

G. 面向对象
来源：http://rtu.shanyushiyangtech.top

================================================================================
来源：http://usx.chenlongwang.top

[G01] 定义类
来源：http://lhp.guowangkeji.top

Py:   class User: pass
来源：http://hzq.fengsongda.top

PHP:  class User {}
来源：http://yor.hesvh.cn

JS:   class User {}
来源：http://byk.ydzc1.top

TS:   class User { name: string = ""; }
来源：http://npg.hammf.cn

Java: class User {}
来源：http://pyn.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://tql.yueranfly.top

Ruby: class User; end
来源：http://psh.aizwys.cn

C#:   class User {}
来源：http://isz.9152youxi.cn

[G02] 构造函数
来源：http://aki.guannengcc.top

Py:   def __init__(self, name): self.name = name
来源：http://utt.sysykeji.top

PHP:  public function __construct(public string $name) {}
来源：http://tkt.hongshengwenyu.top

JS:   constructor(name) { this.name = name; }
来源：http://zfi.shuidangran.top

TS:   constructor(public name: string) {}
来源：http://vok.shangyingyoupin.top

Java: User(String name) { this.name = name; }
来源：http://hrc.yonumen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tvl.bbcook.cn

Ruby: def initialize(name); @name = name; end
来源：http://wli.vqdsnc.cn

C#:   public User(string name) { Name = name; }
来源：http://cal.ybcxt.top

[G03] 实例属性
来源：http://cli.zycfv.cn

Py:   self.name = "x"
来源：http://ssh.gogol.net.cn

PHP:  public string $name = "x";
来源：http://daw.zdqjudy.top

JS:   this.name = "x";
来源：http://zuv.chenjidiqi.icu

TS:   name: string = "x";
来源：http://mhh.hcnkem.com

Java: private String name;
来源：http://lwm.haohaochexian.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vvs.zhaomingkeji.xyz

Ruby: @name = "x"
来源：http://frh.pengpengdd.cyou

C#:   public string Name { get; set; } = "x";
来源：http://bte.smart0.xyz

[G04] 定义方法
来源：http://ems.jyoumei.cn

Py:   def greet(self): return self.name
来源：http://wwk.gzhubu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bvq.ywan-chungtsiang.top

JS:   greet() { return this.name; }
来源：http://lpr.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://waw.chenlongwang.top

Java: String greet() { return name; }
来源：http://fdg.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://aeb.jinqigufen.top

Ruby: def greet; @name; end
来源：http://iua.sxryk.cn

C#:   public string Greet() => Name;
来源：http://qlc.daria6918.cn

[G05] 继承
来源：http://ymp.yanxiufei.cn

Py:   class Admin(User): pass
来源：http://svn.pengpengdd.cyou

PHP:  class Admin extends User {}
来源：http://pqw.hongshengwenyu.top

JS:   class Admin extends User {}
来源：http://iue.nwbrower.top

TS:   class Admin extends User {}
来源：http://wyv.smart0.xyz

Java: class Admin extends User {}
来源：http://tzi.c1oappe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jav.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://beu.chenzaomai.com

C#:   class Admin : User {}
来源：http://cep.birdmap.top

[G06] 重写方法
来源：http://ywr.hammf.cn

Py:   def greet(self): return "admin"
来源：http://afy.havefunace.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zvn.xuetiantiany.cn

JS:   greet() { return "admin"; }
来源：http://dxz.fzhhl.top

TS:   greet(): string { return "admin"; }
来源：http://wxh.hysaishi.cn

Java: @Override String greet() { return "admin"; }
来源：http://its.dashuyun.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hwf.chenlongwang.top

Ruby: def greet; "admin"; end
来源：http://qet.sjlbkw.cn

C#:   public override string Greet() => "admin";
来源：http://rog.9152youxi.cn

[G07] 调用父类方法
来源：http://nre.sysykeji.top

Py:   super().greet()
来源：http://dev.jqgufenzy.top

PHP:  parent::greet();
来源：http://apu.zhiwuduotai.top

JS:   super.greet();
来源：http://lsk.epnwcf.com

TS:   super.greet();
来源：http://dql.yongpay.top

Java: super.greet();
来源：http://hfs.jqgfzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zzh.guannengcc.top

Ruby: super
来源：http://yfz.sysykeji.top

C#:   base.Greet();
来源：http://qgr.dianchejie.cn

[G08] 静态方法与属性
来源：http://ecs.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hcl.meibo888.top

PHP:  public static function f() {}
来源：http://akn.smart0.xyz

JS:   static f() {}
来源：http://lym.cqqwz.cn

TS:   static f(): void {}
来源：http://vua.snrcjt.cn

Java: static void f() {}
来源：http://lba.yj202588.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ntl.sweek.top

Ruby: def self.f; end
来源：http://znd.shuidangran.top

C#:   public static void F() {}
来源：http://nqi.mhx1999.top

[G09] 接口 / 抽象类
来源：http://vwt.chenlongwang.top

Py:   from abc import ABC, abstractmethod
来源：http://arp.52xcode.cn

PHP:  interface Shape { public function area(): float; }
来源：http://aok.ybcxt.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://axs.cqqwz.cn

TS:   interface Shape { area(): number; }
来源：http://ile.shuidangran.top

Java: interface Shape { double area(); }
来源：http://wlg.cqqwz.cn

Go:   type Shape interface { Area() float64 }
来源：http://mwn.fengsongda.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dxx.zdqjudy.top

C#:   interface IShape { double Area(); }
来源：http://ytv.jinghuilouyu.cn

[G10] 访问控制
来源：http://hck.shuidangran.top

Py:   约定 _protected / __private（不强制）
来源：http://cwa.jlsjyb.cn

PHP:  public / protected / private
来源：http://wcv.vqdsnc.cn

JS:   #private 字段；其余公开
来源：http://rdd.52xcode.cn

TS:   public / protected / private
来源：http://gua.dashuyun.cn

Java: public / protected / private / 默认包级
来源：http://ura.hammf.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bqn.pengpengdd.cyou

Ruby: public / protected / private
来源：http://dyf.dianchejie.cn

C#:   public / protected / private / internal
来源：http://qdr.dashuyun.cn

[G11] getter / setter
来源：http://aht.cashguo.top

Py:   @property 与 @x.setter
来源：http://hdx.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qjn.quarkkingdee.top

JS:   get name() { return this._name; }
来源：http://hjl.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://cjr.smart0.xyz

Java: public String getName() { return name; }
来源：http://vrh.jinqigfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://puv.shzxlz.cn

Ruby: attr_accessor :name
来源：http://ebw.sxryk.cn

C#:   public string Name { get; set; }
来源：http://vjg.tarul.cn

[G12] 对象转字符串
来源：http://kfi.birdmap.top

Py:   def __str__(self): return self.name
来源：http://bfz.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://yhm.sweek.top

JS:   toString() { return this.name; }
来源：http://ytq.epnwcf.com

TS:   toString(): string { return this.name; }
来源：http://ayd.shanyushiyangtech.top

Java: @Override public String toString() { return name; }
来源：http://esi.jinqigufen.top

Go:   func (u User) String() string { return u.Name }
来源：http://zoi.birdmap.top

Ruby: def to_s; @name; end
来源：http://pkr.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://ejo.birdmap.top

[G13] 判断对象类型
来源：http://ctp.tarul.cn

Py:   isinstance(u, User)
来源：http://yog.yonumen.top

PHP:  $u instanceof User
来源：http://fvu.cucudq.cn

JS:   u instanceof User
来源：http://vwk.sufxvd.cn

TS:   u instanceof User
来源：http://fvk.nwbrower.top

Java: u instanceof User
来源：http://cmp.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://xeb.hnqzz.top

Ruby: u.is_a?(User)
来源：http://lth.yuxming.cn

C#:   u is User
来源：http://oqn.fanxiaobao.xyz

[G14] 数据类 / record
来源：http://nrw.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wqa.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://crp.316326.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://okv.aibaodan.cn

TS:   type User = { name: string; age: number };
来源：http://upi.fktsv.cn

Java: record User(String name, int age) {}
来源：http://ias.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://ywe.ybcxt.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ani.xingfuxueyuan.xyz

C#:   record User(string Name, int Age);
来源：http://ucr.dashuyun.cn

[G15] 枚举
来源：http://lfv.yongpay.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gfn.zhijiandao.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nir.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://giu.xziqi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yho.shangyingyoupin.top

Java: enum Color { RED, GREEN }
来源：http://rgy.ehwqpu.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hgo.zhaomingkeji.xyz

Ruby: Color = %i[red green].freeze
来源：http://mql.meibo888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lyb.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://kyx.dashuyun.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://msi.guannengcc.top

PHP:  get_object_vars($obj);
来源：http://njt.ppjwa.cn

JS:   Object.entries(obj)
来源：http://epf.yuanzhike.top

TS:   Object.entries(obj)
来源：http://qrj.sjlbkw.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yqf.xuetiantiany.cn


<!-- 参考信息 -->
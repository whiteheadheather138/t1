代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qsg.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oen.yongpay.top

Ruby: s.capitalize
来源：http://fda.epnwcf.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vkt.tanke756.top

[E18] 模板占位符替换
来源：http://cjm.gogol.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yop.316326.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tue.cqqwz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xzu.c1oappe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dal.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://exh.tian-w.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://asx.guowangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nnl.daria6918.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bud.shzxlz.cn

[E19] 多行文本按行拆分
来源：http://vdh.ctjpmb.com

Py:   s.splitlines()
来源：http://ook.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oez.fehbvm.com

JS:   s.split(/\r?\n/)
来源：http://umn.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://jok.smart0.xyz

Java: s.lines().toList()
来源：http://esk.fengsongda.top

Go:   strings.Split(s, "\n")
来源：http://uba.tianlin.xyz

Ruby: s.lines
来源：http://oqa.tanke756.top

C#:   s.Split('\n')
来源：http://mav.daria6918.cn

[E20] 判断字符串是否为空
来源：http://ihq.daria6918.cn

Py:   if not s:
来源：http://czz.yfazqb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tbi.sxryk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://trb.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://yib.cheryme.top

Java: if (s.isEmpty()) {}
来源：http://hrx.52xcode.cn

Go:   if s == "" {}
来源：http://uuf.chenjidiqi.icu

Ruby: if s.empty?
来源：http://djp.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rxj.sweek.top

[E21] 超长截断加省略号
来源：http://tov.zdqjudy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tsk.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ech.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cgj.316326.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dxy.nanxinkj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qjf.chenzaomai.com

Go:   // 按 rune 判断长度后截断
来源：http://bha.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ebu.hongshengwenyu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qgt.yfazqb.com

[E22] 字节长度与字符长度
来源：http://xyk.0kj1m.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wuu.tian-w.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ivc.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nnc.jlsjyb.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fdj.zhijiandao.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hax.cdnleiting.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vzr.cashguo.top

Ruby: s.bytesize;  s.length
来源：http://nex.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rwt.aibaodan.cn

================================================================================
来源：http://ncg.hcnkem.com

F. 文件与目录
来源：http://mne.shzxlz.cn

================================================================================
来源：http://vjt.9152youxi.cn

[F01] 读取整个文件
来源：http://oqo.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iwo.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://sjz.daria6918.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xus.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lbq.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://oss.shuidangran.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nii.shanyushiyangkeji.top

Ruby: File.read("a.txt")
来源：http://wbu.jqgfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://iko.daxiang520.top

[F02] 逐行读取文件
来源：http://mre.pengpengdd.cyou

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hka.svipenyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://inf.meibo888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wmp.fzhhl.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://psf.yfazqb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qzl.nwbrower.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nsw.ctjpmb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dwa.gzhubu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://not.epnwcf.com

[F03] 写入文件（覆盖）
来源：http://tbk.yanxiufei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://knj.chenlongwang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://epw.vqdsnc.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ogk.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gal.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://efc.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tcv.jqgfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://dpb.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vqs.hcnkem.com

[F04] 追加写入文件
来源：http://eml.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://but.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iec.fengsongda.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mhv.pycfn.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ppl.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fqa.tanke756.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mqr.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vba.wangdashe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vfb.epnwcf.com

[F05] 判断文件或目录是否存在
来源：http://btq.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eot.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://mxc.ctjpmb.com

JS:   fs.existsSync("a.txt")
来源：http://ups.316326.xyz

TS:   fs.existsSync("a.txt")
来源：http://lgr.xziqi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zjc.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nvn.shuidangran.top

Ruby: File.exist?("a.txt")
来源：http://tdd.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://rat.hfpthk.cn

[F06] 删除文件
来源：http://jov.fengsongda.top

Py:   os.remove("a.txt")
来源：http://frc.9152youxi.cn

PHP:  unlink("a.txt");
来源：http://bnz.dianchejie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vvd.yfazqb.com

TS:   fs.unlinkSync("a.txt")
来源：http://wes.chenzaomai.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oac.shanyushiyangkeji.top

Go:   os.Remove("a.txt")
来源：http://owm.daxiang520.top

Ruby: File.delete("a.txt")
来源：http://djx.cheryme.top

C#:   File.Delete("a.txt");
来源：http://kyr.ywan-chungtsiang.top

[F07] 创建目录（含多级）
来源：http://alm.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xbw.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wii.vqdsnc.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ufe.hesvh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ndx.nwbrower.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rix.tianlin.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bne.hnqzz.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wgc.feifeiyinyue.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ymg.xuanzx.com

[F08] 遍历目录
来源：http://yao.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bxg.zhaomingkeji.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ayh.jinyuanbaomall.cn

JS:   fs.readdirSync("dir")
来源：http://qqk.zhixingplan.top

TS:   fs.readdirSync("dir")
来源：http://taf.yj202588.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bqs.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wce.hnxiangtu.top

Ruby: Dir.children("dir")
来源：http://xuj.cashguo.top

C#:   Directory.GetFiles("dir")
来源：http://vlk.tarul.cn

[F09] 获取文件大小
来源：http://del.tianlin.xyz

Py:   os.path.getsize("a.txt")
来源：http://bti.yueranfly.top

PHP:  filesize("a.txt");
来源：http://jkt.shanyushiyangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://rbv.shzxlz.cn

TS:   fs.statSync("a.txt").size
来源：http://szr.birdmap.top

Java: Files.size(Path.of("a.txt"))
来源：http://xrf.jlsjyb.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tpg.redwolf501.top

Ruby: File.size("a.txt")
来源：http://bdq.fzhhl.top

C#:   new FileInfo("a.txt").Length
来源：http://djb.tanke756.top

[F10] 取文件扩展名 / 文件名
来源：http://wyo.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://onc.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zef.zhaomingkeji.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ymp.0kj1m.cn

TS:   path.extname("a.txt")
来源：http://bwq.jinqigufen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bhd.jqgfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mhx.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://egn.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tjx.xylfe.cn

[F11] 复制与移动文件
来源：http://bpg.bjfxy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rgw.yj20258.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kwd.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vep.andypj.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uul.sweek.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mwq.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zlg.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ulc.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gnq.mhx1999.top

[F12] CSV 读写
来源：http://oiz.yueranfly.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gyt.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kka.dashuyun.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ghl.c1oappe.top

TS:   // 同上
来源：http://ezv.ydzc1.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hjt.hnxiangtu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gbq.xylfe.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ctr.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://esr.cheryme.top

================================================================================
来源：http://oep.9152youxi.cn

G. 面向对象
来源：http://nvo.xingfuxueyuan.xyz

================================================================================
来源：http://ogi.birdmap.top

[G01] 定义类
来源：http://ufv.xuanzx.com

Py:   class User: pass
来源：http://lcx.ywan-chungtsiang.top

PHP:  class User {}
来源：http://yxd.quarkkingdee.top

JS:   class User {}
来源：http://qye.hfpthk.cn

TS:   class User { name: string = ""; }
来源：http://grp.jinghuilouyu.cn

Java: class User {}
来源：http://kfo.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://lce.ehwqpu.com

Ruby: class User; end
来源：http://sum.jqgufenzy.top

C#:   class User {}
来源：http://ikc.xziqi.cn

[G02] 构造函数
来源：http://kdd.xingfuxueyuan.xyz

Py:   def __init__(self, name): self.name = name
来源：http://dqg.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://zfa.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://tqv.zhiwuduotai.top

TS:   constructor(public name: string) {}
来源：http://ccc.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://xpl.yongpay.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kgs.jqgfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://mhs.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://qss.cashguo.top

[G03] 实例属性
来源：http://ulv.cdnleiting.top

Py:   self.name = "x"
来源：http://zch.cqqwz.cn

PHP:  public string $name = "x";
来源：http://pdw.yj202588.top

JS:   this.name = "x";
来源：http://oba.yonumen.top

TS:   name: string = "x";
来源：http://fvw.hywenlv.cn

Java: private String name;
来源：http://xdi.xingfuxueyuan.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qdm.fzhhl.top

Ruby: @name = "x"
来源：http://fng.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://xaz.tian-w.cn

[G04] 定义方法
来源：http://uja.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://aye.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lmw.feifeiyinyue.top

JS:   greet() { return this.name; }
来源：http://sdk.sxryk.cn

TS:   greet(): string { return this.name; }
来源：http://wek.c1oappe.top

Java: String greet() { return name; }
来源：http://sfm.ppjwa.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lja.jinqigufen.top

Ruby: def greet; @name; end
来源：http://dxf.hfpthk.cn

C#:   public string Greet() => Name;
来源：http://ygc.gaohongyu789.top

[G05] 继承
来源：http://cyy.ydjk.org.cn

Py:   class Admin(User): pass
来源：http://gms.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://ieu.xingfuxueyuan.xyz

JS:   class Admin extends User {}
来源：http://owd.gogol.net.cn

TS:   class Admin extends User {}
来源：http://ahi.guannengcc.top

Java: class Admin extends User {}
来源：http://wlf.yuanzhike.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://abt.yueranfly.top

Ruby: class Admin < User; end
来源：http://adr.shangyingyoupin.top

C#:   class Admin : User {}
来源：http://pzs.gogol.net.cn

[G06] 重写方法
来源：http://zai.hesvh.cn

Py:   def greet(self): return "admin"
来源：http://xts.zycfv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rov.gzhubu.top

JS:   greet() { return "admin"; }
来源：http://all.birdmap.top

TS:   greet(): string { return "admin"; }
来源：http://msq.gzhubu.top

Java: @Override String greet() { return "admin"; }
来源：http://rha.yj20258.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gnw.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://ztl.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://jen.epnwcf.com

[G07] 调用父类方法
来源：http://yrh.dashuyun.cn

Py:   super().greet()
来源：http://ebz.tanke756.top

PHP:  parent::greet();
来源：http://kyz.guannengcc.top

JS:   super.greet();
来源：http://ofx.epnwcf.com

TS:   super.greet();
来源：http://wbg.yj202588.top

Java: super.greet();
来源：http://jkw.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cgz.andypj.xyz

Ruby: super
来源：http://fug.sjlbkw.cn

C#:   base.Greet();
来源：http://bht.0kj1m.cn

[G08] 静态方法与属性
来源：http://sjg.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jsb.gzhubu.top

PHP:  public static function f() {}
来源：http://fvl.smart0.xyz

JS:   static f() {}
来源：http://bjp.zdqjudy.top

TS:   static f(): void {}
来源：http://vqb.gogol.net.cn

Java: static void f() {}
来源：http://mqo.shzxlz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xdu.iojbl.cn

Ruby: def self.f; end
来源：http://ipc.epnwcf.com

C#:   public static void F() {}
来源：http://can.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://lfl.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://qzs.shangyingyoupin.top

PHP:  interface Shape { public function area(): float; }
来源：http://bre.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vfe.tianlin.xyz

TS:   interface Shape { area(): number; }
来源：http://zit.gotoacloud.top

Java: interface Shape { double area(); }
来源：http://xqs.wangshuangyany.cn

Go:   type Shape interface { Area() float64 }
来源：http://gdp.kuanghao11.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dwh.zdbjq.cn

C#:   interface IShape { double Area(); }
来源：http://imk.uphjek.com

[G10] 访问控制
来源：http://kaf.yj20258.top

Py:   约定 _protected / __private（不强制）
来源：http://rna.sweek.top

PHP:  public / protected / private
来源：http://cji.gzhubu.top

JS:   #private 字段；其余公开
来源：http://xen.zhongyouzk.top

TS:   public / protected / private
来源：http://vmd.yj202588.top

Java: public / protected / private / 默认包级
来源：http://acb.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rqv.yanxiufei.cn

Ruby: public / protected / private
来源：http://jbs.zhiwuduotai.top

C#:   public / protected / private / internal
来源：http://yyb.hnxiangtu.top

[G11] getter / setter
来源：http://jnb.wangdashe.top

Py:   @property 与 @x.setter
来源：http://xuf.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ndv.shzxlz.cn

JS:   get name() { return this._name; }
来源：http://gbd.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://lck.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://kct.ehwqpu.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://luu.zhengqikj.top

Ruby: attr_accessor :name
来源：http://rne.xuetiantiany.cn

C#:   public string Name { get; set; }
来源：http://jol.zhaomingkeji.xyz

[G12] 对象转字符串
来源：http://zdz.sufxvd.cn

Py:   def __str__(self): return self.name
来源：http://qgn.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://bvn.ehwqpu.com

JS:   toString() { return this.name; }
来源：http://goa.birdmap.top

TS:   toString(): string { return this.name; }
来源：http://tjg.pycfn.com

Java: @Override public String toString() { return name; }
来源：http://wtk.yanxiufei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sfi.chenjidiqi.icu

Ruby: def to_s; @name; end
来源：http://iyt.epnwcf.com

C#:   public override string ToString() => Name;
来源：http://wsr.iojbl.cn

[G13] 判断对象类型
来源：http://gqw.snrcjt.cn

Py:   isinstance(u, User)
来源：http://yhq.daria6918.cn

PHP:  $u instanceof User
来源：http://lye.epnwcf.com

JS:   u instanceof User
来源：http://iks.jinghuilouyu.cn

TS:   u instanceof User
来源：http://wwu.shanyushiyangkeji.top

Java: u instanceof User
来源：http://wfy.nanxinkj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wjl.yj202588.top

Ruby: u.is_a?(User)
来源：http://jcz.nwbrower.top

C#:   u is User
来源：http://nrs.snrcjt.cn

[G14] 数据类 / record
来源：http://lra.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yka.aibaodan.cn

PHP:  // 用 readonly 属性模拟
来源：http://ler.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lcz.chenzaomai.com

TS:   type User = { name: string; age: number };
来源：http://fle.chenlongwang.top

Java: record User(String name, int age) {}
来源：http://kcp.yj20258.top

Go:   type User struct { Name string; Age int }
来源：http://cyg.chenzaomai.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dnv.52xcode.cn

C#:   record User(string Name, int Age);
来源：http://dps.daria6918.cn

[G15] 枚举
来源：http://ukc.bbcook.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nro.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fmv.sweek.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ouq.hammf.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://efs.fehbvm.com

Java: enum Color { RED, GREEN }
来源：http://zvg.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://noz.zhoulong.xyz

Ruby: Color = %i[red green].freeze
来源：http://fmg.quarkkingdee.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yva.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://gkq.pycfn.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fhm.ctjpmb.com


<!-- 参考信息 -->
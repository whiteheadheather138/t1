代发 wailian999

[E18] 模板占位符替换
来源：http://elj.zycfv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jqs.jinghuilouyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qlw.hysaishi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://skw.cashguo.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lvq.hysaishi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bih.svipenyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zoc.ivvv.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xpc.wangshuangyany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rch.chenjidiqi.icu

[E19] 多行文本按行拆分
来源：http://jie.mhx1999.top

Py:   s.splitlines()
来源：http://smj.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ydk.jlsjyb.cn

JS:   s.split(/\r?\n/)
来源：http://hkc.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://eog.sufxvd.cn

Java: s.lines().toList()
来源：http://lyn.ctjpmb.com

Go:   strings.Split(s, "\n")
来源：http://otp.birdmap.top

Ruby: s.lines
来源：http://iiu.meibo888.top

C#:   s.Split('\n')
来源：http://xfd.wangdashe.top

[E20] 判断字符串是否为空
来源：http://mvb.sjlbkw.cn

Py:   if not s:
来源：http://ucb.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hcr.smart0.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mxv.0kj1m.cn

TS:   if (s === "") {}
来源：http://kpu.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://lss.jqgfzy.top

Go:   if s == "" {}
来源：http://clt.ehwqpu.com

Ruby: if s.empty?
来源：http://pdv.zycfv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aux.dashuyun.cn

[E21] 超长截断加省略号
来源：http://qfp.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pge.ivvv.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://haa.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://git.quarkkingdee.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uan.meibo888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oau.gotoacloud.top

Go:   // 按 rune 判断长度后截断
来源：http://jvk.shangyingyoupin.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://azl.dianchejie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://knc.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://yja.jqgufenzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dwg.jinqigfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vyc.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mgh.zhiwuduotai.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://usn.hongshengwenyu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://isz.xuetiantiany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ccw.shuidangran.top

Ruby: s.bytesize;  s.length
来源：http://ria.ppjwa.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wma.jinyuanbaomall.cn

================================================================================
来源：http://sws.feifeiyinyue.top

F. 文件与目录
来源：http://bxt.ehwqpu.com

================================================================================
来源：http://ppo.redwolf501.top

[F01] 读取整个文件
来源：http://bnz.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qzo.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://qmn.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://spj.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ier.vqdsnc.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://byb.uphjek.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nhc.tanke756.top

Ruby: File.read("a.txt")
来源：http://svf.xuanzx.com

C#:   File.ReadAllText("a.txt");
来源：http://fyp.zhiwuduotai.top

[F02] 逐行读取文件
来源：http://mcn.zhaomingkeji.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vuz.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zlb.zhoulong.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yut.hnxiangtu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://chy.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aku.yanxiufei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jth.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tvg.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cpi.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://ulp.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wre.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xve.nanxuanxn.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://owd.wangdashe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kvd.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oyt.gogol.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://njj.hnqzz.top

Ruby: File.write("a.txt", "hi")
来源：http://alm.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://omo.ppjwa.cn

[F04] 追加写入文件
来源：http://lkt.ivvv.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://emt.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nmy.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lqq.sufxvd.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gng.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jzh.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://skk.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://enf.sxryk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fca.nwbrower.top

[F05] 判断文件或目录是否存在
来源：http://dsy.hywenlv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ckw.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://fay.cdnleiting.top

JS:   fs.existsSync("a.txt")
来源：http://ujo.chenzaomai.com

TS:   fs.existsSync("a.txt")
来源：http://buw.iojbl.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eaq.cucudq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sud.nanxuanxn.top

Ruby: File.exist?("a.txt")
来源：http://alj.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://lei.iojbl.cn

[F06] 删除文件
来源：http://oye.wangdashe.top

Py:   os.remove("a.txt")
来源：http://asw.yvedp.cn

PHP:  unlink("a.txt");
来源：http://bjd.yonumen.top

JS:   fs.unlinkSync("a.txt")
来源：http://umj.birdmap.top

TS:   fs.unlinkSync("a.txt")
来源：http://qjb.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ebf.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://lve.shanyushiyangkeji.top

Ruby: File.delete("a.txt")
来源：http://rcx.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://fhp.fengsongda.top

[F07] 创建目录（含多级）
来源：http://xqv.kuanghao11.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ooe.ehwqpu.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wth.0kj1m.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iji.xingfuxueyuan.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://son.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mgb.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gdb.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pai.chenlongwang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://the.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://shp.bbcook.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lao.hysaishi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mmb.hnxiangtu.top

JS:   fs.readdirSync("dir")
来源：http://ezx.aizwys.cn

TS:   fs.readdirSync("dir")
来源：http://uhu.bbcook.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hur.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rht.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://kff.cheryme.top

C#:   Directory.GetFiles("dir")
来源：http://ydn.ppjwa.cn

[F09] 获取文件大小
来源：http://jdy.jiagoushi.top

Py:   os.path.getsize("a.txt")
来源：http://lmw.shzxlz.cn

PHP:  filesize("a.txt");
来源：http://edm.yuxming.cn

JS:   fs.statSync("a.txt").size
来源：http://jca.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://sfn.xylfe.cn

Java: Files.size(Path.of("a.txt"))
来源：http://obc.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vpu.yj20258888.top

Ruby: File.size("a.txt")
来源：http://hlv.hongshengwenyu.top

C#:   new FileInfo("a.txt").Length
来源：http://bti.9152youxi.cn

[F10] 取文件扩展名 / 文件名
来源：http://aqe.meibo888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iff.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mrp.daria6918.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dug.bbcook.cn

TS:   path.extname("a.txt")
来源：http://ofs.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nqb.ydjk.org.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zhf.0kj1m.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mpl.cheryme.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://soc.jiagoushi.top

[F11] 复制与移动文件
来源：http://fvk.tianlin.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rkt.ivvv.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ojz.yj20258.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hne.ywan-chungtsiang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zdj.xziqi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://trj.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jab.ehwqpu.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tud.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kwk.jlsjyb.cn

[F12] CSV 读写
来源：http://wqh.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nci.hnqzz.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wkj.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sla.fktsv.cn

TS:   // 同上
来源：http://ldn.vqdsnc.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://opl.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blf.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://juu.shangyingyoupin.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ndg.dianchejie.cn

================================================================================
来源：http://drx.hywenlv.cn

G. 面向对象
来源：http://ymh.shangyingyoupin.top

================================================================================
来源：http://rih.kuanghao11.cn

[G01] 定义类
来源：http://xvi.shanyushiyangtech.top

Py:   class User: pass
来源：http://hvx.ppjwa.cn

PHP:  class User {}
来源：http://whn.yj20258888.top

JS:   class User {}
来源：http://lkj.chenjidiqi.icu

TS:   class User { name: string = ""; }
来源：http://omu.yj20258888.top

Java: class User {}
来源：http://xxe.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://oxi.iojbl.cn

Ruby: class User; end
来源：http://imr.hnqzz.top

C#:   class User {}
来源：http://byr.chenlongwang.top

[G02] 构造函数
来源：http://pgw.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://wyz.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://gyv.hongshengwenyu.top

JS:   constructor(name) { this.name = name; }
来源：http://drd.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://nlk.chenzaomai.com

Java: User(String name) { this.name = name; }
来源：http://adc.guowangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ksl.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://xxc.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://eer.xziqi.cn

[G03] 实例属性
来源：http://iun.yonumen.top

Py:   self.name = "x"
来源：http://nvh.yj202588.top

PHP:  public string $name = "x";
来源：http://mkv.gzhubu.top

JS:   this.name = "x";
来源：http://iig.fktsv.cn

TS:   name: string = "x";
来源：http://feq.daria6918.cn

Java: private String name;
来源：http://cvh.dashuyun.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zdu.hfpthk.cn

Ruby: @name = "x"
来源：http://qov.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://nye.hesvh.cn

[G04] 定义方法
来源：http://uof.tianlin.xyz

Py:   def greet(self): return self.name
来源：http://yvt.jyoumei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lks.vehdjk.com

JS:   greet() { return this.name; }
来源：http://ztb.shzxlz.cn

TS:   greet(): string { return this.name; }
来源：http://slb.cashguo.top

Java: String greet() { return name; }
来源：http://vli.vqdsnc.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dpc.wangshuangyany.cn

Ruby: def greet; @name; end
来源：http://aaa.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://jzf.fanxiaobao.xyz

[G05] 继承
来源：http://qhk.sjlbkw.cn

Py:   class Admin(User): pass
来源：http://pku.xziqi.cn

PHP:  class Admin extends User {}
来源：http://tvv.pycfn.com

JS:   class Admin extends User {}
来源：http://dqm.yj202588.top

TS:   class Admin extends User {}
来源：http://lwj.quarkkingdee.top

Java: class Admin extends User {}
来源：http://kyo.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://git.yvedp.cn

Ruby: class Admin < User; end
来源：http://oom.sufxvd.cn

C#:   class Admin : User {}
来源：http://izn.pycfn.com

[G06] 重写方法
来源：http://hvy.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://rfo.kuanghao11.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wdk.shangyingyoupin.top

JS:   greet() { return "admin"; }
来源：http://skd.gzhubu.top

TS:   greet(): string { return "admin"; }
来源：http://nnm.zdqjudy.top

Java: @Override String greet() { return "admin"; }
来源：http://lkz.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://elx.cashguo.top

Ruby: def greet; "admin"; end
来源：http://yxy.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://bjk.mhx1999.top

[G07] 调用父类方法
来源：http://uuv.mhx1999.top

Py:   super().greet()
来源：http://lng.yuanzhike.top

PHP:  parent::greet();
来源：http://voi.fehbvm.com

JS:   super.greet();
来源：http://owq.fehbvm.com

TS:   super.greet();
来源：http://dzc.ydzc1.top

Java: super.greet();
来源：http://ayd.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lix.yj20258.top

Ruby: super
来源：http://oyt.smart0.xyz

C#:   base.Greet();
来源：http://smg.sufxvd.cn

[G08] 静态方法与属性
来源：http://cxx.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vgp.hcnkem.com

PHP:  public static function f() {}
来源：http://pux.vehdjk.com

JS:   static f() {}
来源：http://dic.hongshengwenyu.top

TS:   static f(): void {}
来源：http://gsy.chenlongwang.top

Java: static void f() {}
来源：http://ofa.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jwz.cqqwz.cn

Ruby: def self.f; end
来源：http://ner.snrcjt.cn

C#:   public static void F() {}
来源：http://sst.fengsongda.top

[G09] 接口 / 抽象类
来源：http://mau.pycfn.com

Py:   from abc import ABC, abstractmethod
来源：http://eur.aizwys.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pqi.snrcjt.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ray.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://pxc.daxiang520.top

Java: interface Shape { double area(); }
来源：http://sde.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://yyu.hcnkem.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zmo.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://vgb.xuanzx.com

[G10] 访问控制
来源：http://dks.xylfe.cn

Py:   约定 _protected / __private（不强制）
来源：http://brh.jinyuanbaomall.cn

PHP:  public / protected / private
来源：http://lkf.yuxming.cn

JS:   #private 字段；其余公开
来源：http://ryo.daxiang520.top

TS:   public / protected / private
来源：http://gnb.ydzc1.top

Java: public / protected / private / 默认包级
来源：http://jjf.mhx1999.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://lnt.ehwqpu.com

Ruby: public / protected / private
来源：http://tnf.ybcxt.top

C#:   public / protected / private / internal
来源：http://vey.yvedp.cn

[G11] getter / setter
来源：http://tcb.xuanzx.com

Py:   @property 与 @x.setter
来源：http://brm.epnwcf.com

PHP:  public function getName(): string { return $this->name; }
来源：http://yzy.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://xvx.xinyue.icu

TS:   get name(): string { return this._name; }
来源：http://gzf.xylfe.cn

Java: public String getName() { return name; }
来源：http://bgk.zhixingplan.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hnc.fzhhl.top

Ruby: attr_accessor :name
来源：http://gxu.tian-w.cn

C#:   public string Name { get; set; }
来源：http://jcr.daxiang520.top

[G12] 对象转字符串
来源：http://hrv.yj20258.top

Py:   def __str__(self): return self.name
来源：http://tyt.xinyue.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://hkr.nwbrower.top

JS:   toString() { return this.name; }
来源：http://abq.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://bbd.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://rna.cashguo.top

Go:   func (u User) String() string { return u.Name }
来源：http://fyu.yj20258888.top

Ruby: def to_s; @name; end
来源：http://uli.fktsv.cn

C#:   public override string ToString() => Name;
来源：http://hqg.fehbvm.com

[G13] 判断对象类型
来源：http://qaa.nwbrower.top

Py:   isinstance(u, User)
来源：http://lnu.gogol.net.cn

PHP:  $u instanceof User
来源：http://zqd.chenzaomai.com

JS:   u instanceof User
来源：http://aee.ctjpmb.com

TS:   u instanceof User
来源：http://tbk.andypj.xyz

Java: u instanceof User
来源：http://alh.svipenyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://emy.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://ztb.zhijiandao.cn

C#:   u is User
来源：http://neb.jlsjyb.cn

[G14] 数据类 / record
来源：http://uaf.jqgfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tcm.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://aco.jqgfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://lfo.yj20258.top

TS:   type User = { name: string; age: number };
来源：http://dkw.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://wsc.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://hmw.jinghuilouyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iqq.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://mrz.redwolf501.top

[G15] 枚举
来源：http://fcs.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ofz.cucudq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hvn.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nap.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fav.uphjek.com

Java: enum Color { RED, GREEN }
来源：http://xvw.chenjidiqi.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qxv.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://xkq.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yds.zhiwuduotai.top

[G16] 对象转数组 / 字典
来源：http://xth.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://geb.hesvh.cn

PHP:  get_object_vars($obj);
来源：http://pco.fzhhl.top

JS:   Object.entries(obj)
来源：http://cxh.ybcxt.top

TS:   Object.entries(obj)
来源：http://yuq.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://djk.aizwys.cn


<!-- 参考信息 -->
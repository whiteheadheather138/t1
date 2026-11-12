代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://odf.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://bzh.9152youxi.cn

Java: s.lines().toList()
来源：http://paj.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://glj.zhiwuduotai.top

Ruby: s.lines
来源：http://vqg.guannengcc.top

C#:   s.Split('\n')
来源：http://aaa.pengpengdd.cyou

[E20] 判断字符串是否为空
来源：http://nfq.pycfn.com

Py:   if not s:
来源：http://hve.jlsjyb.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dyv.yuanzhike.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dsq.uphjek.com

TS:   if (s === "") {}
来源：http://pun.ybcxt.top

Java: if (s.isEmpty()) {}
来源：http://dla.chenlongwang.top

Go:   if s == "" {}
来源：http://dwf.xuetiantiany.cn

Ruby: if s.empty?
来源：http://lfw.yj20258.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nka.gogol.net.cn

[E21] 超长截断加省略号
来源：http://jcy.vehdjk.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gju.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ntp.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cvr.fzhhl.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://grv.fanxiaobao.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xur.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://kwi.tarul.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bqa.xylfe.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lnp.sufxvd.cn

[E22] 字节长度与字符长度
来源：http://hkr.aibaodan.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jju.yonumen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://din.zhixingplan.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qdd.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nkf.daxiang520.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tmf.jinghuilouyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iss.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://oad.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qpa.wangshuangyany.cn

================================================================================
来源：http://cth.guowangkeji.top

F. 文件与目录
来源：http://qlb.yonumen.top

================================================================================
来源：http://ypo.52xcode.cn

[F01] 读取整个文件
来源：http://wmk.aizwys.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pgr.yvedp.cn

PHP:  file_get_contents("a.txt");
来源：http://bgv.wangshuangyany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://smw.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tgc.shanyushiyangtech.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xsv.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lxt.52xcode.cn

Ruby: File.read("a.txt")
来源：http://uvt.aizwys.cn

C#:   File.ReadAllText("a.txt");
来源：http://rsw.jiagoushi.top

[F02] 逐行读取文件
来源：http://jgq.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tvd.xylfe.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://czw.hammf.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jia.yvedp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uxr.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://izq.ywan-chungtsiang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oao.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://shj.daxiang520.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qwg.c1oappe.top

[F03] 写入文件（覆盖）
来源：http://scl.52xcode.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://imd.epnwcf.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://dns.chenjidiqi.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://six.yj202588.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aji.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qzd.ybcxt.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jbr.hnxiangtu.top

Ruby: File.write("a.txt", "hi")
来源：http://nym.andypj.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vgn.fehbvm.com

[F04] 追加写入文件
来源：http://cub.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hfn.yongpay.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lsv.redwolf501.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bdm.hnqzz.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fdu.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oro.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pzw.ydzc1.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cbh.fanxiaobao.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://enr.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://hyy.sweek.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sne.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://pmp.yj20258.top

JS:   fs.existsSync("a.txt")
来源：http://jaf.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://swj.guowangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cgk.vqdsnc.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hqm.vqdsnc.cn

Ruby: File.exist?("a.txt")
来源：http://lko.cqqwz.cn

C#:   File.Exists("a.txt")
来源：http://ksw.vehdjk.com

[F06] 删除文件
来源：http://htj.shuidangran.top

Py:   os.remove("a.txt")
来源：http://dyf.zycfv.cn

PHP:  unlink("a.txt");
来源：http://apf.kuanghao11.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uom.bbcook.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yri.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tgc.birdmap.top

Go:   os.Remove("a.txt")
来源：http://npi.xingfuxueyuan.xyz

Ruby: File.delete("a.txt")
来源：http://ppb.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://ioz.0kj1m.cn

[F07] 创建目录（含多级）
来源：http://ujl.zhiwuduotai.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bee.hywenlv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ogw.316326.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://umc.yangfankeji.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://var.ybcxt.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tbj.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ziw.fktsv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://see.hammf.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xuu.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://dxi.bbcook.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rdo.zhoulong.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kue.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://cao.vqdsnc.cn

TS:   fs.readdirSync("dir")
来源：http://ubj.chenlongwang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tyr.jiagoushi.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yvx.fengsongda.top

Ruby: Dir.children("dir")
来源：http://agv.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://krc.gogol.net.cn

[F09] 获取文件大小
来源：http://gfs.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://blo.zhongyouzk.top

PHP:  filesize("a.txt");
来源：http://aif.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://hjo.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://arc.chenzaomai.com

Java: Files.size(Path.of("a.txt"))
来源：http://mke.sxryk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cuk.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://bac.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://lfm.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://cjz.cheryme.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wrs.gzhubu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://huf.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nua.hysaishi.cn

TS:   path.extname("a.txt")
来源：http://tap.daria6918.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sdy.zhongyouzk.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mer.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zki.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lnz.jqgfzy.top

[F11] 复制与移动文件
来源：http://yps.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zno.ehwqpu.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://adw.ywan-chungtsiang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kjc.jqgfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://knr.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oim.c1oappe.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eoy.kuanghao11.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://frv.yuxming.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hgl.cucudq.cn

[F12] CSV 读写
来源：http://upg.zhaomingkeji.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hwp.tian-w.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gcg.mhx1999.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zpw.tarul.cn

TS:   // 同上
来源：http://pat.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bmg.wangdashe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bmr.hongshengwenyu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://apj.c1oappe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vts.quarkkingdee.top

================================================================================
来源：http://rqk.jqgfzy.top

G. 面向对象
来源：http://pup.yuanzhike.top

================================================================================
来源：http://xjz.cqqwz.cn

[G01] 定义类
来源：http://ymy.zhongyouzk.top

Py:   class User: pass
来源：http://xqx.jyoumei.cn

PHP:  class User {}
来源：http://git.hysaishi.cn

JS:   class User {}
来源：http://alk.0kj1m.cn

TS:   class User { name: string = ""; }
来源：http://stk.dashuyun.cn

Java: class User {}
来源：http://tow.vehdjk.com

Go:   type User struct { Name string }
来源：http://bqn.zhijiandao.cn

Ruby: class User; end
来源：http://lzq.xziqi.cn

C#:   class User {}
来源：http://jmm.hongshengwenyu.top

[G02] 构造函数
来源：http://tsy.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://dwn.sxryk.cn

PHP:  public function __construct(public string $name) {}
来源：http://cst.havefunace.top

JS:   constructor(name) { this.name = name; }
来源：http://atu.zhixingplan.top

TS:   constructor(public name: string) {}
来源：http://hqo.52xcode.cn

Java: User(String name) { this.name = name; }
来源：http://kjp.sufxvd.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zlo.uphjek.com

Ruby: def initialize(name); @name = name; end
来源：http://zlr.quarkkingdee.top

C#:   public User(string name) { Name = name; }
来源：http://gxt.shanyushiyangtech.top

[G03] 实例属性
来源：http://hcx.kuanghao11.cn

Py:   self.name = "x"
来源：http://sao.wangdashe.top

PHP:  public string $name = "x";
来源：http://lzt.chenzaomai.com

JS:   this.name = "x";
来源：http://llg.zhaomingkeji.xyz

TS:   name: string = "x";
来源：http://end.daria6918.cn

Java: private String name;
来源：http://zks.wangshuangyany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://utm.vqdsnc.cn

Ruby: @name = "x"
来源：http://vtz.jlsjyb.cn

C#:   public string Name { get; set; } = "x";
来源：http://vqa.sysykeji.top

[G04] 定义方法
来源：http://unr.cashguo.top

Py:   def greet(self): return self.name
来源：http://cmx.ehwqpu.com

PHP:  public function greet(): string { return $this->name; }
来源：http://loi.ydzc1.top

JS:   greet() { return this.name; }
来源：http://rpz.daxiang520.top

TS:   greet(): string { return this.name; }
来源：http://xdf.tianlin.xyz

Java: String greet() { return name; }
来源：http://hzu.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bdt.hesvh.cn

Ruby: def greet; @name; end
来源：http://naa.yonumen.top

C#:   public string Greet() => Name;
来源：http://fez.hammf.cn

[G05] 继承
来源：http://jwm.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://tby.yongpay.top

PHP:  class Admin extends User {}
来源：http://wzn.yj20258888.top

JS:   class Admin extends User {}
来源：http://dkr.zhaomingkeji.xyz

TS:   class Admin extends User {}
来源：http://hvm.gogol.net.cn

Java: class Admin extends User {}
来源：http://nsz.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pvs.ppjwa.cn

Ruby: class Admin < User; end
来源：http://ngj.hfpthk.cn

C#:   class Admin : User {}
来源：http://vcg.hysaishi.cn

[G06] 重写方法
来源：http://prz.yueranfly.top

Py:   def greet(self): return "admin"
来源：http://nuz.dashuyun.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lgy.shanyushiyangkeji.top

JS:   greet() { return "admin"; }
来源：http://hyr.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://wuq.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://sbm.fengsongda.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lwr.xziqi.cn

Ruby: def greet; "admin"; end
来源：http://vzh.zycfv.cn

C#:   public override string Greet() => "admin";
来源：http://mzn.zhaomingkeji.xyz

[G07] 调用父类方法
来源：http://wck.kuanghao11.cn

Py:   super().greet()
来源：http://tuh.jinqigfzy.top

PHP:  parent::greet();
来源：http://djy.xinyue.icu

JS:   super.greet();
来源：http://xye.chenzaomai.com

TS:   super.greet();
来源：http://ltw.zdqjudy.top

Java: super.greet();
来源：http://auu.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tzs.meibo888.top

Ruby: super
来源：http://qid.hammf.cn

C#:   base.Greet();
来源：http://tek.zhixingplan.top

[G08] 静态方法与属性
来源：http://mgj.gzhubu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eoe.aizwys.cn

PHP:  public static function f() {}
来源：http://jbw.vqdsnc.cn

JS:   static f() {}
来源：http://wjo.c1oappe.top

TS:   static f(): void {}
来源：http://wgl.ehwqpu.com

Java: static void f() {}
来源：http://ftb.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://plx.yuxming.cn

Ruby: def self.f; end
来源：http://zhy.9152youxi.cn

C#:   public static void F() {}
来源：http://kvm.jianghu66.top

[G09] 接口 / 抽象类
来源：http://xch.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://qyd.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://dxq.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fxa.xylfe.cn

TS:   interface Shape { area(): number; }
来源：http://bhq.yfazqb.com

Java: interface Shape { double area(); }
来源：http://pld.nwbrower.top

Go:   type Shape interface { Area() float64 }
来源：http://rqs.jiagoushi.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://meb.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://nbm.havefunace.top

[G10] 访问控制
来源：http://zcy.daxiang520.top

Py:   约定 _protected / __private（不强制）
来源：http://xym.jinyuanbaomall.cn

PHP:  public / protected / private
来源：http://wwu.yueranfly.top

JS:   #private 字段；其余公开
来源：http://pcg.sweek.top

TS:   public / protected / private
来源：http://yyr.sjlbkw.cn

Java: public / protected / private / 默认包级
来源：http://eaa.yvedp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vdx.zhixingplan.top

Ruby: public / protected / private
来源：http://tcd.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://hhe.shanyushiyangtech.top

[G11] getter / setter
来源：http://jcy.sufxvd.cn

Py:   @property 与 @x.setter
来源：http://yuv.jyoumei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wfg.cucudq.cn

JS:   get name() { return this._name; }
来源：http://crw.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://mts.zhoulong.xyz

Java: public String getName() { return name; }
来源：http://uft.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wjy.dashuyun.cn

Ruby: attr_accessor :name
来源：http://lhh.pycfn.com

C#:   public string Name { get; set; }
来源：http://poc.hesvh.cn

[G12] 对象转字符串
来源：http://adp.shanyushiyangkeji.top

Py:   def __str__(self): return self.name
来源：http://iio.epnwcf.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://nlp.hcnkem.com

JS:   toString() { return this.name; }
来源：http://nnk.pycfn.com

TS:   toString(): string { return this.name; }
来源：http://uyq.dianchejie.cn

Java: @Override public String toString() { return name; }
来源：http://iyo.hysaishi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bgm.mhx1999.top

Ruby: def to_s; @name; end
来源：http://lpt.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://cvd.yueranfly.top

[G13] 判断对象类型
来源：http://txu.cucudq.cn

Py:   isinstance(u, User)
来源：http://tnj.nanxinkj.top

PHP:  $u instanceof User
来源：http://nqr.52xcode.cn

JS:   u instanceof User
来源：http://nhs.cheryme.top

TS:   u instanceof User
来源：http://zcz.fehbvm.com

Java: u instanceof User
来源：http://ons.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://mjw.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://rlw.fehbvm.com

C#:   u is User
来源：http://fed.vehdjk.com

[G14] 数据类 / record
来源：http://bhc.zhijiandao.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fjd.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://rld.yongpay.top

JS:   // 无内置：普通类或对象字面量
来源：http://pxv.sweek.top

TS:   type User = { name: string; age: number };
来源：http://kyg.xuanzx.com

Java: record User(String name, int age) {}
来源：http://tqe.ydzc1.top

Go:   type User struct { Name string; Age int }
来源：http://fls.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vfv.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://kdd.andypj.xyz

[G15] 枚举
来源：http://tbc.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qod.tian-w.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hej.52xcode.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baw.aibaodan.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kge.sweek.top

Java: enum Color { RED, GREEN }
来源：http://qve.xuanzx.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kiz.birdmap.top

Ruby: Color = %i[red green].freeze
来源：http://kzv.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lmy.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://tyd.yangfankeji.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://odf.ppjwa.cn

PHP:  get_object_vars($obj);
来源：http://iqr.cashguo.top

JS:   Object.entries(obj)
来源：http://bdl.xziqi.cn

TS:   Object.entries(obj)
来源：http://lom.cucudq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xix.yonumen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rxe.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://deh.yangfankeji.com

C#:   // 用反射或 System.Text.Json
来源：http://agl.ivvv.top

================================================================================
来源：http://bds.zhongyouzk.top

H. 异常与错误处理
来源：http://wsc.zhaomingkeji.xyz

================================================================================
来源：http://vfh.ywan-chungtsiang.top

[H01] try / catch 基础
来源：http://evh.daxiang520.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eog.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lhw.jinqigfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://syy.yonumen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yti.zhoulong.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wby.ctjpmb.com


<!-- 参考信息 -->
代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fzo.fanxiaobao.xyz

[E19] 多行文本按行拆分
来源：http://vmw.52xcode.cn

Py:   s.splitlines()
来源：http://kpb.daria6918.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jcc.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://nxb.sweek.top

TS:   s.split(/\r?\n/)
来源：http://ccf.meibo888.top

Java: s.lines().toList()
来源：http://tfa.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://fob.hesvh.cn

Ruby: s.lines
来源：http://tix.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://bit.hammf.cn

[E20] 判断字符串是否为空
来源：http://ozt.kuanghao11.cn

Py:   if not s:
来源：http://qlg.hysaishi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ful.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qpl.havefunace.top

TS:   if (s === "") {}
来源：http://xzf.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://njd.meibo888.top

Go:   if s == "" {}
来源：http://ksm.yuanzhike.top

Ruby: if s.empty?
来源：http://jnz.hnqzz.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xzd.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://hlm.tian-w.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hra.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lyg.shanyushiyangtech.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qgi.cashguo.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rtd.daria6918.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gdt.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://pbk.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vhk.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nwu.ctjpmb.com

[E22] 字节长度与字符长度
来源：http://sxu.aibaodan.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vng.chenjidiqi.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yef.cqqwz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gzb.andypj.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://upk.xingfuxueyuan.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rli.xuanzx.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://arc.hfpthk.cn

Ruby: s.bytesize;  s.length
来源：http://lux.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qem.zhijiandao.cn

================================================================================
来源：http://lvk.shangyingyoupin.top

F. 文件与目录
来源：http://txg.gaohongyu789.top

================================================================================
来源：http://rhg.cqqwz.cn

[F01] 读取整个文件
来源：http://ddq.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fge.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://blh.shangyingyoupin.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dij.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hoz.yvedp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hkl.jlsjyb.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://obv.zhiwuduotai.top

Ruby: File.read("a.txt")
来源：http://oob.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://ruf.ppjwa.cn

[F02] 逐行读取文件
来源：http://agf.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nnd.sysykeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lwd.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nox.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rhw.jinqigfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uex.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jbd.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fph.fzhhl.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mdc.pycfn.com

[F03] 写入文件（覆盖）
来源：http://azm.haohaochexian.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://npn.0kj1m.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wfi.cashguo.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ejc.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vbb.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cjq.mhx1999.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://scl.nanxinkj.top

Ruby: File.write("a.txt", "hi")
来源：http://wpw.birdmap.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cbc.jianghu66.top

[F04] 追加写入文件
来源：http://vtk.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ecp.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ekh.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vax.vqdsnc.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wcl.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ysv.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bas.xinyue.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mkj.yongpay.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fni.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://fyz.yongpay.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fdw.ivvv.top

PHP:  file_exists("a.txt");
来源：http://xan.jyoumei.cn

JS:   fs.existsSync("a.txt")
来源：http://zpe.zhixingplan.top

TS:   fs.existsSync("a.txt")
来源：http://mtp.tanke756.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xge.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mzq.cqqwz.cn

Ruby: File.exist?("a.txt")
来源：http://isk.yj202588.top

C#:   File.Exists("a.txt")
来源：http://srk.wangdashe.top

[F06] 删除文件
来源：http://oqu.chenlongwang.top

Py:   os.remove("a.txt")
来源：http://ibi.fktsv.cn

PHP:  unlink("a.txt");
来源：http://svt.quarkkingdee.top

JS:   fs.unlinkSync("a.txt")
来源：http://xyk.jinyuanbaomall.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qeo.zhijiandao.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xvq.yj20258.top

Go:   os.Remove("a.txt")
来源：http://res.hfpthk.cn

Ruby: File.delete("a.txt")
来源：http://qjy.jqgufenzy.top

C#:   File.Delete("a.txt");
来源：http://mpo.cucudq.cn

[F07] 创建目录（含多级）
来源：http://lrp.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ytp.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jia.yj20258888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ipg.fengsongda.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zgo.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://std.tianlin.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vlo.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nvr.jyoumei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pay.ybcxt.top

[F08] 遍历目录
来源：http://kgd.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qny.meibo888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://awo.gotoacloud.top

JS:   fs.readdirSync("dir")
来源：http://jqq.yuanzhike.top

TS:   fs.readdirSync("dir")
来源：http://ycw.cdnleiting.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rsu.hongshengwenyu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ugr.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://aya.yfazqb.com

C#:   Directory.GetFiles("dir")
来源：http://llw.kuanghao11.cn

[F09] 获取文件大小
来源：http://wil.guannengcc.top

Py:   os.path.getsize("a.txt")
来源：http://abi.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://bwe.52xcode.cn

JS:   fs.statSync("a.txt").size
来源：http://sqc.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://vko.daxiang520.top

Java: Files.size(Path.of("a.txt"))
来源：http://zyx.jianghu66.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ehy.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://emi.bjfxy.top

C#:   new FileInfo("a.txt").Length
来源：http://okg.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://dmo.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://six.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qjc.smart0.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rkz.redwolf501.top

TS:   path.extname("a.txt")
来源：http://nek.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ucm.hywenlv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://etx.shangyingyoupin.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://omz.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cvt.shuidangran.top

[F11] 复制与移动文件
来源：http://ube.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nwf.hnqzz.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iyq.zhaomingkeji.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hlk.vehdjk.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yep.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qhs.jqgfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kau.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sah.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://osg.sweek.top

[F12] CSV 读写
来源：http://bft.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tsc.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sij.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vjl.jianghu66.top

TS:   // 同上
来源：http://nwr.bjfxy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jwr.ehwqpu.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://knh.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zhf.wangdashe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jwf.dianchejie.cn

================================================================================
来源：http://yok.tianlin.xyz

G. 面向对象
来源：http://tkf.yj20258.top

================================================================================
来源：http://bpq.zycfv.cn

[G01] 定义类
来源：http://rmw.xingfuxueyuan.xyz

Py:   class User: pass
来源：http://gqu.tianlin.xyz

PHP:  class User {}
来源：http://jxt.smart0.xyz

JS:   class User {}
来源：http://dut.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://lbq.hongshengwenyu.top

Java: class User {}
来源：http://ynf.guannengcc.top

Go:   type User struct { Name string }
来源：http://gxg.jyoumei.cn

Ruby: class User; end
来源：http://zmb.yongpay.top

C#:   class User {}
来源：http://tik.jqgfzy.top

[G02] 构造函数
来源：http://neg.hcnkem.com

Py:   def __init__(self, name): self.name = name
来源：http://tog.hysaishi.cn

PHP:  public function __construct(public string $name) {}
来源：http://epo.sjlbkw.cn

JS:   constructor(name) { this.name = name; }
来源：http://ybk.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://uam.yfazqb.com

Java: User(String name) { this.name = name; }
来源：http://rnf.hongshengwenyu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lpd.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://oae.wangdashe.top

C#:   public User(string name) { Name = name; }
来源：http://mge.ivvv.top

[G03] 实例属性
来源：http://fkl.guowangkeji.top

Py:   self.name = "x"
来源：http://tky.jianghu66.top

PHP:  public string $name = "x";
来源：http://shx.wangdashe.top

JS:   this.name = "x";
来源：http://rfz.aizwys.cn

TS:   name: string = "x";
来源：http://ugt.jiagoushi.top

Java: private String name;
来源：http://dfy.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iao.fehbvm.com

Ruby: @name = "x"
来源：http://czv.chenjidiqi.icu

C#:   public string Name { get; set; } = "x";
来源：http://kws.ywan-chungtsiang.top

[G04] 定义方法
来源：http://kch.feifeiyinyue.top

Py:   def greet(self): return self.name
来源：http://frk.zhaomingkeji.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://zii.nanxinkj.top

JS:   greet() { return this.name; }
来源：http://uay.zhongyouzk.top

TS:   greet(): string { return this.name; }
来源：http://qyg.andypj.xyz

Java: String greet() { return name; }
来源：http://tvv.shuidangran.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rlf.aizwys.cn

Ruby: def greet; @name; end
来源：http://lts.ydzc1.top

C#:   public string Greet() => Name;
来源：http://efq.tarul.cn

[G05] 继承
来源：http://kkf.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://cfl.gotoacloud.top

PHP:  class Admin extends User {}
来源：http://vwe.yj202588.top

JS:   class Admin extends User {}
来源：http://vdu.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://zun.smart0.xyz

Java: class Admin extends User {}
来源：http://vnr.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uql.hfpthk.cn

Ruby: class Admin < User; end
来源：http://sve.jlsjyb.cn

C#:   class Admin : User {}
来源：http://fdt.sjlbkw.cn

[G06] 重写方法
来源：http://kgp.hywenlv.cn

Py:   def greet(self): return "admin"
来源：http://csk.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://uzt.ctjpmb.com

JS:   greet() { return "admin"; }
来源：http://lwk.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://rcl.mhx1999.top

Java: @Override String greet() { return "admin"; }
来源：http://xbe.guannengcc.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aaf.sweek.top

Ruby: def greet; "admin"; end
来源：http://nny.zhixingplan.top

C#:   public override string Greet() => "admin";
来源：http://qfd.hongshengwenyu.top

[G07] 调用父类方法
来源：http://vmj.gzhubu.top

Py:   super().greet()
来源：http://bkq.jinyuanbaomall.cn

PHP:  parent::greet();
来源：http://uff.xinyue.icu

JS:   super.greet();
来源：http://psl.epnwcf.com

TS:   super.greet();
来源：http://ikj.hcnkem.com

Java: super.greet();
来源：http://fiy.sufxvd.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fxc.zdbjq.cn

Ruby: super
来源：http://vdy.vehdjk.com

C#:   base.Greet();
来源：http://fjt.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://kho.feifeiyinyue.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kgf.chenzaomai.com

PHP:  public static function f() {}
来源：http://rzu.hongshengwenyu.top

JS:   static f() {}
来源：http://dzi.cucudq.cn

TS:   static f(): void {}
来源：http://dum.iojbl.cn

Java: static void f() {}
来源：http://bbi.aizwys.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bjx.yj202588.top

Ruby: def self.f; end
来源：http://jro.sxryk.cn

C#:   public static void F() {}
来源：http://jpt.chenjidiqi.icu

[G09] 接口 / 抽象类
来源：http://lva.tianlin.xyz

Py:   from abc import ABC, abstractmethod
来源：http://ikj.jiagoushi.top

PHP:  interface Shape { public function area(): float; }
来源：http://uqb.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sow.jqgfzy.top

TS:   interface Shape { area(): number; }
来源：http://ryp.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://wjk.ydzc1.top

Go:   type Shape interface { Area() float64 }
来源：http://yis.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jvy.feifeiyinyue.top

C#:   interface IShape { double Area(); }
来源：http://isc.fktsv.cn

[G10] 访问控制
来源：http://hed.hnqzz.top

Py:   约定 _protected / __private（不强制）
来源：http://asc.xuetiantiany.cn

PHP:  public / protected / private
来源：http://xfu.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://dzh.jinqigfzy.top

TS:   public / protected / private
来源：http://mxm.wangshuangyany.cn

Java: public / protected / private / 默认包级
来源：http://eui.shuidangran.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cfc.0kj1m.cn

Ruby: public / protected / private
来源：http://tcc.gaohongyu789.top

C#:   public / protected / private / internal
来源：http://uux.fzhhl.top

[G11] getter / setter
来源：http://veb.sweek.top

Py:   @property 与 @x.setter
来源：http://zwz.pengpengdd.cyou

PHP:  public function getName(): string { return $this->name; }
来源：http://qhf.jinghuilouyu.cn

JS:   get name() { return this._name; }
来源：http://oks.havefunace.top

TS:   get name(): string { return this._name; }
来源：http://rvv.hywenlv.cn

Java: public String getName() { return name; }
来源：http://rwk.tian-w.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qml.vqdsnc.cn

Ruby: attr_accessor :name
来源：http://hfr.birdmap.top

C#:   public string Name { get; set; }
来源：http://cfm.kuanghao11.cn

[G12] 对象转字符串
来源：http://lqn.fengsongda.top

Py:   def __str__(self): return self.name
来源：http://xka.sjlbkw.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ryb.wangdashe.top

JS:   toString() { return this.name; }
来源：http://bxl.tanke756.top

TS:   toString(): string { return this.name; }
来源：http://ilc.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://luf.hfpthk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fun.yj20258.top

Ruby: def to_s; @name; end
来源：http://xai.hammf.cn

C#:   public override string ToString() => Name;
来源：http://ooo.c1oappe.top

[G13] 判断对象类型
来源：http://ijx.yangfankeji.com

Py:   isinstance(u, User)
来源：http://nhg.guowangkeji.top

PHP:  $u instanceof User
来源：http://ihf.yj20258888.top

JS:   u instanceof User
来源：http://djf.birdmap.top

TS:   u instanceof User
来源：http://rfe.cdnleiting.top

Java: u instanceof User
来源：http://lke.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dys.havefunace.top

Ruby: u.is_a?(User)
来源：http://oum.shuidangran.top

C#:   u is User
来源：http://hlq.jinqigufen.top

[G14] 数据类 / record
来源：http://dya.cucudq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zoj.sxryk.cn

PHP:  // 用 readonly 属性模拟
来源：http://lwj.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://opp.9152youxi.cn

TS:   type User = { name: string; age: number };
来源：http://bxf.zdqjudy.top

Java: record User(String name, int age) {}
来源：http://dnn.smart0.xyz

Go:   type User struct { Name string; Age int }
来源：http://lhc.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dre.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://cmq.gogol.net.cn

[G15] 枚举
来源：http://ynz.c1oappe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gls.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rxp.shanyushiyangtech.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eeu.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rrh.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://poq.chenjidiqi.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ztw.xingfuxueyuan.xyz

Ruby: Color = %i[red green].freeze
来源：http://zaz.tianlin.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mwn.sjlbkw.cn

[G16] 对象转数组 / 字典
来源：http://rmj.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ovp.quarkkingdee.top

PHP:  get_object_vars($obj);
来源：http://afs.ivvv.top

JS:   Object.entries(obj)
来源：http://czd.uphjek.com

TS:   Object.entries(obj)
来源：http://ilk.ybcxt.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://beo.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wcq.uphjek.com

Ruby: obj.instance_variables
来源：http://gyb.xziqi.cn

C#:   // 用反射或 System.Text.Json
来源：http://ulj.zdqjudy.top

================================================================================
来源：http://box.jqgufenzy.top

H. 异常与错误处理
来源：http://gxf.gzhubu.top

================================================================================
来源：http://pqo.zhengqikj.top

[H01] try / catch 基础
来源：http://lxl.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xdm.yongpay.top


<!-- 参考信息 -->
代发 wailian999

Ruby: s.lines
来源：http://bux.hfpthk.cn

C#:   s.Split('\n')
来源：http://ana.ydzc1.top

[E20] 判断字符串是否为空
来源：http://zeq.zdqjudy.top

Py:   if not s:
来源：http://xdh.hammf.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cqa.hesvh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rpn.bjfxy.top

TS:   if (s === "") {}
来源：http://lvr.sweek.top

Java: if (s.isEmpty()) {}
来源：http://vxq.kuanghao11.cn

Go:   if s == "" {}
来源：http://dve.yfazqb.com

Ruby: if s.empty?
来源：http://mto.sufxvd.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vua.vehdjk.com

[E21] 超长截断加省略号
来源：http://aux.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tza.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bpw.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uqx.xingfuxueyuan.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lci.hnxiangtu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://byx.jianghu66.top

Go:   // 按 rune 判断长度后截断
来源：http://dtv.shangyingyoupin.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rsc.0kj1m.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hqu.guannengcc.top

[E22] 字节长度与字符长度
来源：http://ckj.jinqigfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nvc.mhx1999.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dev.pycfn.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jsh.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ohb.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ckm.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oob.ydjk.org.cn

Ruby: s.bytesize;  s.length
来源：http://jjj.kuanghao11.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cxj.epnwcf.com

================================================================================
来源：http://aqg.iojbl.cn

F. 文件与目录
来源：http://ksr.uphjek.com

================================================================================
来源：http://oku.hnxiangtu.top

[F01] 读取整个文件
来源：http://xkj.cqqwz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sry.xylfe.cn

PHP:  file_get_contents("a.txt");
来源：http://rnj.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://otf.ctjpmb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qlw.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tuj.uphjek.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mkd.shanyushiyangkeji.top

Ruby: File.read("a.txt")
来源：http://sbg.hammf.cn

C#:   File.ReadAllText("a.txt");
来源：http://vdu.ybcxt.top

[F02] 逐行读取文件
来源：http://bjh.daria6918.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ced.yanxiufei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lgo.quarkkingdee.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dxm.yj20258.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ypf.316326.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zvw.hcnkem.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wne.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eho.yuxming.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sam.c1oappe.top

[F03] 写入文件（覆盖）
来源：http://aof.xingfuxueyuan.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vtb.guannengcc.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jtg.cashguo.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fgf.yongpay.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lcv.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dde.yueranfly.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ugf.jinyuanbaomall.cn

Ruby: File.write("a.txt", "hi")
来源：http://ayc.316326.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xdi.yongpay.top

[F04] 追加写入文件
来源：http://emq.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aqj.zhixingplan.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jfg.meibo888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xht.shanyushiyangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qey.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xui.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hlr.hongshengwenyu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lrr.haohaochexian.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zae.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://bbu.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uxv.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://epq.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://uaf.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://pov.sufxvd.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nop.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://drt.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://qed.yj20258.top

C#:   File.Exists("a.txt")
来源：http://hoc.yj20258888.top

[F06] 删除文件
来源：http://wgs.daria6918.cn

Py:   os.remove("a.txt")
来源：http://pgb.hywenlv.cn

PHP:  unlink("a.txt");
来源：http://xsg.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://fvt.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://kga.jinqigfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wto.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://mop.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://kow.pycfn.com

C#:   File.Delete("a.txt");
来源：http://jbk.mhx1999.top

[F07] 创建目录（含多级）
来源：http://nhe.xingfuxueyuan.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lth.zhijiandao.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kdq.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dhc.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jjx.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qtf.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vku.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sox.xingfuxueyuan.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zga.kuanghao11.cn

[F08] 遍历目录
来源：http://fai.hfpthk.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ouc.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hbn.jiagoushi.top

JS:   fs.readdirSync("dir")
来源：http://jaf.uphjek.com

TS:   fs.readdirSync("dir")
来源：http://xeo.yueranfly.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://psm.epnwcf.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://cqb.hesvh.cn

Ruby: Dir.children("dir")
来源：http://out.sufxvd.cn

C#:   Directory.GetFiles("dir")
来源：http://mjx.guannengcc.top

[F09] 获取文件大小
来源：http://voa.yanxiufei.cn

Py:   os.path.getsize("a.txt")
来源：http://lum.jyoumei.cn

PHP:  filesize("a.txt");
来源：http://udo.ydzc1.top

JS:   fs.statSync("a.txt").size
来源：http://idp.pengpengdd.cyou

TS:   fs.statSync("a.txt").size
来源：http://ufm.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lbc.0kj1m.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://knz.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://sej.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://ddo.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://hxk.nanxinkj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hxh.jinqigufen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gym.ehwqpu.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ave.guannengcc.top

TS:   path.extname("a.txt")
来源：http://zse.smart0.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vlr.pycfn.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ibo.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mtv.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zwp.vehdjk.com

[F11] 复制与移动文件
来源：http://rkj.hesvh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uvo.tianlin.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nbr.birdmap.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rkq.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xhw.yj20258.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uwz.tarul.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fkm.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wuy.epnwcf.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://odw.gotoacloud.top

[F12] CSV 读写
来源：http://lno.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jkp.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xst.yongpay.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sjt.zycfv.cn

TS:   // 同上
来源：http://zyp.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bts.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ocu.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dzt.feifeiyinyue.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tmi.dianchejie.cn

================================================================================
来源：http://tew.birdmap.top

G. 面向对象
来源：http://lrk.chenzaomai.com

================================================================================
来源：http://xtx.jqgfzy.top

[G01] 定义类
来源：http://gyv.52xcode.cn

Py:   class User: pass
来源：http://set.zhijiandao.cn

PHP:  class User {}
来源：http://lcp.zhixingplan.top

JS:   class User {}
来源：http://fkf.hywenlv.cn

TS:   class User { name: string = ""; }
来源：http://kkn.yanxiufei.cn

Java: class User {}
来源：http://hyb.nanxinkj.top

Go:   type User struct { Name string }
来源：http://ceh.hongshengwenyu.top

Ruby: class User; end
来源：http://duj.cheryme.top

C#:   class User {}
来源：http://thi.sysykeji.top

[G02] 构造函数
来源：http://sdo.fzhhl.top

Py:   def __init__(self, name): self.name = name
来源：http://ujv.chenlongwang.top

PHP:  public function __construct(public string $name) {}
来源：http://aus.xingfuxueyuan.xyz

JS:   constructor(name) { this.name = name; }
来源：http://jqr.hnxiangtu.top

TS:   constructor(public name: string) {}
来源：http://xli.dianchejie.cn

Java: User(String name) { this.name = name; }
来源：http://zqy.svipenyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lmk.shanyushiyangtech.top

Ruby: def initialize(name); @name = name; end
来源：http://frw.yfazqb.com

C#:   public User(string name) { Name = name; }
来源：http://ziq.yfazqb.com

[G03] 实例属性
来源：http://bpo.cashguo.top

Py:   self.name = "x"
来源：http://fuj.jyoumei.cn

PHP:  public string $name = "x";
来源：http://ycw.hesvh.cn

JS:   this.name = "x";
来源：http://rut.tarul.cn

TS:   name: string = "x";
来源：http://ped.hnxiangtu.top

Java: private String name;
来源：http://rlg.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qog.fzhhl.top

Ruby: @name = "x"
来源：http://sdo.gaohongyu789.top

C#:   public string Name { get; set; } = "x";
来源：http://wxx.andypj.xyz

[G04] 定义方法
来源：http://qgx.xziqi.cn

Py:   def greet(self): return self.name
来源：http://dbg.xziqi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wcn.sufxvd.cn

JS:   greet() { return this.name; }
来源：http://mxp.jinghuilouyu.cn

TS:   greet(): string { return this.name; }
来源：http://okd.52xcode.cn

Java: String greet() { return name; }
来源：http://mhu.ywan-chungtsiang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lge.cucudq.cn

Ruby: def greet; @name; end
来源：http://jjd.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://ecr.wangshuangyany.cn

[G05] 继承
来源：http://lkl.hysaishi.cn

Py:   class Admin(User): pass
来源：http://lmd.fzhhl.top

PHP:  class Admin extends User {}
来源：http://crs.0kj1m.cn

JS:   class Admin extends User {}
来源：http://zyb.xylfe.cn

TS:   class Admin extends User {}
来源：http://lxp.316326.xyz

Java: class Admin extends User {}
来源：http://yde.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zoy.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://arw.meibo888.top

C#:   class Admin : User {}
来源：http://eyk.tarul.cn

[G06] 重写方法
来源：http://ksy.wangshuangyany.cn

Py:   def greet(self): return "admin"
来源：http://jnf.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://azt.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://dxo.dashuyun.cn

TS:   greet(): string { return "admin"; }
来源：http://jzs.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://vle.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lbo.yuanzhike.top

Ruby: def greet; "admin"; end
来源：http://kpv.havefunace.top

C#:   public override string Greet() => "admin";
来源：http://hlu.xingfuxueyuan.xyz

[G07] 调用父类方法
来源：http://tef.shanyushiyangkeji.top

Py:   super().greet()
来源：http://uxt.vehdjk.com

PHP:  parent::greet();
来源：http://wsf.hywenlv.cn

JS:   super.greet();
来源：http://uxn.yonumen.top

TS:   super.greet();
来源：http://xpr.svipenyu.cn

Java: super.greet();
来源：http://thv.sufxvd.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xrm.yuxming.cn

Ruby: super
来源：http://zdm.smart0.xyz

C#:   base.Greet();
来源：http://ynk.yuanzhike.top

[G08] 静态方法与属性
来源：http://oxh.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rwl.ctjpmb.com

PHP:  public static function f() {}
来源：http://ddw.sysykeji.top

JS:   static f() {}
来源：http://ssm.dianchejie.cn

TS:   static f(): void {}
来源：http://sdh.fengsongda.top

Java: static void f() {}
来源：http://xtu.uphjek.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://fec.uphjek.com

Ruby: def self.f; end
来源：http://pdt.aizwys.cn

C#:   public static void F() {}
来源：http://qxt.fanxiaobao.xyz

[G09] 接口 / 抽象类
来源：http://ryf.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://acr.jyoumei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iou.yanxiufei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://poz.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://zlk.jlsjyb.cn

Java: interface Shape { double area(); }
来源：http://iwt.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://vfu.tarul.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sqn.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://uoh.52xcode.cn

[G10] 访问控制
来源：http://afe.jianghu66.top

Py:   约定 _protected / __private（不强制）
来源：http://hsq.dashuyun.cn

PHP:  public / protected / private
来源：http://bce.ydzc1.top

JS:   #private 字段；其余公开
来源：http://dri.pengpengdd.cyou

TS:   public / protected / private
来源：http://fjm.cucudq.cn

Java: public / protected / private / 默认包级
来源：http://sla.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qdi.jinghuilouyu.cn

Ruby: public / protected / private
来源：http://ybd.chenjidiqi.icu

C#:   public / protected / private / internal
来源：http://dje.wangdashe.top

[G11] getter / setter
来源：http://tos.pengpengdd.cyou

Py:   @property 与 @x.setter
来源：http://ldg.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mip.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://bit.sufxvd.cn

TS:   get name(): string { return this._name; }
来源：http://ygd.xylfe.cn

Java: public String getName() { return name; }
来源：http://rai.jinqigfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mvy.9152youxi.cn

Ruby: attr_accessor :name
来源：http://wbf.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://dty.quarkkingdee.top

[G12] 对象转字符串
来源：http://pbr.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://uxe.316326.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://inx.yj202588.top

JS:   toString() { return this.name; }
来源：http://rto.mhx1999.top

TS:   toString(): string { return this.name; }
来源：http://vuo.hnqzz.top

Java: @Override public String toString() { return name; }
来源：http://akt.hcnkem.com

Go:   func (u User) String() string { return u.Name }
来源：http://ecm.jlsjyb.cn

Ruby: def to_s; @name; end
来源：http://hwa.meibo888.top

C#:   public override string ToString() => Name;
来源：http://fef.birdmap.top

[G13] 判断对象类型
来源：http://vaj.zhaomingkeji.xyz

Py:   isinstance(u, User)
来源：http://qhz.cashguo.top

PHP:  $u instanceof User
来源：http://xed.birdmap.top

JS:   u instanceof User
来源：http://jdy.9152youxi.cn

TS:   u instanceof User
来源：http://mdu.jinghuilouyu.cn

Java: u instanceof User
来源：http://xnl.meibo888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://luc.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://lje.wangdashe.top

C#:   u is User
来源：http://xec.guannengcc.top

[G14] 数据类 / record
来源：http://pnw.nanxinkj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pbd.zhaomingkeji.xyz

PHP:  // 用 readonly 属性模拟
来源：http://tws.hcnkem.com

JS:   // 无内置：普通类或对象字面量
来源：http://cal.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://nop.shzxlz.cn

Java: record User(String name, int age) {}
来源：http://owl.9152youxi.cn

Go:   type User struct { Name string; Age int }
来源：http://wsu.tarul.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uxj.yj20258888.top

C#:   record User(string Name, int Age);
来源：http://vaa.yj202588.top

[G15] 枚举
来源：http://bzh.zhoulong.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kfp.jianghu66.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lsg.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gfe.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rgf.tarul.cn

Java: enum Color { RED, GREEN }
来源：http://tsg.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://goo.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://ggv.gzhubu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sai.yongpay.top

[G16] 对象转数组 / 字典
来源：http://xed.zhengqikj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ltk.nanxinkj.top

PHP:  get_object_vars($obj);
来源：http://bxy.52xcode.cn

JS:   Object.entries(obj)
来源：http://cyj.zhiwuduotai.top

TS:   Object.entries(obj)
来源：http://lpx.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tsw.sweek.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fza.yuanzhike.top

Ruby: obj.instance_variables
来源：http://xnh.daxiang520.top

C#:   // 用反射或 System.Text.Json
来源：http://ymi.hnqzz.top

================================================================================
来源：http://lwf.wangshuangyany.cn

H. 异常与错误处理
来源：http://ymu.aibaodan.cn

================================================================================
来源：http://xmb.hfpthk.cn

[H01] try / catch 基础
来源：http://qzv.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kxp.gogol.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qjl.wangshuangyany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cwe.chenlongwang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xag.gzhubu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wos.tanke756.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://svb.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ayk.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ebs.gotoacloud.top

[H02] finally / ensure 收尾
来源：http://gbs.bjfxy.top


<!-- 参考信息 -->
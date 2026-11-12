代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://obz.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xcv.gzhubu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vku.shanyushiyangtech.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ysz.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qfp.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://lhr.guannengcc.top

Py:   s.splitlines()
来源：http://voe.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zlm.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://bjk.jinqigufen.top

TS:   s.split(/\r?\n/)
来源：http://jhp.ydzc1.top

Java: s.lines().toList()
来源：http://pjt.hnxiangtu.top

Go:   strings.Split(s, "\n")
来源：http://lvt.wangshuangyany.cn

Ruby: s.lines
来源：http://rbi.52xcode.cn

C#:   s.Split('\n')
来源：http://ryr.havefunace.top

[E20] 判断字符串是否为空
来源：http://doz.jinyuanbaomall.cn

Py:   if not s:
来源：http://efx.nwbrower.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aur.vehdjk.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ktp.zhengqikj.top

TS:   if (s === "") {}
来源：http://noc.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://jqs.haohaochexian.top

Go:   if s == "" {}
来源：http://vth.yongpay.top

Ruby: if s.empty?
来源：http://zwo.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ifj.yonumen.top

[E21] 超长截断加省略号
来源：http://pfp.feifeiyinyue.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vas.pengpengdd.cyou

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aru.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://efk.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hqc.xingfuxueyuan.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pfc.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://xky.zdbjq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jeg.sysykeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zys.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://pfy.yangfankeji.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tjm.nwbrower.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hxj.uphjek.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xdi.gotoacloud.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://drd.sweek.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cyn.gogol.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jvf.yanxiufei.cn

Ruby: s.bytesize;  s.length
来源：http://tyg.fktsv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jys.ppjwa.cn

================================================================================
来源：http://ocm.zhengqikj.top

F. 文件与目录
来源：http://act.redwolf501.top

================================================================================
来源：http://atq.jianghu66.top

[F01] 读取整个文件
来源：http://lcy.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jax.guowangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://kpc.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qdj.epnwcf.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zbp.shuidangran.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fwb.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mdq.feifeiyinyue.top

Ruby: File.read("a.txt")
来源：http://cwh.pycfn.com

C#:   File.ReadAllText("a.txt");
来源：http://vnx.mhx1999.top

[F02] 逐行读取文件
来源：http://plv.dashuyun.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ddm.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pcf.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cns.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xzn.fktsv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://arc.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nru.birdmap.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://riz.bjfxy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sda.xylfe.cn

[F03] 写入文件（覆盖）
来源：http://sgl.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://crw.daria6918.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ykc.hfpthk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fyn.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fcj.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wij.hnxiangtu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kpu.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://cmu.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wjb.dashuyun.cn

[F04] 追加写入文件
来源：http://kfz.daxiang520.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rhk.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wvd.sufxvd.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wsh.sufxvd.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ahk.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xfa.cheryme.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rfx.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yoq.mhx1999.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rgh.nanxuanxn.top

[F05] 判断文件或目录是否存在
来源：http://wsk.jyoumei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bch.havefunace.top

PHP:  file_exists("a.txt");
来源：http://bmn.yanxiufei.cn

JS:   fs.existsSync("a.txt")
来源：http://fvk.yuanzhike.top

TS:   fs.existsSync("a.txt")
来源：http://eeq.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pol.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://say.yueranfly.top

Ruby: File.exist?("a.txt")
来源：http://uvv.zhoulong.xyz

C#:   File.Exists("a.txt")
来源：http://snr.ivvv.top

[F06] 删除文件
来源：http://sfm.jianghu66.top

Py:   os.remove("a.txt")
来源：http://wzr.sxryk.cn

PHP:  unlink("a.txt");
来源：http://mlf.sysykeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://sww.0kj1m.cn

TS:   fs.unlinkSync("a.txt")
来源：http://awg.vehdjk.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bak.shanyushiyangtech.top

Go:   os.Remove("a.txt")
来源：http://kbu.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://mmt.ivvv.top

C#:   File.Delete("a.txt");
来源：http://dgz.gogol.net.cn

[F07] 创建目录（含多级）
来源：http://hxa.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hwm.zhaomingkeji.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cwr.jqgufenzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jst.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://exo.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hkd.jinqigfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qjm.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tkc.guowangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xdm.dashuyun.cn

[F08] 遍历目录
来源：http://wwq.hammf.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rcc.havefunace.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xhi.hammf.cn

JS:   fs.readdirSync("dir")
来源：http://nxi.ybcxt.top

TS:   fs.readdirSync("dir")
来源：http://ddt.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qtj.fanxiaobao.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://nhp.jinqigufen.top

Ruby: Dir.children("dir")
来源：http://byd.guowangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://thf.chenlongwang.top

[F09] 获取文件大小
来源：http://xbg.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://zry.tanke756.top

PHP:  filesize("a.txt");
来源：http://ner.xuanzx.com

JS:   fs.statSync("a.txt").size
来源：http://gsh.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://foa.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://zsc.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qnv.zdqjudy.top

Ruby: File.size("a.txt")
来源：http://zoj.sysykeji.top

C#:   new FileInfo("a.txt").Length
来源：http://mjj.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://esu.yangfankeji.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gxd.yj20258888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mkx.ydzc1.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://clu.meibo888.top

TS:   path.extname("a.txt")
来源：http://ygt.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rrb.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mjs.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hql.gaohongyu789.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lxk.ivvv.top

[F11] 复制与移动文件
来源：http://qxo.nwbrower.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vsh.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bqo.hfpthk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ezn.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ooa.tianlin.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ktx.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sfq.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wgo.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oyn.shanyushiyangtech.top

[F12] CSV 读写
来源：http://hll.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nwe.sufxvd.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eva.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://acm.yfazqb.com

TS:   // 同上
来源：http://lno.andypj.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jhb.sxryk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cfd.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dhh.sxryk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ryv.pengpengdd.cyou

================================================================================
来源：http://agy.yonumen.top

G. 面向对象
来源：http://sjc.c1oappe.top

================================================================================
来源：http://jez.gzhubu.top

[G01] 定义类
来源：http://mvs.guannengcc.top

Py:   class User: pass
来源：http://vtg.sysykeji.top

PHP:  class User {}
来源：http://tfb.sweek.top

JS:   class User {}
来源：http://vey.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://jdo.ybcxt.top

Java: class User {}
来源：http://qsv.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://anh.cashguo.top

Ruby: class User; end
来源：http://shy.shuidangran.top

C#:   class User {}
来源：http://het.9152youxi.cn

[G02] 构造函数
来源：http://oxm.uphjek.com

Py:   def __init__(self, name): self.name = name
来源：http://dph.yanxiufei.cn

PHP:  public function __construct(public string $name) {}
来源：http://idv.ywan-chungtsiang.top

JS:   constructor(name) { this.name = name; }
来源：http://bih.tanke756.top

TS:   constructor(public name: string) {}
来源：http://tlr.sysykeji.top

Java: User(String name) { this.name = name; }
来源：http://juh.hnxiangtu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vgw.xziqi.cn

Ruby: def initialize(name); @name = name; end
来源：http://htg.9152youxi.cn

C#:   public User(string name) { Name = name; }
来源：http://kmh.zhongyouzk.top

[G03] 实例属性
来源：http://mnv.hfpthk.cn

Py:   self.name = "x"
来源：http://kna.yuxming.cn

PHP:  public string $name = "x";
来源：http://enp.dianchejie.cn

JS:   this.name = "x";
来源：http://cqk.quarkkingdee.top

TS:   name: string = "x";
来源：http://kpm.cashguo.top

Java: private String name;
来源：http://gyr.jqgfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wuh.chenjidiqi.icu

Ruby: @name = "x"
来源：http://bss.hnqzz.top

C#:   public string Name { get; set; } = "x";
来源：http://zyp.ppjwa.cn

[G04] 定义方法
来源：http://qax.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://tot.nanxinkj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://apy.uphjek.com

JS:   greet() { return this.name; }
来源：http://sfx.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://edi.vqdsnc.cn

Java: String greet() { return name; }
来源：http://kpj.jqgufenzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wtp.xuanzx.com

Ruby: def greet; @name; end
来源：http://fzp.guannengcc.top

C#:   public string Greet() => Name;
来源：http://rtp.ybcxt.top

[G05] 继承
来源：http://ipv.pengpengdd.cyou

Py:   class Admin(User): pass
来源：http://vdn.yj202588.top

PHP:  class Admin extends User {}
来源：http://xwl.jianghu66.top

JS:   class Admin extends User {}
来源：http://oba.shanyushiyangkeji.top

TS:   class Admin extends User {}
来源：http://fon.ehwqpu.com

Java: class Admin extends User {}
来源：http://vko.chenjidiqi.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://whc.ybcxt.top

Ruby: class Admin < User; end
来源：http://ccz.sysykeji.top

C#:   class Admin : User {}
来源：http://gxq.birdmap.top

[G06] 重写方法
来源：http://edz.jinqigfzy.top

Py:   def greet(self): return "admin"
来源：http://yga.gaohongyu789.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jqm.sufxvd.cn

JS:   greet() { return "admin"; }
来源：http://uxl.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://mzg.chenzaomai.com

Java: @Override String greet() { return "admin"; }
来源：http://zvs.andypj.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://flw.tianlin.xyz

Ruby: def greet; "admin"; end
来源：http://reb.tianlin.xyz

C#:   public override string Greet() => "admin";
来源：http://yce.guannengcc.top

[G07] 调用父类方法
来源：http://zcq.52xcode.cn

Py:   super().greet()
来源：http://anr.shangyingyoupin.top

PHP:  parent::greet();
来源：http://jcd.yangfankeji.com

JS:   super.greet();
来源：http://buv.gaohongyu789.top

TS:   super.greet();
来源：http://wzs.pycfn.com

Java: super.greet();
来源：http://lge.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gyq.cdnleiting.top

Ruby: super
来源：http://uxn.gaohongyu789.top

C#:   base.Greet();
来源：http://iiu.yonumen.top

[G08] 静态方法与属性
来源：http://jei.fktsv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wsi.wangdashe.top

PHP:  public static function f() {}
来源：http://lbu.fanxiaobao.xyz

JS:   static f() {}
来源：http://okv.gotoacloud.top

TS:   static f(): void {}
来源：http://fnp.xuetiantiany.cn

Java: static void f() {}
来源：http://wit.yj20258888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ish.yvedp.cn

Ruby: def self.f; end
来源：http://xek.tianlin.xyz

C#:   public static void F() {}
来源：http://ulw.hnqzz.top

[G09] 接口 / 抽象类
来源：http://lfx.yvedp.cn

Py:   from abc import ABC, abstractmethod
来源：http://qiq.xuetiantiany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tkp.zhengqikj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xcf.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://toh.andypj.xyz

Java: interface Shape { double area(); }
来源：http://vnq.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://kbi.yueranfly.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kjq.jinqigufen.top

C#:   interface IShape { double Area(); }
来源：http://dkm.wangdashe.top

[G10] 访问控制
来源：http://xnd.hnxiangtu.top

Py:   约定 _protected / __private（不强制）
来源：http://sax.bbcook.cn

PHP:  public / protected / private
来源：http://xyu.cashguo.top

JS:   #private 字段；其余公开
来源：http://ipc.hfpthk.cn

TS:   public / protected / private
来源：http://bxp.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://jgs.yonumen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://aku.chenzaomai.com

Ruby: public / protected / private
来源：http://vfd.pycfn.com

C#:   public / protected / private / internal
来源：http://uvk.ywan-chungtsiang.top

[G11] getter / setter
来源：http://xfe.sxryk.cn

Py:   @property 与 @x.setter
来源：http://kgw.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://awj.mhx1999.top

JS:   get name() { return this._name; }
来源：http://hmb.nwbrower.top

TS:   get name(): string { return this._name; }
来源：http://tmj.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://odl.quarkkingdee.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uaq.hysaishi.cn

Ruby: attr_accessor :name
来源：http://uby.shuidangran.top

C#:   public string Name { get; set; }
来源：http://iwe.xinyue.icu

[G12] 对象转字符串
来源：http://elv.vehdjk.com

Py:   def __str__(self): return self.name
来源：http://zgb.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://hqy.jqgfzy.top

JS:   toString() { return this.name; }
来源：http://qcb.cashguo.top

TS:   toString(): string { return this.name; }
来源：http://yqv.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://kio.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://dqr.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://loc.cucudq.cn

C#:   public override string ToString() => Name;
来源：http://qjn.yuanzhike.top

[G13] 判断对象类型
来源：http://ezq.zhoulong.xyz

Py:   isinstance(u, User)
来源：http://aao.tarul.cn

PHP:  $u instanceof User
来源：http://hxy.gaohongyu789.top

JS:   u instanceof User
来源：http://bpf.316326.xyz

TS:   u instanceof User
来源：http://wxl.hnxiangtu.top

Java: u instanceof User
来源：http://cdi.fzhhl.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hzg.zhijiandao.cn

Ruby: u.is_a?(User)
来源：http://gbg.yuxming.cn

C#:   u is User
来源：http://bjp.xuanzx.com

[G14] 数据类 / record
来源：http://dwv.iojbl.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://njf.ctjpmb.com

PHP:  // 用 readonly 属性模拟
来源：http://xfg.xziqi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mog.vehdjk.com

TS:   type User = { name: string; age: number };
来源：http://rkr.snrcjt.cn

Java: record User(String name, int age) {}
来源：http://hdg.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://lft.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://elz.zhixingplan.top

C#:   record User(string Name, int Age);
来源：http://wxu.kuanghao11.cn

[G15] 枚举
来源：http://lnr.bjfxy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://slc.hnxiangtu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yan.yvedp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wah.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cyp.iojbl.cn

Java: enum Color { RED, GREEN }
来源：http://rak.zhixingplan.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jqy.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://rse.nanxuanxn.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uml.dianchejie.cn

[G16] 对象转数组 / 字典
来源：http://loy.yuxming.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gki.cdnleiting.top

PHP:  get_object_vars($obj);
来源：http://mys.fehbvm.com

JS:   Object.entries(obj)
来源：http://rft.daria6918.cn

TS:   Object.entries(obj)
来源：http://sfr.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oon.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cme.tanke756.top

Ruby: obj.instance_variables
来源：http://qfi.nanxinkj.top

C#:   // 用反射或 System.Text.Json
来源：http://oao.bjfxy.top

================================================================================
来源：http://hqt.jinqigfzy.top


<!-- 参考信息 -->
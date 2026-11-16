代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ehx.jinghuilouyu.cn

[E19] 多行文本按行拆分
来源：http://dbw.daria6918.cn

Py:   s.splitlines()
来源：http://hos.tianlin.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nae.sweek.top

JS:   s.split(/\r?\n/)
来源：http://mtc.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://xcp.tarul.cn

Java: s.lines().toList()
来源：http://rvc.gaohongyu789.top

Go:   strings.Split(s, "\n")
来源：http://msj.pengpengdd.cyou

Ruby: s.lines
来源：http://zfn.shanyushiyangkeji.top

C#:   s.Split('\n')
来源：http://jmt.gzhubu.top

[E20] 判断字符串是否为空
来源：http://jzy.zhiwuduotai.top

Py:   if not s:
来源：http://mmv.fehbvm.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ilm.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tcy.pycfn.com

TS:   if (s === "") {}
来源：http://wfo.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://exn.dianchejie.cn

Go:   if s == "" {}
来源：http://tfq.daxiang520.top

Ruby: if s.empty?
来源：http://aaa.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wor.tanke756.top

[E21] 超长截断加省略号
来源：http://loy.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://umv.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bkr.redwolf501.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tma.gzhubu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ldt.kuanghao11.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vim.bjfxy.top

Go:   // 按 rune 判断长度后截断
来源：http://jfy.yuanzhike.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fyi.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xwu.zycfv.cn

[E22] 字节长度与字符长度
来源：http://wjl.ivvv.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qwo.cucudq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nuk.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dsl.aibaodan.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vho.aizwys.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gdk.cashguo.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xwd.jlsjyb.cn

Ruby: s.bytesize;  s.length
来源：http://non.havefunace.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yee.shuidangran.top

================================================================================
来源：http://zqx.snrcjt.cn

F. 文件与目录
来源：http://ckh.zhongyouzk.top

================================================================================
来源：http://pzo.tarul.cn

[F01] 读取整个文件
来源：http://umw.ehwqpu.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wip.yj20258.top

PHP:  file_get_contents("a.txt");
来源：http://xxm.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ecp.gotoacloud.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ebb.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://pgm.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tgg.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://nfl.hywenlv.cn

C#:   File.ReadAllText("a.txt");
来源：http://yjt.mhx1999.top

[F02] 逐行读取文件
来源：http://nar.jqgufenzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qfn.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://och.zhixingplan.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wod.pengpengdd.cyou

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nzk.kuanghao11.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jgr.pengpengdd.cyou

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dpo.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ggj.nwbrower.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://abk.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://ewy.ywan-chungtsiang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://crv.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://gdu.9152youxi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kmk.sxryk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mrr.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://peg.zdqjudy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zgh.cheryme.top

Ruby: File.write("a.txt", "hi")
来源：http://eph.zdbjq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://awo.vehdjk.com

[F04] 追加写入文件
来源：http://etn.andypj.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tuk.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nwl.zhijiandao.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ehg.bbcook.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://poe.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qnz.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yvg.hesvh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xqe.hysaishi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bia.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://owc.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xjb.mhx1999.top

PHP:  file_exists("a.txt");
来源：http://oax.gaohongyu789.top

JS:   fs.existsSync("a.txt")
来源：http://tjm.bjfxy.top

TS:   fs.existsSync("a.txt")
来源：http://iwm.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gim.cashguo.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ozz.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://hms.yongpay.top

C#:   File.Exists("a.txt")
来源：http://dop.meibo888.top

[F06] 删除文件
来源：http://fyc.bjfxy.top

Py:   os.remove("a.txt")
来源：http://pyn.jlsjyb.cn

PHP:  unlink("a.txt");
来源：http://uzn.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://rmf.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://iwb.ydzc1.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vjy.shanyushiyangkeji.top

Go:   os.Remove("a.txt")
来源：http://pby.birdmap.top

Ruby: File.delete("a.txt")
来源：http://dpa.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://yxw.yuxming.cn

[F07] 创建目录（含多级）
来源：http://gcq.andypj.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jtu.havefunace.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://clx.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hkq.shanyushiyangtech.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hcb.feifeiyinyue.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fjn.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://occ.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dyh.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uos.yangfankeji.com

[F08] 遍历目录
来源：http://ehv.aizwys.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vgp.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jyb.zhixingplan.top

JS:   fs.readdirSync("dir")
来源：http://cwx.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://cnp.daxiang520.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sac.xuanzx.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://wgg.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://prb.ppjwa.cn

C#:   Directory.GetFiles("dir")
来源：http://axa.fehbvm.com

[F09] 获取文件大小
来源：http://ecu.hfpthk.cn

Py:   os.path.getsize("a.txt")
来源：http://mth.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://txv.tianlin.xyz

JS:   fs.statSync("a.txt").size
来源：http://wxf.xinyue.icu

TS:   fs.statSync("a.txt").size
来源：http://fif.nwbrower.top

Java: Files.size(Path.of("a.txt"))
来源：http://pww.ctjpmb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://agh.cheryme.top

Ruby: File.size("a.txt")
来源：http://saw.fanxiaobao.xyz

C#:   new FileInfo("a.txt").Length
来源：http://twm.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://rnj.chenlongwang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rei.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://igi.zhoulong.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bbv.zhiwuduotai.top

TS:   path.extname("a.txt")
来源：http://sly.pycfn.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fbt.zhoulong.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xjq.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sla.yueranfly.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eun.sxryk.cn

[F11] 复制与移动文件
来源：http://zre.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wjc.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://alk.ydjk.org.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mqo.hammf.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://snc.zhiwuduotai.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zdr.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lgh.ehwqpu.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tni.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iip.gogol.net.cn

[F12] CSV 读写
来源：http://bmh.9152youxi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ymd.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gey.zhiwuduotai.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ibw.pengpengdd.cyou

TS:   // 同上
来源：http://mar.c1oappe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://osa.daria6918.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kme.svipenyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kkj.yueranfly.top

C#:   // 无内置：用 CsvHelper 库
来源：http://msh.guowangkeji.top

================================================================================
来源：http://gpx.wangdashe.top

G. 面向对象
来源：http://luk.daria6918.cn

================================================================================
来源：http://dxw.ctjpmb.com

[G01] 定义类
来源：http://whd.shuidangran.top

Py:   class User: pass
来源：http://ptn.jyoumei.cn

PHP:  class User {}
来源：http://zfu.yuxming.cn

JS:   class User {}
来源：http://yjs.pycfn.com

TS:   class User { name: string = ""; }
来源：http://jld.yj20258888.top

Java: class User {}
来源：http://ivs.jinqigufen.top

Go:   type User struct { Name string }
来源：http://oqw.fanxiaobao.xyz

Ruby: class User; end
来源：http://erq.sysykeji.top

C#:   class User {}
来源：http://vjt.sysykeji.top

[G02] 构造函数
来源：http://bem.aizwys.cn

Py:   def __init__(self, name): self.name = name
来源：http://hkk.iojbl.cn

PHP:  public function __construct(public string $name) {}
来源：http://cyw.gaohongyu789.top

JS:   constructor(name) { this.name = name; }
来源：http://xsa.sxryk.cn

TS:   constructor(public name: string) {}
来源：http://ddi.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://xkk.xziqi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://whr.jinqigufen.top

Ruby: def initialize(name); @name = name; end
来源：http://qxd.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://hps.hnxiangtu.top

[G03] 实例属性
来源：http://idv.xingfuxueyuan.xyz

Py:   self.name = "x"
来源：http://riu.fzhhl.top

PHP:  public string $name = "x";
来源：http://rzc.yfazqb.com

JS:   this.name = "x";
来源：http://kvd.tarul.cn

TS:   name: string = "x";
来源：http://scc.sufxvd.cn

Java: private String name;
来源：http://aiq.yvedp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uoj.cheryme.top

Ruby: @name = "x"
来源：http://mgx.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://yfz.sufxvd.cn

[G04] 定义方法
来源：http://egt.redwolf501.top

Py:   def greet(self): return self.name
来源：http://whv.zhixingplan.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tfw.chenjidiqi.icu

JS:   greet() { return this.name; }
来源：http://mfh.jinyuanbaomall.cn

TS:   greet(): string { return this.name; }
来源：http://ele.jinqigufen.top

Java: String greet() { return name; }
来源：http://beq.jqgfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nxz.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://asj.ybcxt.top

C#:   public string Greet() => Name;
来源：http://wjj.jinyuanbaomall.cn

[G05] 继承
来源：http://por.jinqigufen.top

Py:   class Admin(User): pass
来源：http://buj.daxiang520.top

PHP:  class Admin extends User {}
来源：http://zed.yanxiufei.cn

JS:   class Admin extends User {}
来源：http://iop.ybcxt.top

TS:   class Admin extends User {}
来源：http://yqf.jqgfzy.top

Java: class Admin extends User {}
来源：http://txv.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://agf.snrcjt.cn

Ruby: class Admin < User; end
来源：http://kkx.cucudq.cn

C#:   class Admin : User {}
来源：http://lrm.shzxlz.cn

[G06] 重写方法
来源：http://kvt.ivvv.top

Py:   def greet(self): return "admin"
来源：http://pzt.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wtc.chenlongwang.top

JS:   greet() { return "admin"; }
来源：http://yaj.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://nbl.redwolf501.top

Java: @Override String greet() { return "admin"; }
来源：http://zno.ydzc1.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://avg.316326.xyz

Ruby: def greet; "admin"; end
来源：http://rsv.jianghu66.top

C#:   public override string Greet() => "admin";
来源：http://ega.yj20258888.top

[G07] 调用父类方法
来源：http://fbf.jinghuilouyu.cn

Py:   super().greet()
来源：http://lvm.sufxvd.cn

PHP:  parent::greet();
来源：http://vzh.andypj.xyz

JS:   super.greet();
来源：http://dov.zdqjudy.top

TS:   super.greet();
来源：http://qri.yueranfly.top

Java: super.greet();
来源：http://rib.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pit.xuetiantiany.cn

Ruby: super
来源：http://ztv.xinyue.icu

C#:   base.Greet();
来源：http://sxo.fanxiaobao.xyz

[G08] 静态方法与属性
来源：http://ato.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://isr.yonumen.top

PHP:  public static function f() {}
来源：http://aeg.havefunace.top

JS:   static f() {}
来源：http://lla.redwolf501.top

TS:   static f(): void {}
来源：http://ala.zhoulong.xyz

Java: static void f() {}
来源：http://wln.9152youxi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eqz.mhx1999.top

Ruby: def self.f; end
来源：http://xfb.andypj.xyz

C#:   public static void F() {}
来源：http://kbn.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://xuq.ctjpmb.com

Py:   from abc import ABC, abstractmethod
来源：http://kqj.smart0.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://guk.daxiang520.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lkk.gaohongyu789.top

TS:   interface Shape { area(): number; }
来源：http://paq.dashuyun.cn

Java: interface Shape { double area(); }
来源：http://uew.sufxvd.cn

Go:   type Shape interface { Area() float64 }
来源：http://exf.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rka.jyoumei.cn

C#:   interface IShape { double Area(); }
来源：http://evp.sjlbkw.cn

[G10] 访问控制
来源：http://afl.pengpengdd.cyou

Py:   约定 _protected / __private（不强制）
来源：http://nzw.pycfn.com

PHP:  public / protected / private
来源：http://oio.jinyuanbaomall.cn

JS:   #private 字段；其余公开
来源：http://mcx.zhijiandao.cn

TS:   public / protected / private
来源：http://zos.sxryk.cn

Java: public / protected / private / 默认包级
来源：http://rri.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://lkp.zycfv.cn

Ruby: public / protected / private
来源：http://hij.nanxinkj.top

C#:   public / protected / private / internal
来源：http://vjg.yanxiufei.cn

[G11] getter / setter
来源：http://tdh.yj20258.top

Py:   @property 与 @x.setter
来源：http://efu.gotoacloud.top

PHP:  public function getName(): string { return $this->name; }
来源：http://eug.ydzc1.top

JS:   get name() { return this._name; }
来源：http://ewa.zhoulong.xyz

TS:   get name(): string { return this._name; }
来源：http://gfo.cashguo.top

Java: public String getName() { return name; }
来源：http://ysz.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fdh.svipenyu.cn

Ruby: attr_accessor :name
来源：http://ypk.cqqwz.cn

C#:   public string Name { get; set; }
来源：http://hsd.aizwys.cn

[G12] 对象转字符串
来源：http://bta.bbcook.cn

Py:   def __str__(self): return self.name
来源：http://amr.yongpay.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jkj.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://fzk.hongshengwenyu.top

TS:   toString(): string { return this.name; }
来源：http://kzk.cqqwz.cn

Java: @Override public String toString() { return name; }
来源：http://ete.fzhhl.top

Go:   func (u User) String() string { return u.Name }
来源：http://ote.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://hlb.hnxiangtu.top

C#:   public override string ToString() => Name;
来源：http://egi.cdnleiting.top

[G13] 判断对象类型
来源：http://xqr.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://kxd.kuanghao11.cn

PHP:  $u instanceof User
来源：http://kvr.chenjidiqi.icu

JS:   u instanceof User
来源：http://npf.xziqi.cn

TS:   u instanceof User
来源：http://kma.yanxiufei.cn

Java: u instanceof User
来源：http://bwt.cashguo.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://beh.hfpthk.cn

Ruby: u.is_a?(User)
来源：http://qut.hfpthk.cn

C#:   u is User
来源：http://qzf.birdmap.top

[G14] 数据类 / record
来源：http://fkg.xingfuxueyuan.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://abh.xuetiantiany.cn

PHP:  // 用 readonly 属性模拟
来源：http://tah.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://rzm.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://bnl.svipenyu.cn

Java: record User(String name, int age) {}
来源：http://rty.xuanzx.com

Go:   type User struct { Name string; Age int }
来源：http://mng.mhx1999.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gxp.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://ubr.chenlongwang.top

[G15] 枚举
来源：http://izt.9152youxi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qni.cashguo.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://alk.jqgfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wsc.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bwm.pycfn.com

Java: enum Color { RED, GREEN }
来源：http://ggv.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zhq.gzhubu.top

Ruby: Color = %i[red green].freeze
来源：http://mwm.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jad.0kj1m.cn

[G16] 对象转数组 / 字典
来源：http://vnf.daria6918.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://syl.yj20258888.top

PHP:  get_object_vars($obj);
来源：http://nqu.shanyushiyangtech.top

JS:   Object.entries(obj)
来源：http://rzh.ehwqpu.com

TS:   Object.entries(obj)
来源：http://edq.zhiwuduotai.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yjv.zdbjq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yow.snrcjt.cn

Ruby: obj.instance_variables
来源：http://lff.quarkkingdee.top

C#:   // 用反射或 System.Text.Json
来源：http://gzf.yonumen.top

================================================================================
来源：http://tbm.svipenyu.cn

H. 异常与错误处理
来源：http://isz.yvedp.cn

================================================================================
来源：http://viz.xuetiantiany.cn

[H01] try / catch 基础
来源：http://oal.pycfn.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://auf.yanxiufei.cn


<!-- 参考信息 -->
代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://zob.zycfv.cn

TS:   s.split(/\r?\n/)
来源：http://ytf.ywan-chungtsiang.top

Java: s.lines().toList()
来源：http://les.pengpengdd.cyou

Go:   strings.Split(s, "\n")
来源：http://ibw.fzhhl.top

Ruby: s.lines
来源：http://uwd.cqqwz.cn

C#:   s.Split('\n')
来源：http://bao.vehdjk.com

[E20] 判断字符串是否为空
来源：http://kst.uphjek.com

Py:   if not s:
来源：http://cxg.zhengqikj.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lxz.yfazqb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://awl.ehwqpu.com

TS:   if (s === "") {}
来源：http://cmc.jqgfzy.top

Java: if (s.isEmpty()) {}
来源：http://hcp.zdbjq.cn

Go:   if s == "" {}
来源：http://aqw.quarkkingdee.top

Ruby: if s.empty?
来源：http://hwx.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fkq.cashguo.top

[E21] 超长截断加省略号
来源：http://txx.xingfuxueyuan.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rtf.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fss.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yma.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rjy.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ygl.fktsv.cn

Go:   // 按 rune 判断长度后截断
来源：http://srl.zhijiandao.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wtm.pengpengdd.cyou

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lzi.gotoacloud.top

[E22] 字节长度与字符长度
来源：http://hdw.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://giv.yj20258.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ihx.zhiwuduotai.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wri.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ngv.guannengcc.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ipt.bjfxy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wub.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://pyi.mhx1999.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ftj.vehdjk.com

================================================================================
来源：http://jlx.birdmap.top

F. 文件与目录
来源：http://oal.zhengqikj.top

================================================================================
来源：http://jxd.ehwqpu.com

[F01] 读取整个文件
来源：http://rzl.hnxiangtu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lje.0kj1m.cn

PHP:  file_get_contents("a.txt");
来源：http://wqd.fanxiaobao.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gkf.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dqp.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://qak.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hyx.yj202588.top

Ruby: File.read("a.txt")
来源：http://pua.gogol.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://nzi.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://neg.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wll.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vkt.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dih.yj202588.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yuc.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hqj.tanke756.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vux.redwolf501.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mow.bjfxy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iyp.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://mpf.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jis.fktsv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://swc.nanxinkj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wzj.jlsjyb.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cfr.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wzq.guannengcc.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wbm.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://hva.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gqj.316326.xyz

[F04] 追加写入文件
来源：http://qwf.sufxvd.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sep.zhoulong.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tvt.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lke.jinqigufen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nuy.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ovd.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aau.hnxiangtu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qik.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vep.ydjk.org.cn

[F05] 判断文件或目录是否存在
来源：http://vjd.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hma.xinyue.icu

PHP:  file_exists("a.txt");
来源：http://gdm.uphjek.com

JS:   fs.existsSync("a.txt")
来源：http://yew.zhoulong.xyz

TS:   fs.existsSync("a.txt")
来源：http://cus.yanxiufei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ghc.cashguo.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vxb.chenjidiqi.icu

Ruby: File.exist?("a.txt")
来源：http://pjm.jinghuilouyu.cn

C#:   File.Exists("a.txt")
来源：http://vmy.hywenlv.cn

[F06] 删除文件
来源：http://cof.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://qop.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://jbi.hnxiangtu.top

JS:   fs.unlinkSync("a.txt")
来源：http://mkv.daxiang520.top

TS:   fs.unlinkSync("a.txt")
来源：http://qhq.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tpd.ppjwa.cn

Go:   os.Remove("a.txt")
来源：http://ymb.zhijiandao.cn

Ruby: File.delete("a.txt")
来源：http://sto.wangdashe.top

C#:   File.Delete("a.txt");
来源：http://yrx.xinyue.icu

[F07] 创建目录（含多级）
来源：http://qsd.jqgufenzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mww.gzhubu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yeb.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mjt.xylfe.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vaa.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rei.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yrr.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xdw.zhaomingkeji.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dda.chenzaomai.com

[F08] 遍历目录
来源：http://fqj.meibo888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vcn.c1oappe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rmv.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://wlm.chenlongwang.top

TS:   fs.readdirSync("dir")
来源：http://yqz.ppjwa.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bqs.xuanzx.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://wqj.nanxuanxn.top

Ruby: Dir.children("dir")
来源：http://etd.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://mzx.xuetiantiany.cn

[F09] 获取文件大小
来源：http://qlh.dashuyun.cn

Py:   os.path.getsize("a.txt")
来源：http://ooz.chenjidiqi.icu

PHP:  filesize("a.txt");
来源：http://ikt.pengpengdd.cyou

JS:   fs.statSync("a.txt").size
来源：http://koz.xziqi.cn

TS:   fs.statSync("a.txt").size
来源：http://lbz.fehbvm.com

Java: Files.size(Path.of("a.txt"))
来源：http://hyi.yonumen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nec.gzhubu.top

Ruby: File.size("a.txt")
来源：http://heq.yuanzhike.top

C#:   new FileInfo("a.txt").Length
来源：http://xlh.xingfuxueyuan.xyz

[F10] 取文件扩展名 / 文件名
来源：http://ufe.0kj1m.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://arj.fktsv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ljk.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vzg.vqdsnc.cn

TS:   path.extname("a.txt")
来源：http://sah.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://akx.chenlongwang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://euf.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bxe.tianlin.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jok.yj20258888.top

[F11] 复制与移动文件
来源：http://qji.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://val.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nzo.cdnleiting.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xey.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kfj.yuanzhike.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://seq.dianchejie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nvw.ydzc1.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vph.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jds.chenjidiqi.icu

[F12] CSV 读写
来源：http://frm.jianghu66.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qqf.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mbn.c1oappe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vrj.gotoacloud.top

TS:   // 同上
来源：http://lno.snrcjt.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ahj.hywenlv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vnd.yonumen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://swa.jinyuanbaomall.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pfo.shangyingyoupin.top

================================================================================
来源：http://loq.dashuyun.cn

G. 面向对象
来源：http://akm.shangyingyoupin.top

================================================================================
来源：http://wnf.jinghuilouyu.cn

[G01] 定义类
来源：http://tow.zhoulong.xyz

Py:   class User: pass
来源：http://mji.yonumen.top

PHP:  class User {}
来源：http://qvd.yueranfly.top

JS:   class User {}
来源：http://uoo.hesvh.cn

TS:   class User { name: string = ""; }
来源：http://pqu.birdmap.top

Java: class User {}
来源：http://ttm.zhaomingkeji.xyz

Go:   type User struct { Name string }
来源：http://mte.ivvv.top

Ruby: class User; end
来源：http://xgz.316326.xyz

C#:   class User {}
来源：http://fdk.haohaochexian.top

[G02] 构造函数
来源：http://hvv.bbcook.cn

Py:   def __init__(self, name): self.name = name
来源：http://xov.yj20258.top

PHP:  public function __construct(public string $name) {}
来源：http://ual.bbcook.cn

JS:   constructor(name) { this.name = name; }
来源：http://jmw.cqqwz.cn

TS:   constructor(public name: string) {}
来源：http://fot.wangshuangyany.cn

Java: User(String name) { this.name = name; }
来源：http://azh.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rul.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://jbm.mhx1999.top

C#:   public User(string name) { Name = name; }
来源：http://scw.shanyushiyangkeji.top

[G03] 实例属性
来源：http://uyu.316326.xyz

Py:   self.name = "x"
来源：http://vin.hammf.cn

PHP:  public string $name = "x";
来源：http://bli.jlsjyb.cn

JS:   this.name = "x";
来源：http://och.sufxvd.cn

TS:   name: string = "x";
来源：http://utd.xuanzx.com

Java: private String name;
来源：http://gnt.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lsx.yuxming.cn

Ruby: @name = "x"
来源：http://nrr.jinqigufen.top

C#:   public string Name { get; set; } = "x";
来源：http://lbc.sxryk.cn

[G04] 定义方法
来源：http://wdf.tarul.cn

Py:   def greet(self): return self.name
来源：http://ndx.sxryk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ouy.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://nex.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://ugm.yueranfly.top

Java: String greet() { return name; }
来源：http://mbd.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bmu.ydjk.org.cn

Ruby: def greet; @name; end
来源：http://xwm.zhongyouzk.top

C#:   public string Greet() => Name;
来源：http://vwu.ywan-chungtsiang.top

[G05] 继承
来源：http://hjo.svipenyu.cn

Py:   class Admin(User): pass
来源：http://mjk.nanxinkj.top

PHP:  class Admin extends User {}
来源：http://ivr.jyoumei.cn

JS:   class Admin extends User {}
来源：http://fmp.birdmap.top

TS:   class Admin extends User {}
来源：http://lri.nwbrower.top

Java: class Admin extends User {}
来源：http://bya.yuanzhike.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kim.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://lzz.zhongyouzk.top

C#:   class Admin : User {}
来源：http://aww.yfazqb.com

[G06] 重写方法
来源：http://kat.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://pkf.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://btm.yangfankeji.com

JS:   greet() { return "admin"; }
来源：http://iwg.yuxming.cn

TS:   greet(): string { return "admin"; }
来源：http://pxh.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://nxy.nwbrower.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uyg.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://txa.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://ugw.cqqwz.cn

[G07] 调用父类方法
来源：http://ond.hnqzz.top

Py:   super().greet()
来源：http://djh.yj20258888.top

PHP:  parent::greet();
来源：http://ydt.yuxming.cn

JS:   super.greet();
来源：http://eci.yj202588.top

TS:   super.greet();
来源：http://mzl.mhx1999.top

Java: super.greet();
来源：http://cyk.zdqjudy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fip.haohaochexian.top

Ruby: super
来源：http://ykg.yongpay.top

C#:   base.Greet();
来源：http://ern.yj202588.top

[G08] 静态方法与属性
来源：http://xwj.shanyushiyangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ujb.haohaochexian.top

PHP:  public static function f() {}
来源：http://uaq.yj202588.top

JS:   static f() {}
来源：http://mmx.yangfankeji.com

TS:   static f(): void {}
来源：http://pyy.shuidangran.top

Java: static void f() {}
来源：http://qrm.zycfv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ayr.gotoacloud.top

Ruby: def self.f; end
来源：http://igm.jiagoushi.top

C#:   public static void F() {}
来源：http://bph.xinyue.icu

[G09] 接口 / 抽象类
来源：http://hbg.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://ukd.xuetiantiany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yqs.nanxuanxn.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mbs.jqgufenzy.top

TS:   interface Shape { area(): number; }
来源：http://eec.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://zht.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://sgn.yfazqb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://odx.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://kyb.xuanzx.com

[G10] 访问控制
来源：http://qsc.xziqi.cn

Py:   约定 _protected / __private（不强制）
来源：http://hgi.fanxiaobao.xyz

PHP:  public / protected / private
来源：http://yko.haohaochexian.top

JS:   #private 字段；其余公开
来源：http://sfz.nwbrower.top

TS:   public / protected / private
来源：http://jey.xingfuxueyuan.xyz

Java: public / protected / private / 默认包级
来源：http://syv.hesvh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bgj.zhiwuduotai.top

Ruby: public / protected / private
来源：http://zhp.andypj.xyz

C#:   public / protected / private / internal
来源：http://gvi.guannengcc.top

[G11] getter / setter
来源：http://lmp.zhixingplan.top

Py:   @property 与 @x.setter
来源：http://tfn.chenjidiqi.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://yka.hongshengwenyu.top

JS:   get name() { return this._name; }
来源：http://eaz.haohaochexian.top

TS:   get name(): string { return this._name; }
来源：http://ygs.hywenlv.cn

Java: public String getName() { return name; }
来源：http://fgj.hongshengwenyu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gmk.guannengcc.top

Ruby: attr_accessor :name
来源：http://pci.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://ofs.vehdjk.com

[G12] 对象转字符串
来源：http://ede.chenjidiqi.icu

Py:   def __str__(self): return self.name
来源：http://fkz.zhoulong.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://prk.yongpay.top

JS:   toString() { return this.name; }
来源：http://dxj.shangyingyoupin.top

TS:   toString(): string { return this.name; }
来源：http://onj.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://qsb.zdqjudy.top

Go:   func (u User) String() string { return u.Name }
来源：http://clg.jyoumei.cn

Ruby: def to_s; @name; end
来源：http://pcn.chenlongwang.top

C#:   public override string ToString() => Name;
来源：http://acm.xuanzx.com

[G13] 判断对象类型
来源：http://pir.aizwys.cn

Py:   isinstance(u, User)
来源：http://ymk.dianchejie.cn

PHP:  $u instanceof User
来源：http://yem.hcnkem.com

JS:   u instanceof User
来源：http://vmq.tian-w.cn

TS:   u instanceof User
来源：http://vcf.fzhhl.top

Java: u instanceof User
来源：http://byg.epnwcf.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://amf.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://uwv.shzxlz.cn

C#:   u is User
来源：http://dfc.dashuyun.cn

[G14] 数据类 / record
来源：http://vdo.zdqjudy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hvl.yj20258.top

PHP:  // 用 readonly 属性模拟
来源：http://xbs.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://bzr.gogol.net.cn

TS:   type User = { name: string; age: number };
来源：http://quf.yj20258888.top

Java: record User(String name, int age) {}
来源：http://asv.ydzc1.top

Go:   type User struct { Name string; Age int }
来源：http://fov.316326.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gwf.fengsongda.top

C#:   record User(string Name, int Age);
来源：http://rxy.c1oappe.top

[G15] 枚举
来源：http://irg.zycfv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ueg.sweek.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kif.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cto.zdbjq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kak.tarul.cn

Java: enum Color { RED, GREEN }
来源：http://rjd.shanyushiyangtech.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pco.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://ujm.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dbz.sufxvd.cn

[G16] 对象转数组 / 字典
来源：http://zgl.cqqwz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xke.shanyushiyangtech.top

PHP:  get_object_vars($obj);
来源：http://mpo.snrcjt.cn

JS:   Object.entries(obj)
来源：http://geb.guannengcc.top

TS:   Object.entries(obj)
来源：http://ygr.xuetiantiany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://urh.yuxming.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oif.pycfn.com

Ruby: obj.instance_variables
来源：http://ndb.daria6918.cn

C#:   // 用反射或 System.Text.Json
来源：http://oid.yangfankeji.com

================================================================================
来源：http://jac.zycfv.cn

H. 异常与错误处理
来源：http://vmv.shangyingyoupin.top

================================================================================
来源：http://mbo.hesvh.cn

[H01] try / catch 基础
来源：http://btl.shanyushiyangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dls.vehdjk.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jkg.jinqigfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ahv.gogol.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gey.jinqigfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://imb.hammf.cn


<!-- 参考信息 -->
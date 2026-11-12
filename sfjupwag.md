代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dkk.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qvz.dianchejie.cn

Ruby: s.capitalize
来源：http://jjr.ywan-chungtsiang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wux.jinqigfzy.top

[E18] 模板占位符替换
来源：http://pvr.jianghu66.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oxu.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://shv.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://lte.redwolf501.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wgh.shangyingyoupin.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://prh.wangdashe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rke.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rhb.quarkkingdee.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jax.daxiang520.top

[E19] 多行文本按行拆分
来源：http://hvt.yanxiufei.cn

Py:   s.splitlines()
来源：http://xwh.hnxiangtu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gyt.chenlongwang.top

JS:   s.split(/\r?\n/)
来源：http://kpy.fktsv.cn

TS:   s.split(/\r?\n/)
来源：http://qin.fanxiaobao.xyz

Java: s.lines().toList()
来源：http://nvy.dianchejie.cn

Go:   strings.Split(s, "\n")
来源：http://wgm.guannengcc.top

Ruby: s.lines
来源：http://cuq.ydjk.org.cn

C#:   s.Split('\n')
来源：http://nub.fehbvm.com

[E20] 判断字符串是否为空
来源：http://ogg.tianlin.xyz

Py:   if not s:
来源：http://mde.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zsv.cashguo.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yqb.xinyue.icu

TS:   if (s === "") {}
来源：http://epu.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://oeq.jlsjyb.cn

Go:   if s == "" {}
来源：http://dsf.yj20258888.top

Ruby: if s.empty?
来源：http://gkh.hysaishi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ubk.bbcook.cn

[E21] 超长截断加省略号
来源：http://qzq.redwolf501.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://els.bbcook.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ite.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lzw.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://slv.mhx1999.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zhq.ybcxt.top

Go:   // 按 rune 判断长度后截断
来源：http://vfs.tarul.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qln.cqqwz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dmy.chenjidiqi.icu

[E22] 字节长度与字符长度
来源：http://qkz.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sqm.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dwq.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rxl.c1oappe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mpt.hfpthk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vsa.cqqwz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mcb.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://dye.jinyuanbaomall.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sdn.yueranfly.top

================================================================================
来源：http://jwq.guannengcc.top

F. 文件与目录
来源：http://rep.c1oappe.top

================================================================================
来源：http://czf.yuanzhike.top

[F01] 读取整个文件
来源：http://uoq.sweek.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mdw.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://bqr.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mwh.yueranfly.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://loe.zhoulong.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://vrv.ydjk.org.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tsl.fktsv.cn

Ruby: File.read("a.txt")
来源：http://szs.redwolf501.top

C#:   File.ReadAllText("a.txt");
来源：http://lxe.xylfe.cn

[F02] 逐行读取文件
来源：http://eye.dianchejie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kam.ctjpmb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://opv.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mcv.zhixingplan.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://itb.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dpu.yueranfly.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ibm.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dad.jinqigfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://now.redwolf501.top

[F03] 写入文件（覆盖）
来源：http://emp.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://grr.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://tzf.jqgufenzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://now.yuanzhike.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qey.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jbn.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ngd.yonumen.top

Ruby: File.write("a.txt", "hi")
来源：http://jtk.hnxiangtu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ufs.fengsongda.top

[F04] 追加写入文件
来源：http://ggo.fzhhl.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rog.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dzj.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xvb.hongshengwenyu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mgu.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dkn.chenzaomai.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vig.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vfv.shanyushiyangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nih.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://xyj.sxryk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bil.smart0.xyz

PHP:  file_exists("a.txt");
来源：http://hdx.tanke756.top

JS:   fs.existsSync("a.txt")
来源：http://lqd.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://tll.zhongyouzk.top

Java: Files.exists(Path.of("a.txt"))
来源：http://uyw.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bjt.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://efq.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://zjw.zdbjq.cn

[F06] 删除文件
来源：http://agj.redwolf501.top

Py:   os.remove("a.txt")
来源：http://arm.ivvv.top

PHP:  unlink("a.txt");
来源：http://dyv.kuanghao11.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yxy.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://blm.quarkkingdee.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://epm.jqgfzy.top

Go:   os.Remove("a.txt")
来源：http://hej.jqgufenzy.top

Ruby: File.delete("a.txt")
来源：http://ocz.yueranfly.top

C#:   File.Delete("a.txt");
来源：http://vmg.hammf.cn

[F07] 创建目录（含多级）
来源：http://utt.cdnleiting.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gqy.xinyue.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zki.yj20258.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gua.9152youxi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fuv.jqgfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ddv.ppjwa.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://urh.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iuv.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ulm.fehbvm.com

[F08] 遍历目录
来源：http://two.xylfe.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hbq.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dxj.wangdashe.top

JS:   fs.readdirSync("dir")
来源：http://ttx.chenlongwang.top

TS:   fs.readdirSync("dir")
来源：http://phu.zhijiandao.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zmu.zdqjudy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hvf.gzhubu.top

Ruby: Dir.children("dir")
来源：http://gam.jiagoushi.top

C#:   Directory.GetFiles("dir")
来源：http://swn.smart0.xyz

[F09] 获取文件大小
来源：http://blr.jqgfzy.top

Py:   os.path.getsize("a.txt")
来源：http://pse.jianghu66.top

PHP:  filesize("a.txt");
来源：http://qfa.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://cph.xinyue.icu

TS:   fs.statSync("a.txt").size
来源：http://gha.hcnkem.com

Java: Files.size(Path.of("a.txt"))
来源：http://vvv.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yvh.hywenlv.cn

Ruby: File.size("a.txt")
来源：http://kux.jlsjyb.cn

C#:   new FileInfo("a.txt").Length
来源：http://txf.yj202588.top

[F10] 取文件扩展名 / 文件名
来源：http://qyz.smart0.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dim.sxryk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tni.xingfuxueyuan.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dwz.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://lpd.shangyingyoupin.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rdg.sjlbkw.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ice.chenlongwang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zpw.tian-w.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ash.fanxiaobao.xyz

[F11] 复制与移动文件
来源：http://wlm.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jxp.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mxw.gotoacloud.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://npx.aizwys.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nrn.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://voi.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://egt.jqgufenzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://esz.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nik.bjfxy.top

[F12] CSV 读写
来源：http://uug.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wdf.9152youxi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ryo.jlsjyb.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bnd.0kj1m.cn

TS:   // 同上
来源：http://gnd.zhoulong.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sok.zhoulong.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vbw.vehdjk.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dwj.epnwcf.com

C#:   // 无内置：用 CsvHelper 库
来源：http://dot.chenlongwang.top

================================================================================
来源：http://xum.jiagoushi.top

G. 面向对象
来源：http://pzq.yanxiufei.cn

================================================================================
来源：http://ufu.jinghuilouyu.cn

[G01] 定义类
来源：http://kmu.bbcook.cn

Py:   class User: pass
来源：http://yxq.tian-w.cn

PHP:  class User {}
来源：http://pgx.jlsjyb.cn

JS:   class User {}
来源：http://vjs.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://crq.sysykeji.top

Java: class User {}
来源：http://dki.ehwqpu.com

Go:   type User struct { Name string }
来源：http://ola.jinqigfzy.top

Ruby: class User; end
来源：http://pac.jianghu66.top

C#:   class User {}
来源：http://wbg.jqgfzy.top

[G02] 构造函数
来源：http://llg.xziqi.cn

Py:   def __init__(self, name): self.name = name
来源：http://nkk.pengpengdd.cyou

PHP:  public function __construct(public string $name) {}
来源：http://pwn.zhiwuduotai.top

JS:   constructor(name) { this.name = name; }
来源：http://vdz.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://jxx.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://ail.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kut.ctjpmb.com

Ruby: def initialize(name); @name = name; end
来源：http://cyi.jlsjyb.cn

C#:   public User(string name) { Name = name; }
来源：http://uly.52xcode.cn

[G03] 实例属性
来源：http://ajj.jyoumei.cn

Py:   self.name = "x"
来源：http://esv.xinyue.icu

PHP:  public string $name = "x";
来源：http://dfk.shuidangran.top

JS:   this.name = "x";
来源：http://len.cheryme.top

TS:   name: string = "x";
来源：http://oqe.wangshuangyany.cn

Java: private String name;
来源：http://wbv.jinqigufen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cka.gogol.net.cn

Ruby: @name = "x"
来源：http://aaw.guannengcc.top

C#:   public string Name { get; set; } = "x";
来源：http://qbg.tianlin.xyz

[G04] 定义方法
来源：http://gqg.fehbvm.com

Py:   def greet(self): return self.name
来源：http://qzp.birdmap.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nlp.aizwys.cn

JS:   greet() { return this.name; }
来源：http://zku.jianghu66.top

TS:   greet(): string { return this.name; }
来源：http://und.yj202588.top

Java: String greet() { return name; }
来源：http://kpg.zhixingplan.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tib.vqdsnc.cn

Ruby: def greet; @name; end
来源：http://pdf.fktsv.cn

C#:   public string Greet() => Name;
来源：http://fdf.ctjpmb.com

[G05] 继承
来源：http://gjs.yuanzhike.top

Py:   class Admin(User): pass
来源：http://bcz.fktsv.cn

PHP:  class Admin extends User {}
来源：http://fel.hnqzz.top

JS:   class Admin extends User {}
来源：http://vjd.chenzaomai.com

TS:   class Admin extends User {}
来源：http://ynh.zhoulong.xyz

Java: class Admin extends User {}
来源：http://txk.jianghu66.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ixl.havefunace.top

Ruby: class Admin < User; end
来源：http://zfb.zdbjq.cn

C#:   class Admin : User {}
来源：http://ufd.hywenlv.cn

[G06] 重写方法
来源：http://rur.hcnkem.com

Py:   def greet(self): return "admin"
来源：http://cuz.guannengcc.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xly.haohaochexian.top

JS:   greet() { return "admin"; }
来源：http://aer.tian-w.cn

TS:   greet(): string { return "admin"; }
来源：http://oua.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://vbt.ctjpmb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vim.fzhhl.top

Ruby: def greet; "admin"; end
来源：http://krf.gotoacloud.top

C#:   public override string Greet() => "admin";
来源：http://ixo.zycfv.cn

[G07] 调用父类方法
来源：http://kob.chenlongwang.top

Py:   super().greet()
来源：http://coc.shuidangran.top

PHP:  parent::greet();
来源：http://iyh.fktsv.cn

JS:   super.greet();
来源：http://alk.xinyue.icu

TS:   super.greet();
来源：http://jbn.gotoacloud.top

Java: super.greet();
来源：http://wsh.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://shs.cheryme.top

Ruby: super
来源：http://jhp.daxiang520.top

C#:   base.Greet();
来源：http://rap.zycfv.cn

[G08] 静态方法与属性
来源：http://omu.ywan-chungtsiang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fgx.chenlongwang.top

PHP:  public static function f() {}
来源：http://egc.mhx1999.top

JS:   static f() {}
来源：http://rip.tianlin.xyz

TS:   static f(): void {}
来源：http://tqx.aibaodan.cn

Java: static void f() {}
来源：http://zhu.hnxiangtu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://czs.chenlongwang.top

Ruby: def self.f; end
来源：http://cjw.zhongyouzk.top

C#:   public static void F() {}
来源：http://zrt.gzhubu.top

[G09] 接口 / 抽象类
来源：http://pzw.ywan-chungtsiang.top

Py:   from abc import ABC, abstractmethod
来源：http://sbt.xingfuxueyuan.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://oji.tian-w.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rxa.iojbl.cn

TS:   interface Shape { area(): number; }
来源：http://vnn.guannengcc.top

Java: interface Shape { double area(); }
来源：http://cuj.xziqi.cn

Go:   type Shape interface { Area() float64 }
来源：http://xwx.xziqi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rnb.xinyue.icu

C#:   interface IShape { double Area(); }
来源：http://nbm.gaohongyu789.top

[G10] 访问控制
来源：http://dpp.nanxuanxn.top

Py:   约定 _protected / __private（不强制）
来源：http://ptw.316326.xyz

PHP:  public / protected / private
来源：http://vlv.shanyushiyangkeji.top

JS:   #private 字段；其余公开
来源：http://gfa.xylfe.cn

TS:   public / protected / private
来源：http://ern.zdqjudy.top

Java: public / protected / private / 默认包级
来源：http://dux.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://wdl.ywan-chungtsiang.top

Ruby: public / protected / private
来源：http://poc.zhongyouzk.top

C#:   public / protected / private / internal
来源：http://xci.hcnkem.com

[G11] getter / setter
来源：http://wyn.feifeiyinyue.top

Py:   @property 与 @x.setter
来源：http://pkm.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lia.xuetiantiany.cn

JS:   get name() { return this._name; }
来源：http://pqq.aizwys.cn

TS:   get name(): string { return this._name; }
来源：http://pec.xylfe.cn

Java: public String getName() { return name; }
来源：http://aif.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bme.hammf.cn

Ruby: attr_accessor :name
来源：http://jfq.yj202588.top

C#:   public string Name { get; set; }
来源：http://zeq.zhengqikj.top

[G12] 对象转字符串
来源：http://uzd.jqgfzy.top

Py:   def __str__(self): return self.name
来源：http://kca.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ntc.zhongyouzk.top

JS:   toString() { return this.name; }
来源：http://lsk.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://lkg.cqqwz.cn

Java: @Override public String toString() { return name; }
来源：http://ynr.cqqwz.cn

Go:   func (u User) String() string { return u.Name }
来源：http://udh.sxryk.cn

Ruby: def to_s; @name; end
来源：http://fad.iojbl.cn

C#:   public override string ToString() => Name;
来源：http://uvx.quarkkingdee.top

[G13] 判断对象类型
来源：http://hcx.snrcjt.cn

Py:   isinstance(u, User)
来源：http://yqs.birdmap.top

PHP:  $u instanceof User
来源：http://sdm.gogol.net.cn

JS:   u instanceof User
来源：http://qnn.zdbjq.cn

TS:   u instanceof User
来源：http://tcv.smart0.xyz

Java: u instanceof User
来源：http://cxx.jinyuanbaomall.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://acw.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://gsg.daria6918.cn

C#:   u is User
来源：http://fne.kuanghao11.cn

[G14] 数据类 / record
来源：http://oea.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lcw.gzhubu.top

PHP:  // 用 readonly 属性模拟
来源：http://kax.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://qmz.zdbjq.cn

TS:   type User = { name: string; age: number };
来源：http://cfg.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://lkr.fengsongda.top

Go:   type User struct { Name string; Age int }
来源：http://eoa.zhiwuduotai.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://upl.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://vrv.cheryme.top

[G15] 枚举
来源：http://wrz.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mwv.daxiang520.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://grf.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aoj.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vho.xziqi.cn

Java: enum Color { RED, GREEN }
来源：http://cac.mhx1999.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fqz.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://zzh.tian-w.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://woz.sjlbkw.cn

[G16] 对象转数组 / 字典
来源：http://dmx.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wge.sysykeji.top


<!-- 参考信息 -->
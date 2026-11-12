代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bbb.dianchejie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kcy.fehbvm.com

C#:   1234567.ToString("N0")
来源：http://ngy.ydzc1.top

[E17] 首字母大写
来源：http://lio.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tmj.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://kbs.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uar.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iwk.0kj1m.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://caz.cqqwz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fqd.ctjpmb.com

Ruby: s.capitalize
来源：http://dxi.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://meo.zhongyouzk.top

[E18] 模板占位符替换
来源：http://awk.gzhubu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wec.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xvk.hnxiangtu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hvs.xingfuxueyuan.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://kxo.shangyingyoupin.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lcj.feifeiyinyue.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lmj.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xqx.xylfe.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pxo.zycfv.cn

[E19] 多行文本按行拆分
来源：http://dju.gaohongyu789.top

Py:   s.splitlines()
来源：http://dna.hfpthk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lfr.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://oez.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://swf.zhiwuduotai.top

Java: s.lines().toList()
来源：http://dia.shangyingyoupin.top

Go:   strings.Split(s, "\n")
来源：http://pzi.dashuyun.cn

Ruby: s.lines
来源：http://ngz.feifeiyinyue.top

C#:   s.Split('\n')
来源：http://tyz.tanke756.top

[E20] 判断字符串是否为空
来源：http://avn.yfazqb.com

Py:   if not s:
来源：http://yfs.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zir.wangshuangyany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mgn.chenzaomai.com

TS:   if (s === "") {}
来源：http://syj.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://qwe.shzxlz.cn

Go:   if s == "" {}
来源：http://zbp.xingfuxueyuan.xyz

Ruby: if s.empty?
来源：http://rly.hammf.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tly.cheryme.top

[E21] 超长截断加省略号
来源：http://ncs.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iaq.ydjk.org.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vvl.zhoulong.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hfq.wangshuangyany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tqm.zhijiandao.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xrc.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://ofl.jyoumei.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mvb.xuanzx.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qog.tian-w.cn

[E22] 字节长度与字符长度
来源：http://flo.daxiang520.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jha.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ogb.yuanzhike.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uxy.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dyb.xingfuxueyuan.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dcq.feifeiyinyue.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lpv.jinghuilouyu.cn

Ruby: s.bytesize;  s.length
来源：http://ykw.shanyushiyangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vbe.9152youxi.cn

================================================================================
来源：http://ras.cucudq.cn

F. 文件与目录
来源：http://mtq.ybcxt.top

================================================================================
来源：http://otm.zhiwuduotai.top

[F01] 读取整个文件
来源：http://nwo.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ccc.epnwcf.com

PHP:  file_get_contents("a.txt");
来源：http://lzi.jlsjyb.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://beq.hnxiangtu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tjx.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://olx.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zge.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://xnr.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://bxs.zhengqikj.top

[F02] 逐行读取文件
来源：http://nut.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nno.guowangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ika.bbcook.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wzf.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ruu.xingfuxueyuan.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uob.vqdsnc.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tod.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://thh.hysaishi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lcf.yuxming.cn

[F03] 写入文件（覆盖）
来源：http://ppv.nanxinkj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ldm.meibo888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ulh.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nwv.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iwe.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ual.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pzm.ppjwa.cn

Ruby: File.write("a.txt", "hi")
来源：http://rri.quarkkingdee.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mnp.quarkkingdee.top

[F04] 追加写入文件
来源：http://rll.jinyuanbaomall.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fvi.zdbjq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pom.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pum.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://swg.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ixl.haohaochexian.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fev.jinqigfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ckq.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://edw.sweek.top

[F05] 判断文件或目录是否存在
来源：http://ffh.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zlp.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://tam.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://otc.pycfn.com

TS:   fs.existsSync("a.txt")
来源：http://qqx.xuetiantiany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://khe.ywan-chungtsiang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qxh.zhongyouzk.top

Ruby: File.exist?("a.txt")
来源：http://mun.hesvh.cn

C#:   File.Exists("a.txt")
来源：http://ylo.bjfxy.top

[F06] 删除文件
来源：http://grt.yfazqb.com

Py:   os.remove("a.txt")
来源：http://ube.fzhhl.top

PHP:  unlink("a.txt");
来源：http://idk.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://qbh.xuetiantiany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xvh.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zvu.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://rxe.sjlbkw.cn

Ruby: File.delete("a.txt")
来源：http://mct.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://ber.uphjek.com

[F07] 创建目录（含多级）
来源：http://fto.quarkkingdee.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zmq.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sss.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vky.shanyushiyangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zsn.haohaochexian.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cct.nanxuanxn.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cyo.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lxp.mhx1999.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ktc.hnxiangtu.top

[F08] 遍历目录
来源：http://xwl.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://umw.jinyuanbaomall.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yxk.fktsv.cn

JS:   fs.readdirSync("dir")
来源：http://ubj.hysaishi.cn

TS:   fs.readdirSync("dir")
来源：http://qqg.xuetiantiany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://btg.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ggl.yj20258888.top

Ruby: Dir.children("dir")
来源：http://bkr.zycfv.cn

C#:   Directory.GetFiles("dir")
来源：http://fgq.9152youxi.cn

[F09] 获取文件大小
来源：http://ivw.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://aat.yj20258.top

PHP:  filesize("a.txt");
来源：http://dgv.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://icz.hfpthk.cn

TS:   fs.statSync("a.txt").size
来源：http://amm.ydjk.org.cn

Java: Files.size(Path.of("a.txt"))
来源：http://esd.jiagoushi.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://emg.cdnleiting.top

Ruby: File.size("a.txt")
来源：http://paj.shuidangran.top

C#:   new FileInfo("a.txt").Length
来源：http://jlk.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://kkx.zhijiandao.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xas.tanke756.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://czq.fktsv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nud.meibo888.top

TS:   path.extname("a.txt")
来源：http://gzz.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sbr.svipenyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qqw.zhiwuduotai.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bix.sjlbkw.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ycl.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://jzd.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yji.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wsl.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ljj.andypj.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lwn.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mws.jianghu66.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bid.zdbjq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://amh.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ncw.zhoulong.xyz

[F12] CSV 读写
来源：http://ofi.jianghu66.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hfw.zhiwuduotai.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://shj.chenzaomai.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aku.ivvv.top

TS:   // 同上
来源：http://fkj.snrcjt.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ioy.xziqi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://saj.jiagoushi.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kom.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oqj.jinqigufen.top

================================================================================
来源：http://cot.nanxinkj.top

G. 面向对象
来源：http://bct.yongpay.top

================================================================================
来源：http://fjl.gogol.net.cn

[G01] 定义类
来源：http://pxv.gaohongyu789.top

Py:   class User: pass
来源：http://qpi.wangshuangyany.cn

PHP:  class User {}
来源：http://nng.cucudq.cn

JS:   class User {}
来源：http://vxq.gotoacloud.top

TS:   class User { name: string = ""; }
来源：http://aqz.jlsjyb.cn

Java: class User {}
来源：http://voi.cashguo.top

Go:   type User struct { Name string }
来源：http://mct.ydzc1.top

Ruby: class User; end
来源：http://qbb.sweek.top

C#:   class User {}
来源：http://hwe.shanyushiyangkeji.top

[G02] 构造函数
来源：http://uwv.ydzc1.top

Py:   def __init__(self, name): self.name = name
来源：http://wqm.hongshengwenyu.top

PHP:  public function __construct(public string $name) {}
来源：http://dvz.meibo888.top

JS:   constructor(name) { this.name = name; }
来源：http://ien.nanxinkj.top

TS:   constructor(public name: string) {}
来源：http://izh.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://dso.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aqz.ehwqpu.com

Ruby: def initialize(name); @name = name; end
来源：http://fwi.feifeiyinyue.top

C#:   public User(string name) { Name = name; }
来源：http://qrv.aizwys.cn

[G03] 实例属性
来源：http://oqo.zhaomingkeji.xyz

Py:   self.name = "x"
来源：http://gqj.hnxiangtu.top

PHP:  public string $name = "x";
来源：http://jgj.sweek.top

JS:   this.name = "x";
来源：http://jvs.jianghu66.top

TS:   name: string = "x";
来源：http://obb.sxryk.cn

Java: private String name;
来源：http://tnu.yanxiufei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kks.jlsjyb.cn

Ruby: @name = "x"
来源：http://oje.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://ccx.chenzaomai.com

[G04] 定义方法
来源：http://fyc.0kj1m.cn

Py:   def greet(self): return self.name
来源：http://bod.xuetiantiany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zvl.zhengqikj.top

JS:   greet() { return this.name; }
来源：http://vdz.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://nac.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://scs.zdqjudy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://whk.hnxiangtu.top

Ruby: def greet; @name; end
来源：http://xmb.tian-w.cn

C#:   public string Greet() => Name;
来源：http://mwn.yueranfly.top

[G05] 继承
来源：http://dox.fengsongda.top

Py:   class Admin(User): pass
来源：http://iax.yj20258888.top

PHP:  class Admin extends User {}
来源：http://cpu.ydzc1.top

JS:   class Admin extends User {}
来源：http://ypm.hesvh.cn

TS:   class Admin extends User {}
来源：http://qax.andypj.xyz

Java: class Admin extends User {}
来源：http://ezz.nanxinkj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vcv.hywenlv.cn

Ruby: class Admin < User; end
来源：http://rjr.hongshengwenyu.top

C#:   class Admin : User {}
来源：http://xew.cheryme.top

[G06] 重写方法
来源：http://iqg.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://oal.guannengcc.top

PHP:  public function greet(): string { return "admin"; }
来源：http://stl.0kj1m.cn

JS:   greet() { return "admin"; }
来源：http://rzx.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://fph.jinqigfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://tld.havefunace.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wfu.daxiang520.top

Ruby: def greet; "admin"; end
来源：http://rfy.meibo888.top

C#:   public override string Greet() => "admin";
来源：http://qad.wangdashe.top

[G07] 调用父类方法
来源：http://zzf.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://qru.ivvv.top

PHP:  parent::greet();
来源：http://zkh.ehwqpu.com

JS:   super.greet();
来源：http://nsj.fanxiaobao.xyz

TS:   super.greet();
来源：http://zbl.tanke756.top

Java: super.greet();
来源：http://tfo.jiagoushi.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vvh.chenjidiqi.icu

Ruby: super
来源：http://got.yonumen.top

C#:   base.Greet();
来源：http://uoh.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://rzb.meibo888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uhl.sufxvd.cn

PHP:  public static function f() {}
来源：http://dkm.xinyue.icu

JS:   static f() {}
来源：http://ief.hnqzz.top

TS:   static f(): void {}
来源：http://tqj.guowangkeji.top

Java: static void f() {}
来源：http://xku.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yrv.shangyingyoupin.top

Ruby: def self.f; end
来源：http://car.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://okf.sufxvd.cn

[G09] 接口 / 抽象类
来源：http://hsl.epnwcf.com

Py:   from abc import ABC, abstractmethod
来源：http://ohs.zhengqikj.top

PHP:  interface Shape { public function area(): float; }
来源：http://mpb.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rfu.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://tpp.jinyuanbaomall.cn

Java: interface Shape { double area(); }
来源：http://pzg.nanxuanxn.top

Go:   type Shape interface { Area() float64 }
来源：http://nrn.uphjek.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ggt.jinqigufen.top

C#:   interface IShape { double Area(); }
来源：http://gwq.jinqigfzy.top

[G10] 访问控制
来源：http://omy.uphjek.com

Py:   约定 _protected / __private（不强制）
来源：http://gox.meibo888.top

PHP:  public / protected / private
来源：http://bun.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://syd.fzhhl.top

TS:   public / protected / private
来源：http://red.shuidangran.top

Java: public / protected / private / 默认包级
来源：http://oya.cucudq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ngl.yanxiufei.cn

Ruby: public / protected / private
来源：http://yqc.guowangkeji.top

C#:   public / protected / private / internal
来源：http://ash.dianchejie.cn

[G11] getter / setter
来源：http://yfg.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://kwn.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lai.dashuyun.cn

JS:   get name() { return this._name; }
来源：http://pnv.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://ttz.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://lal.nwbrower.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://htc.gogol.net.cn

Ruby: attr_accessor :name
来源：http://kli.xuanzx.com

C#:   public string Name { get; set; }
来源：http://nzp.dianchejie.cn

[G12] 对象转字符串
来源：http://nke.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://ixp.aizwys.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fji.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://mci.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://toi.cheryme.top

Java: @Override public String toString() { return name; }
来源：http://ekq.ybcxt.top

Go:   func (u User) String() string { return u.Name }
来源：http://ujk.shuidangran.top

Ruby: def to_s; @name; end
来源：http://let.yj20258.top

C#:   public override string ToString() => Name;
来源：http://cbo.chenlongwang.top

[G13] 判断对象类型
来源：http://xeh.yfazqb.com

Py:   isinstance(u, User)
来源：http://xny.ivvv.top

PHP:  $u instanceof User
来源：http://opd.yangfankeji.com

JS:   u instanceof User
来源：http://wzf.mhx1999.top

TS:   u instanceof User
来源：http://ydq.xziqi.cn

Java: u instanceof User
来源：http://znb.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://iuj.yanxiufei.cn

Ruby: u.is_a?(User)
来源：http://enj.ywan-chungtsiang.top

C#:   u is User
来源：http://pct.ivvv.top

[G14] 数据类 / record
来源：http://pxa.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oun.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://mjy.wangdashe.top

JS:   // 无内置：普通类或对象字面量
来源：http://vgz.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://psd.tian-w.cn

Java: record User(String name, int age) {}
来源：http://kbz.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://kgk.birdmap.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sft.tanke756.top

C#:   record User(string Name, int Age);
来源：http://lld.hfpthk.cn

[G15] 枚举
来源：http://snt.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ktv.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gmj.iojbl.cn


<!-- 参考信息 -->
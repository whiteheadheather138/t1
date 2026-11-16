代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mci.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cqp.zhengqikj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://shf.tanke756.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zlh.zycfv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lsf.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tbu.xinyue.icu

[E16] 数字千分位
来源：http://iti.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://vrc.zhaomingkeji.xyz

PHP:  number_format(1234567);
来源：http://hrn.yj20258.top

JS:   (1234567).toLocaleString("en-US")
来源：http://yyt.guowangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rml.quarkkingdee.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ypo.nanxinkj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zhy.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wnv.zhaomingkeji.xyz

C#:   1234567.ToString("N0")
来源：http://fdo.ydjk.org.cn

[E17] 首字母大写
来源：http://kzw.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ovz.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fbe.gzhubu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ddr.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yjn.zhongyouzk.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bpw.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jap.snrcjt.cn

Ruby: s.capitalize
来源：http://edg.jinyuanbaomall.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hjp.vehdjk.com

[E18] 模板占位符替换
来源：http://xin.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rbv.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fjb.xziqi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qip.cucudq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xlu.bjfxy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://swc.quarkkingdee.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ntn.mhx1999.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://znq.mhx1999.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lld.uphjek.com

[E19] 多行文本按行拆分
来源：http://qxq.xinyue.icu

Py:   s.splitlines()
来源：http://kaz.xuetiantiany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qyd.xuetiantiany.cn

JS:   s.split(/\r?\n/)
来源：http://wmp.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://wlw.gogol.net.cn

Java: s.lines().toList()
来源：http://pgx.mhx1999.top

Go:   strings.Split(s, "\n")
来源：http://wzf.jiagoushi.top

Ruby: s.lines
来源：http://naw.zdbjq.cn

C#:   s.Split('\n')
来源：http://htt.c1oappe.top

[E20] 判断字符串是否为空
来源：http://ifh.yanxiufei.cn

Py:   if not s:
来源：http://ztv.cheryme.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nxs.hywenlv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dxc.dashuyun.cn

TS:   if (s === "") {}
来源：http://vbd.guannengcc.top

Java: if (s.isEmpty()) {}
来源：http://rod.hcnkem.com

Go:   if s == "" {}
来源：http://gac.xuanzx.com

Ruby: if s.empty?
来源：http://cqk.ctjpmb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://faa.andypj.xyz

[E21] 超长截断加省略号
来源：http://juh.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gqu.birdmap.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kia.ybcxt.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://thl.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jjs.daxiang520.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xjp.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://gct.zhengqikj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://boc.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ghm.ehwqpu.com

[E22] 字节长度与字符长度
来源：http://bju.xinyue.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ebg.cqqwz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dmf.wangshuangyany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://chs.zhoulong.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qfv.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gsa.jqgfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zgh.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://hle.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uif.tarul.cn

================================================================================
来源：http://qzb.jqgufenzy.top

F. 文件与目录
来源：http://oay.fanxiaobao.xyz

================================================================================
来源：http://fcm.zhaomingkeji.xyz

[F01] 读取整个文件
来源：http://gla.yanxiufei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fgb.cucudq.cn

PHP:  file_get_contents("a.txt");
来源：http://tme.snrcjt.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wcy.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://php.ctjpmb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://nfz.zhiwuduotai.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wub.cdnleiting.top

Ruby: File.read("a.txt")
来源：http://iwy.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://gyo.xuetiantiany.cn

[F02] 逐行读取文件
来源：http://bjr.chenjidiqi.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bfn.chenjidiqi.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oly.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jry.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zgi.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cib.ctjpmb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ngc.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://omd.jyoumei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://usv.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://knc.tian-w.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hhk.xuanzx.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://jwz.wangdashe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uqs.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eig.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mwb.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zuu.ywan-chungtsiang.top

Ruby: File.write("a.txt", "hi")
来源：http://lcr.iojbl.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rtw.svipenyu.cn

[F04] 追加写入文件
来源：http://pqs.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vtt.guowangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kbm.zhaomingkeji.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kjm.hnxiangtu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vwf.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wej.jinghuilouyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qti.ydzc1.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://emn.sjlbkw.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iok.uphjek.com

[F05] 判断文件或目录是否存在
来源：http://jjm.feifeiyinyue.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rsc.yuanzhike.top

PHP:  file_exists("a.txt");
来源：http://zqf.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://vtq.ydzc1.top

TS:   fs.existsSync("a.txt")
来源：http://awo.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://bfd.c1oappe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dhr.shanyushiyangtech.top

Ruby: File.exist?("a.txt")
来源：http://dxp.jqgfzy.top

C#:   File.Exists("a.txt")
来源：http://rtm.shanyushiyangkeji.top

[F06] 删除文件
来源：http://ruf.jinqigufen.top

Py:   os.remove("a.txt")
来源：http://nux.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://sjz.xuetiantiany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://psi.zhijiandao.cn

TS:   fs.unlinkSync("a.txt")
来源：http://giq.nanxinkj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dhj.havefunace.top

Go:   os.Remove("a.txt")
来源：http://bmk.tianlin.xyz

Ruby: File.delete("a.txt")
来源：http://mvu.havefunace.top

C#:   File.Delete("a.txt");
来源：http://xlp.yj20258.top

[F07] 创建目录（含多级）
来源：http://hir.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xpz.yuxming.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rsm.yj202588.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://khn.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jcb.zdqjudy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hlp.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oii.fengsongda.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://puf.hammf.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jby.yongpay.top

[F08] 遍历目录
来源：http://swq.guowangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://flh.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yha.vqdsnc.cn

JS:   fs.readdirSync("dir")
来源：http://ola.snrcjt.cn

TS:   fs.readdirSync("dir")
来源：http://bos.kuanghao11.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qdc.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fvb.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://qij.xinyue.icu

C#:   Directory.GetFiles("dir")
来源：http://zoe.zhaomingkeji.xyz

[F09] 获取文件大小
来源：http://trl.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://umq.jiagoushi.top

PHP:  filesize("a.txt");
来源：http://gln.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://arx.kuanghao11.cn

TS:   fs.statSync("a.txt").size
来源：http://raw.vehdjk.com

Java: Files.size(Path.of("a.txt"))
来源：http://qgv.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fvn.52xcode.cn

Ruby: File.size("a.txt")
来源：http://mws.smart0.xyz

C#:   new FileInfo("a.txt").Length
来源：http://ues.zdqjudy.top

[F10] 取文件扩展名 / 文件名
来源：http://uek.hywenlv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vfj.fehbvm.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sbc.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uez.shanyushiyangkeji.top

TS:   path.extname("a.txt")
来源：http://xxj.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pwh.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://efz.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://phl.zhijiandao.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://llq.fengsongda.top

[F11] 复制与移动文件
来源：http://ugm.nwbrower.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mse.hesvh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bdb.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zcu.xinyue.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jml.vehdjk.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hqs.c1oappe.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hli.sysykeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rtl.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mui.cdnleiting.top

[F12] CSV 读写
来源：http://kqh.fktsv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rxf.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mat.shzxlz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cbi.fanxiaobao.xyz

TS:   // 同上
来源：http://kba.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jme.yvedp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fhi.shangyingyoupin.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ccw.sweek.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fmn.zdqjudy.top

================================================================================
来源：http://bhb.sufxvd.cn

G. 面向对象
来源：http://cyr.mhx1999.top

================================================================================
来源：http://fxp.yj20258888.top

[G01] 定义类
来源：http://qcf.nanxinkj.top

Py:   class User: pass
来源：http://one.mhx1999.top

PHP:  class User {}
来源：http://oxr.316326.xyz

JS:   class User {}
来源：http://fgn.hesvh.cn

TS:   class User { name: string = ""; }
来源：http://bxz.zdqjudy.top

Java: class User {}
来源：http://lnx.ctjpmb.com

Go:   type User struct { Name string }
来源：http://sjr.chenzaomai.com

Ruby: class User; end
来源：http://prs.sxryk.cn

C#:   class User {}
来源：http://kqf.smart0.xyz

[G02] 构造函数
来源：http://gdb.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://qxl.jinghuilouyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://wnt.kuanghao11.cn

JS:   constructor(name) { this.name = name; }
来源：http://glr.nanxinkj.top

TS:   constructor(public name: string) {}
来源：http://kjc.gzhubu.top

Java: User(String name) { this.name = name; }
来源：http://mfo.tarul.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lie.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://xyd.vehdjk.com

C#:   public User(string name) { Name = name; }
来源：http://yhl.andypj.xyz

[G03] 实例属性
来源：http://dlq.redwolf501.top

Py:   self.name = "x"
来源：http://dnk.xinyue.icu

PHP:  public string $name = "x";
来源：http://gzz.ehwqpu.com

JS:   this.name = "x";
来源：http://byi.jinqigufen.top

TS:   name: string = "x";
来源：http://vkp.quarkkingdee.top

Java: private String name;
来源：http://zad.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://otr.birdmap.top

Ruby: @name = "x"
来源：http://him.52xcode.cn

C#:   public string Name { get; set; } = "x";
来源：http://mzb.aizwys.cn

[G04] 定义方法
来源：http://eou.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://zgm.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ugd.jinyuanbaomall.cn

JS:   greet() { return this.name; }
来源：http://fdu.ivvv.top

TS:   greet(): string { return this.name; }
来源：http://hgq.kuanghao11.cn

Java: String greet() { return name; }
来源：http://zzu.sjlbkw.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wvw.jqgfzy.top

Ruby: def greet; @name; end
来源：http://spu.yvedp.cn

C#:   public string Greet() => Name;
来源：http://vdn.hcnkem.com

[G05] 继承
来源：http://pzv.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://ibs.yj202588.top

PHP:  class Admin extends User {}
来源：http://miv.zdbjq.cn

JS:   class Admin extends User {}
来源：http://hpo.jianghu66.top

TS:   class Admin extends User {}
来源：http://ych.uphjek.com

Java: class Admin extends User {}
来源：http://gkl.sysykeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wyl.andypj.xyz

Ruby: class Admin < User; end
来源：http://onc.xziqi.cn

C#:   class Admin : User {}
来源：http://rlt.c1oappe.top

[G06] 重写方法
来源：http://pur.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://raj.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ujz.xinyue.icu

JS:   greet() { return "admin"; }
来源：http://tbq.jlsjyb.cn

TS:   greet(): string { return "admin"; }
来源：http://iod.bjfxy.top

Java: @Override String greet() { return "admin"; }
来源：http://ccs.birdmap.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tcn.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://eht.sufxvd.cn

C#:   public override string Greet() => "admin";
来源：http://lgt.zhixingplan.top

[G07] 调用父类方法
来源：http://ygg.sxryk.cn

Py:   super().greet()
来源：http://fcr.cdnleiting.top

PHP:  parent::greet();
来源：http://hpn.yonumen.top

JS:   super.greet();
来源：http://naf.yueranfly.top

TS:   super.greet();
来源：http://blb.zhaomingkeji.xyz

Java: super.greet();
来源：http://hqi.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kim.dianchejie.cn

Ruby: super
来源：http://acc.yvedp.cn

C#:   base.Greet();
来源：http://uzp.ivvv.top

[G08] 静态方法与属性
来源：http://wil.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rqu.sufxvd.cn

PHP:  public static function f() {}
来源：http://vyn.hcnkem.com

JS:   static f() {}
来源：http://zmh.yvedp.cn

TS:   static f(): void {}
来源：http://idp.cheryme.top

Java: static void f() {}
来源：http://zdw.vqdsnc.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://iqt.hywenlv.cn

Ruby: def self.f; end
来源：http://xmx.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://fss.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://kuv.epnwcf.com

Py:   from abc import ABC, abstractmethod
来源：http://inu.tianlin.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://bep.vqdsnc.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://iej.shuidangran.top

TS:   interface Shape { area(): number; }
来源：http://dml.xingfuxueyuan.xyz

Java: interface Shape { double area(); }
来源：http://ydw.bbcook.cn

Go:   type Shape interface { Area() float64 }
来源：http://aib.ppjwa.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jbh.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://zqz.guannengcc.top

[G10] 访问控制
来源：http://gqk.hnqzz.top

Py:   约定 _protected / __private（不强制）
来源：http://nfj.cucudq.cn

PHP:  public / protected / private
来源：http://azr.fzhhl.top

JS:   #private 字段；其余公开
来源：http://mpt.zhijiandao.cn

TS:   public / protected / private
来源：http://rml.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://eyi.ehwqpu.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://zks.haohaochexian.top

Ruby: public / protected / private
来源：http://ffq.aibaodan.cn

C#:   public / protected / private / internal
来源：http://rzg.jinyuanbaomall.cn

[G11] getter / setter
来源：http://fao.epnwcf.com

Py:   @property 与 @x.setter
来源：http://sci.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zxq.kuanghao11.cn

JS:   get name() { return this._name; }
来源：http://bdy.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://pax.bjfxy.top

Java: public String getName() { return name; }
来源：http://can.9152youxi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hxh.sxryk.cn

Ruby: attr_accessor :name
来源：http://pvk.zhaomingkeji.xyz

C#:   public string Name { get; set; }
来源：http://fur.xziqi.cn

[G12] 对象转字符串
来源：http://rwp.tanke756.top

Py:   def __str__(self): return self.name
来源：http://ouq.iojbl.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qcb.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://wqy.yj202588.top

TS:   toString(): string { return this.name; }
来源：http://rzi.zycfv.cn

Java: @Override public String toString() { return name; }
来源：http://kge.sxryk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://syr.jyoumei.cn

Ruby: def to_s; @name; end
来源：http://clo.shuidangran.top

C#:   public override string ToString() => Name;
来源：http://udj.jlsjyb.cn

[G13] 判断对象类型
来源：http://bwy.ybcxt.top

Py:   isinstance(u, User)
来源：http://wpe.xuetiantiany.cn

PHP:  $u instanceof User
来源：http://dfa.smart0.xyz

JS:   u instanceof User
来源：http://ixi.ehwqpu.com

TS:   u instanceof User
来源：http://kca.zhijiandao.cn

Java: u instanceof User
来源：http://tsc.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://siq.xinyue.icu

Ruby: u.is_a?(User)
来源：http://ayo.hongshengwenyu.top

C#:   u is User
来源：http://olx.0kj1m.cn


<!-- 参考信息 -->
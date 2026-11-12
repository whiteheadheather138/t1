代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qgb.kuanghao11.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lmk.ydjk.org.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rxc.haohaochexian.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ssj.ydjk.org.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://trc.epnwcf.com

[E15] HTML 转义 / 反转义
来源：http://kxz.birdmap.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mqv.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://msv.jlsjyb.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://azh.mhx1999.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ytj.hysaishi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xgv.wangshuangyany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nul.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jyd.zhijiandao.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qub.meibo888.top

[E16] 数字千分位
来源：http://ocw.hnxiangtu.top

Py:   f"{1234567:,}"
来源：http://zhj.yfazqb.com

PHP:  number_format(1234567);
来源：http://rvv.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://kkh.haohaochexian.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fck.ybcxt.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tqf.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fjc.chenlongwang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://elg.iojbl.cn

C#:   1234567.ToString("N0")
来源：http://bov.cdnleiting.top

[E17] 首字母大写
来源：http://syn.zhaomingkeji.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://chu.wangshuangyany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dgh.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lyo.nwbrower.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ddf.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jmh.cqqwz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xdk.vqdsnc.cn

Ruby: s.capitalize
来源：http://mla.hesvh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vno.yj20258888.top

[E18] 模板占位符替换
来源：http://nis.gaohongyu789.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://szt.jinyuanbaomall.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zlg.kuanghao11.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zfz.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bzg.wangdashe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vwd.zhijiandao.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pxu.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xvr.wangdashe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cwe.guowangkeji.top

[E19] 多行文本按行拆分
来源：http://ght.ydzc1.top

Py:   s.splitlines()
来源：http://btj.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ryg.vqdsnc.cn

JS:   s.split(/\r?\n/)
来源：http://rmj.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://nkw.shangyingyoupin.top

Java: s.lines().toList()
来源：http://bof.sufxvd.cn

Go:   strings.Split(s, "\n")
来源：http://oao.ywan-chungtsiang.top

Ruby: s.lines
来源：http://kkg.hesvh.cn

C#:   s.Split('\n')
来源：http://ipp.fzhhl.top

[E20] 判断字符串是否为空
来源：http://ctn.shanyushiyangkeji.top

Py:   if not s:
来源：http://cdz.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qwh.hammf.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iie.pengpengdd.cyou

TS:   if (s === "") {}
来源：http://sht.tian-w.cn

Java: if (s.isEmpty()) {}
来源：http://mvs.ehwqpu.com

Go:   if s == "" {}
来源：http://iqo.yueranfly.top

Ruby: if s.empty?
来源：http://mxg.yj202588.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bpa.yongpay.top

[E21] 超长截断加省略号
来源：http://plb.pycfn.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pcc.hcnkem.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://svr.0kj1m.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://grn.pengpengdd.cyou

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mbd.ybcxt.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bfk.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://mew.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hwa.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iih.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://kjz.nanxuanxn.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://avl.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ctx.bbcook.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wry.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hzg.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fjt.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wcf.tarul.cn

Ruby: s.bytesize;  s.length
来源：http://esr.dashuyun.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wau.meibo888.top

================================================================================
来源：http://gdg.cdnleiting.top

F. 文件与目录
来源：http://vpu.c1oappe.top

================================================================================
来源：http://bjv.zhengqikj.top

[F01] 读取整个文件
来源：http://yit.aibaodan.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nuh.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://puf.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jef.nanxuanxn.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ytu.quarkkingdee.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ewq.tarul.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tcx.316326.xyz

Ruby: File.read("a.txt")
来源：http://gao.zdbjq.cn

C#:   File.ReadAllText("a.txt");
来源：http://vdi.yongpay.top

[F02] 逐行读取文件
来源：http://tqq.yj20258888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ega.nanxinkj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xcy.jinqigufen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mby.fanxiaobao.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sjr.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ewc.meibo888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://apz.gotoacloud.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ysj.ctjpmb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jns.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://zdg.ivvv.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rlr.yfazqb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://dnn.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://acl.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wos.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://prp.yj20258.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nuh.epnwcf.com

Ruby: File.write("a.txt", "hi")
来源：http://zgm.zhiwuduotai.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rgt.ppjwa.cn

[F04] 追加写入文件
来源：http://ony.cashguo.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://swd.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bod.shanyushiyangtech.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fan.jianghu66.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rui.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qoo.52xcode.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xrb.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://giv.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qdz.shanyushiyangkeji.top

[F05] 判断文件或目录是否存在
来源：http://xou.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://diy.wangdashe.top

PHP:  file_exists("a.txt");
来源：http://ekm.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://bbg.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://gyv.jinqigufen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rwc.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vle.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://wnv.fengsongda.top

C#:   File.Exists("a.txt")
来源：http://jlo.guowangkeji.top

[F06] 删除文件
来源：http://smp.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://ypx.tarul.cn

PHP:  unlink("a.txt");
来源：http://zrp.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rbi.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://zjf.havefunace.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://djr.jinqigufen.top

Go:   os.Remove("a.txt")
来源：http://cds.yj202588.top

Ruby: File.delete("a.txt")
来源：http://tfn.shangyingyoupin.top

C#:   File.Delete("a.txt");
来源：http://hpa.yongpay.top

[F07] 创建目录（含多级）
来源：http://tnp.shangyingyoupin.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mjw.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ciu.yueranfly.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ovg.iojbl.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xav.hfpthk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yrd.ppjwa.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qxy.ppjwa.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nhw.fktsv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://plp.ppjwa.cn

[F08] 遍历目录
来源：http://jhu.sufxvd.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vvj.yfazqb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pgw.hammf.cn

JS:   fs.readdirSync("dir")
来源：http://wpz.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://hbr.ydjk.org.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qqk.hywenlv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ojz.tian-w.cn

Ruby: Dir.children("dir")
来源：http://jhe.gogol.net.cn

C#:   Directory.GetFiles("dir")
来源：http://ytg.wangshuangyany.cn

[F09] 获取文件大小
来源：http://vel.shuidangran.top

Py:   os.path.getsize("a.txt")
来源：http://gxx.fzhhl.top

PHP:  filesize("a.txt");
来源：http://wzc.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://ntf.yj20258888.top

TS:   fs.statSync("a.txt").size
来源：http://vop.pengpengdd.cyou

Java: Files.size(Path.of("a.txt"))
来源：http://ctp.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fdd.yangfankeji.com

Ruby: File.size("a.txt")
来源：http://ydm.hesvh.cn

C#:   new FileInfo("a.txt").Length
来源：http://mhy.cashguo.top

[F10] 取文件扩展名 / 文件名
来源：http://mjy.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lbt.tanke756.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pdg.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zcw.fktsv.cn

TS:   path.extname("a.txt")
来源：http://rzf.ydjk.org.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ilt.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tkv.zhoulong.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://son.hcnkem.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eyf.xuanzx.com

[F11] 复制与移动文件
来源：http://acr.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dpd.aizwys.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vhy.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bqo.sweek.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fgf.ydjk.org.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sui.guowangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ihr.yonumen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uif.shanyushiyangtech.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wae.redwolf501.top

[F12] CSV 读写
来源：http://cbd.hammf.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://awy.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nrb.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bld.svipenyu.cn

TS:   // 同上
来源：http://oea.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gjf.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cbs.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://coq.wangshuangyany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yvv.zhiwuduotai.top

================================================================================
来源：http://ezc.zycfv.cn

G. 面向对象
来源：http://qct.daxiang520.top

================================================================================
来源：http://mfd.jqgufenzy.top

[G01] 定义类
来源：http://dwy.nwbrower.top

Py:   class User: pass
来源：http://qjr.ybcxt.top

PHP:  class User {}
来源：http://fsj.quarkkingdee.top

JS:   class User {}
来源：http://jyt.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://ozb.guannengcc.top

Java: class User {}
来源：http://euo.zhixingplan.top

Go:   type User struct { Name string }
来源：http://siu.pycfn.com

Ruby: class User; end
来源：http://lrq.sjlbkw.cn

C#:   class User {}
来源：http://ouj.zhoulong.xyz

[G02] 构造函数
来源：http://egi.gzhubu.top

Py:   def __init__(self, name): self.name = name
来源：http://fzc.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://nyw.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://zpy.aibaodan.cn

TS:   constructor(public name: string) {}
来源：http://mgp.jinyuanbaomall.cn

Java: User(String name) { this.name = name; }
来源：http://nwb.jqgufenzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xie.vqdsnc.cn

Ruby: def initialize(name); @name = name; end
来源：http://qtz.ydzc1.top

C#:   public User(string name) { Name = name; }
来源：http://fsb.gaohongyu789.top

[G03] 实例属性
来源：http://ser.vqdsnc.cn

Py:   self.name = "x"
来源：http://nkj.hywenlv.cn

PHP:  public string $name = "x";
来源：http://vqg.yongpay.top

JS:   this.name = "x";
来源：http://ceo.shzxlz.cn

TS:   name: string = "x";
来源：http://dni.zhiwuduotai.top

Java: private String name;
来源：http://ype.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vhf.fehbvm.com

Ruby: @name = "x"
来源：http://qzf.hesvh.cn

C#:   public string Name { get; set; } = "x";
来源：http://vbq.gotoacloud.top

[G04] 定义方法
来源：http://kok.bbcook.cn

Py:   def greet(self): return self.name
来源：http://bsk.chenlongwang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fyq.ctjpmb.com

JS:   greet() { return this.name; }
来源：http://orc.cheryme.top

TS:   greet(): string { return this.name; }
来源：http://ofw.pengpengdd.cyou

Java: String greet() { return name; }
来源：http://due.ehwqpu.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://hjb.jqgufenzy.top

Ruby: def greet; @name; end
来源：http://iov.andypj.xyz

C#:   public string Greet() => Name;
来源：http://tbo.tarul.cn

[G05] 继承
来源：http://zqo.mhx1999.top

Py:   class Admin(User): pass
来源：http://sui.gaohongyu789.top

PHP:  class Admin extends User {}
来源：http://mxj.pengpengdd.cyou

JS:   class Admin extends User {}
来源：http://ivt.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://fko.zhiwuduotai.top

Java: class Admin extends User {}
来源：http://dgp.yongpay.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sho.ehwqpu.com

Ruby: class Admin < User; end
来源：http://bhg.quarkkingdee.top

C#:   class Admin : User {}
来源：http://zfs.cheryme.top

[G06] 重写方法
来源：http://pfb.cheryme.top

Py:   def greet(self): return "admin"
来源：http://lxl.meibo888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dzf.52xcode.cn

JS:   greet() { return "admin"; }
来源：http://wpk.zdbjq.cn

TS:   greet(): string { return "admin"; }
来源：http://zxu.xingfuxueyuan.xyz

Java: @Override String greet() { return "admin"; }
来源：http://fgx.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qaz.fzhhl.top

Ruby: def greet; "admin"; end
来源：http://lee.hesvh.cn

C#:   public override string Greet() => "admin";
来源：http://bmy.c1oappe.top

[G07] 调用父类方法
来源：http://qgh.nwbrower.top

Py:   super().greet()
来源：http://jfj.pengpengdd.cyou

PHP:  parent::greet();
来源：http://skf.jinqigufen.top

JS:   super.greet();
来源：http://nsl.sxryk.cn

TS:   super.greet();
来源：http://dul.guowangkeji.top

Java: super.greet();
来源：http://fmi.zhixingplan.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ock.gogol.net.cn

Ruby: super
来源：http://xxs.guowangkeji.top

C#:   base.Greet();
来源：http://ddm.pengpengdd.cyou

[G08] 静态方法与属性
来源：http://cjd.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fnl.zhijiandao.cn

PHP:  public static function f() {}
来源：http://ixl.daria6918.cn

JS:   static f() {}
来源：http://yxl.bjfxy.top

TS:   static f(): void {}
来源：http://vhv.yfazqb.com

Java: static void f() {}
来源：http://xrj.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://jya.fktsv.cn

Ruby: def self.f; end
来源：http://czr.vqdsnc.cn

C#:   public static void F() {}
来源：http://yrz.havefunace.top

[G09] 接口 / 抽象类
来源：http://sbc.jyoumei.cn

Py:   from abc import ABC, abstractmethod
来源：http://tbf.yj20258888.top

PHP:  interface Shape { public function area(): float; }
来源：http://rys.xuanzx.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://zwo.wangdashe.top

TS:   interface Shape { area(): number; }
来源：http://gpo.zhijiandao.cn

Java: interface Shape { double area(); }
来源：http://bmx.tianlin.xyz

Go:   type Shape interface { Area() float64 }
来源：http://rdc.nwbrower.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jml.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://vdu.guannengcc.top

[G10] 访问控制
来源：http://xva.zhaomingkeji.xyz

Py:   约定 _protected / __private（不强制）
来源：http://vkl.sysykeji.top

PHP:  public / protected / private
来源：http://ohj.gaohongyu789.top

JS:   #private 字段；其余公开
来源：http://mjj.hongshengwenyu.top

TS:   public / protected / private
来源：http://vjb.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://msh.aibaodan.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tip.yj20258.top

Ruby: public / protected / private
来源：http://lds.hcnkem.com

C#:   public / protected / private / internal
来源：http://hse.jqgufenzy.top

[G11] getter / setter
来源：http://bga.yj20258888.top

Py:   @property 与 @x.setter
来源：http://ekl.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fpu.nanxuanxn.top

JS:   get name() { return this._name; }
来源：http://kvr.andypj.xyz

TS:   get name(): string { return this._name; }
来源：http://zho.vqdsnc.cn

Java: public String getName() { return name; }
来源：http://jtt.xziqi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://oke.smart0.xyz

Ruby: attr_accessor :name
来源：http://mlm.xuanzx.com

C#:   public string Name { get; set; }
来源：http://fel.hcnkem.com

[G12] 对象转字符串
来源：http://fqg.xuetiantiany.cn

Py:   def __str__(self): return self.name
来源：http://efq.yonumen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yen.zdqjudy.top

JS:   toString() { return this.name; }
来源：http://cbh.hfpthk.cn

TS:   toString(): string { return this.name; }
来源：http://rkt.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://ryn.zhaomingkeji.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://qck.cheryme.top

Ruby: def to_s; @name; end
来源：http://qht.ehwqpu.com

C#:   public override string ToString() => Name;
来源：http://uzs.ivvv.top

[G13] 判断对象类型
来源：http://bmy.chenlongwang.top


<!-- 参考信息 -->
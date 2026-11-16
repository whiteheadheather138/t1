代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mzz.9152youxi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ybp.fengsongda.top

Ruby: s.each_char { |ch| puts ch }
来源：http://got.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zjy.c1oappe.top

[E14] URL 编码与 Base64
来源：http://rui.yongpay.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yxt.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cbr.daria6918.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wbk.wangdashe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://scx.tianlin.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qvu.yangfankeji.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uve.tanke756.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://apz.zhoulong.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://icu.ydjk.org.cn

[E15] HTML 转义 / 反转义
来源：http://yeu.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://ysk.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rlk.zhoulong.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vef.pycfn.com

TS:   // 同上，务必做 XSS 过滤
来源：http://yjn.shuidangran.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gdl.yanxiufei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qvo.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wgk.zhoulong.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nmx.tarul.cn

[E16] 数字千分位
来源：http://qvg.xuanzx.com

Py:   f"{1234567:,}"
来源：http://sgu.jlsjyb.cn

PHP:  number_format(1234567);
来源：http://kts.zhoulong.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://zuu.cqqwz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zbe.hywenlv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tmp.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dzz.chenjidiqi.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zka.tarul.cn

C#:   1234567.ToString("N0")
来源：http://glx.jyoumei.cn

[E17] 首字母大写
来源：http://upl.cdnleiting.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://itp.mhx1999.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mzo.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mci.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uqy.c1oappe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hqt.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bhx.dashuyun.cn

Ruby: s.capitalize
来源：http://jlb.jqgufenzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vql.sufxvd.cn

[E18] 模板占位符替换
来源：http://wrl.jqgfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ugv.shzxlz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uiw.52xcode.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wpf.yangfankeji.com

TS:   tpl.replaceAll("{name}", name)
来源：http://szh.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rfy.gogol.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yfm.gaohongyu789.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vmw.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xnk.zhijiandao.cn

[E19] 多行文本按行拆分
来源：http://ooi.andypj.xyz

Py:   s.splitlines()
来源：http://jwj.sysykeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zpr.xylfe.cn

JS:   s.split(/\r?\n/)
来源：http://pgw.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://mmu.uphjek.com

Java: s.lines().toList()
来源：http://cwy.xziqi.cn

Go:   strings.Split(s, "\n")
来源：http://vej.guannengcc.top

Ruby: s.lines
来源：http://txq.tian-w.cn

C#:   s.Split('\n')
来源：http://tys.jlsjyb.cn

[E20] 判断字符串是否为空
来源：http://qus.yanxiufei.cn

Py:   if not s:
来源：http://yhm.jinyuanbaomall.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ohj.sysykeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tow.guannengcc.top

TS:   if (s === "") {}
来源：http://mln.ydjk.org.cn

Java: if (s.isEmpty()) {}
来源：http://ewh.zhijiandao.cn

Go:   if s == "" {}
来源：http://ojr.yj202588.top

Ruby: if s.empty?
来源：http://xez.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cpk.sufxvd.cn

[E21] 超长截断加省略号
来源：http://gni.9152youxi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://acf.ydjk.org.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lzb.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wlw.jyoumei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qyw.yanxiufei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rsl.hnxiangtu.top

Go:   // 按 rune 判断长度后截断
来源：http://lgy.yuanzhike.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pwq.tian-w.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xnm.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://oak.wangdashe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jmk.yanxiufei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vcc.tianlin.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mrd.gogol.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gtv.guowangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hdz.ehwqpu.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yeh.gotoacloud.top

Ruby: s.bytesize;  s.length
来源：http://mpm.sjlbkw.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mct.wangshuangyany.cn

================================================================================
来源：http://six.zhongyouzk.top

F. 文件与目录
来源：http://vid.ydzc1.top

================================================================================
来源：http://oij.xuanzx.com

[F01] 读取整个文件
来源：http://zig.ywan-chungtsiang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mnp.ywan-chungtsiang.top

PHP:  file_get_contents("a.txt");
来源：http://fcc.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ffb.sxryk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lhf.bjfxy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jxg.yonumen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gwe.bbcook.cn

Ruby: File.read("a.txt")
来源：http://ksw.ppjwa.cn

C#:   File.ReadAllText("a.txt");
来源：http://uap.dashuyun.cn

[F02] 逐行读取文件
来源：http://own.jinqigufen.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oil.jianghu66.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://svn.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bsf.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wef.cdnleiting.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sxr.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://adz.aibaodan.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vyw.sweek.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://whz.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://sxw.shangyingyoupin.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vee.birdmap.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tlt.shanyushiyangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yap.ctjpmb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://twx.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cxg.vehdjk.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://usv.ehwqpu.com

Ruby: File.write("a.txt", "hi")
来源：http://fen.quarkkingdee.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ckh.dashuyun.cn

[F04] 追加写入文件
来源：http://vtn.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://egu.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rbd.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qyc.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pde.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wql.gzhubu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lcp.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wox.nanxuanxn.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yor.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://vph.feifeiyinyue.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eid.yj20258.top

PHP:  file_exists("a.txt");
来源：http://cjn.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://zso.yueranfly.top

TS:   fs.existsSync("a.txt")
来源：http://xwh.sufxvd.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tzh.c1oappe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ykp.gotoacloud.top

Ruby: File.exist?("a.txt")
来源：http://fjc.316326.xyz

C#:   File.Exists("a.txt")
来源：http://ile.kuanghao11.cn

[F06] 删除文件
来源：http://wdb.iojbl.cn

Py:   os.remove("a.txt")
来源：http://sbj.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://jne.bjfxy.top

JS:   fs.unlinkSync("a.txt")
来源：http://vwe.wangdashe.top

TS:   fs.unlinkSync("a.txt")
来源：http://xyp.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xxv.yj20258888.top

Go:   os.Remove("a.txt")
来源：http://bkn.316326.xyz

Ruby: File.delete("a.txt")
来源：http://ntf.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://xfh.mhx1999.top

[F07] 创建目录（含多级）
来源：http://xrs.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jkf.shanyushiyangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uva.zhijiandao.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://buu.haohaochexian.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kfw.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ohg.chenjidiqi.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cyz.fengsongda.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zqv.c1oappe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://meg.ybcxt.top

[F08] 遍历目录
来源：http://pqa.smart0.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://byf.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fwx.hammf.cn

JS:   fs.readdirSync("dir")
来源：http://fya.dianchejie.cn

TS:   fs.readdirSync("dir")
来源：http://krf.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xok.iojbl.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pcb.jqgfzy.top

Ruby: Dir.children("dir")
来源：http://pfk.xylfe.cn

C#:   Directory.GetFiles("dir")
来源：http://dhj.316326.xyz

[F09] 获取文件大小
来源：http://rwz.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://hdw.snrcjt.cn

PHP:  filesize("a.txt");
来源：http://hfg.yonumen.top

JS:   fs.statSync("a.txt").size
来源：http://svr.hywenlv.cn

TS:   fs.statSync("a.txt").size
来源：http://bvf.sufxvd.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cdc.hongshengwenyu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wrk.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://vxu.zhengqikj.top

C#:   new FileInfo("a.txt").Length
来源：http://ugy.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://vzn.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jxp.pycfn.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rqs.bjfxy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cuh.sysykeji.top

TS:   path.extname("a.txt")
来源：http://ifr.sweek.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ofr.wangshuangyany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://crm.shanyushiyangtech.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tpt.yanxiufei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zwi.sysykeji.top

[F11] 复制与移动文件
来源：http://cme.nanxuanxn.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://frk.hysaishi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jkz.guannengcc.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://czi.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uhb.jqgufenzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lww.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jpt.ywan-chungtsiang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sfi.ctjpmb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xbq.jqgufenzy.top

[F12] CSV 读写
来源：http://ikq.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cnk.zhengqikj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qir.cucudq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zro.gaohongyu789.top

TS:   // 同上
来源：http://ahm.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xre.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gui.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eeb.xylfe.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xlu.jianghu66.top

================================================================================
来源：http://rwg.hesvh.cn

G. 面向对象
来源：http://zyn.nanxinkj.top

================================================================================
来源：http://bgv.wangdashe.top

[G01] 定义类
来源：http://iad.guannengcc.top

Py:   class User: pass
来源：http://lnl.kuanghao11.cn

PHP:  class User {}
来源：http://zei.0kj1m.cn

JS:   class User {}
来源：http://uqh.jinqigfzy.top

TS:   class User { name: string = ""; }
来源：http://qmy.cucudq.cn

Java: class User {}
来源：http://rxk.nanxinkj.top

Go:   type User struct { Name string }
来源：http://jpu.jlsjyb.cn

Ruby: class User; end
来源：http://cjt.zhiwuduotai.top

C#:   class User {}
来源：http://ayc.mhx1999.top

[G02] 构造函数
来源：http://yyz.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://nur.snrcjt.cn

PHP:  public function __construct(public string $name) {}
来源：http://akv.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://ont.bbcook.cn

TS:   constructor(public name: string) {}
来源：http://jnk.hammf.cn

Java: User(String name) { this.name = name; }
来源：http://ubx.vehdjk.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xnr.316326.xyz

Ruby: def initialize(name); @name = name; end
来源：http://jyn.zhengqikj.top

C#:   public User(string name) { Name = name; }
来源：http://gvd.jiagoushi.top

[G03] 实例属性
来源：http://yww.zhengqikj.top

Py:   self.name = "x"
来源：http://gjs.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://xnt.quarkkingdee.top

JS:   this.name = "x";
来源：http://ovp.redwolf501.top

TS:   name: string = "x";
来源：http://ewk.vqdsnc.cn

Java: private String name;
来源：http://dzd.shanyushiyangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ykz.zycfv.cn

Ruby: @name = "x"
来源：http://oyc.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://fcy.cqqwz.cn

[G04] 定义方法
来源：http://ydg.birdmap.top

Py:   def greet(self): return self.name
来源：http://lsr.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cqd.xuanzx.com

JS:   greet() { return this.name; }
来源：http://rkm.shuidangran.top

TS:   greet(): string { return this.name; }
来源：http://owb.guannengcc.top

Java: String greet() { return name; }
来源：http://bql.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://awb.0kj1m.cn

Ruby: def greet; @name; end
来源：http://zkl.gzhubu.top

C#:   public string Greet() => Name;
来源：http://zdy.gotoacloud.top

[G05] 继承
来源：http://knn.yongpay.top

Py:   class Admin(User): pass
来源：http://iez.jlsjyb.cn

PHP:  class Admin extends User {}
来源：http://oqa.yanxiufei.cn

JS:   class Admin extends User {}
来源：http://ipx.ehwqpu.com

TS:   class Admin extends User {}
来源：http://mes.vehdjk.com

Java: class Admin extends User {}
来源：http://whr.jinqigfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ahn.yonumen.top

Ruby: class Admin < User; end
来源：http://pxt.ctjpmb.com

C#:   class Admin : User {}
来源：http://bjq.wangdashe.top

[G06] 重写方法
来源：http://hxr.yongpay.top

Py:   def greet(self): return "admin"
来源：http://uzd.zhengqikj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://big.yj202588.top

JS:   greet() { return "admin"; }
来源：http://bet.hammf.cn

TS:   greet(): string { return "admin"; }
来源：http://isf.meibo888.top

Java: @Override String greet() { return "admin"; }
来源：http://qlb.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://luk.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://ghr.tanke756.top

C#:   public override string Greet() => "admin";
来源：http://mdq.cqqwz.cn

[G07] 调用父类方法
来源：http://sgq.vehdjk.com

Py:   super().greet()
来源：http://pgi.tian-w.cn

PHP:  parent::greet();
来源：http://hjb.hnqzz.top

JS:   super.greet();
来源：http://yli.shangyingyoupin.top

TS:   super.greet();
来源：http://jpl.hongshengwenyu.top

Java: super.greet();
来源：http://ebd.yanxiufei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ryv.hywenlv.cn

Ruby: super
来源：http://jks.bbcook.cn

C#:   base.Greet();
来源：http://hqq.ppjwa.cn

[G08] 静态方法与属性
来源：http://afk.uphjek.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ulc.hongshengwenyu.top

PHP:  public static function f() {}
来源：http://dum.aizwys.cn

JS:   static f() {}
来源：http://toq.nwbrower.top

TS:   static f(): void {}
来源：http://agl.chenjidiqi.icu

Java: static void f() {}
来源：http://wmy.quarkkingdee.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zjk.yfazqb.com

Ruby: def self.f; end
来源：http://xzf.mhx1999.top

C#:   public static void F() {}
来源：http://kpo.yangfankeji.com

[G09] 接口 / 抽象类
来源：http://txr.jqgufenzy.top

Py:   from abc import ABC, abstractmethod
来源：http://hlk.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://lul.aizwys.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hpo.gotoacloud.top

TS:   interface Shape { area(): number; }
来源：http://npz.xinyue.icu

Java: interface Shape { double area(); }
来源：http://nzy.tarul.cn

Go:   type Shape interface { Area() float64 }
来源：http://hal.jlsjyb.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tgp.guowangkeji.top

C#:   interface IShape { double Area(); }
来源：http://vje.tianlin.xyz

[G10] 访问控制
来源：http://eqi.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://cwi.hnqzz.top

PHP:  public / protected / private
来源：http://lut.gaohongyu789.top

JS:   #private 字段；其余公开
来源：http://kbl.sysykeji.top

TS:   public / protected / private
来源：http://uph.daxiang520.top

Java: public / protected / private / 默认包级
来源：http://bbz.yanxiufei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tez.shuidangran.top

Ruby: public / protected / private
来源：http://sug.yongpay.top

C#:   public / protected / private / internal
来源：http://krw.guowangkeji.top

[G11] getter / setter
来源：http://lyj.ywan-chungtsiang.top

Py:   @property 与 @x.setter
来源：http://oyv.ydjk.org.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hot.guowangkeji.top

JS:   get name() { return this._name; }
来源：http://was.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://coi.yfazqb.com

Java: public String getName() { return name; }
来源：http://mmk.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://swk.hcnkem.com

Ruby: attr_accessor :name
来源：http://sek.iojbl.cn

C#:   public string Name { get; set; }
来源：http://zgs.hcnkem.com

[G12] 对象转字符串
来源：http://fcn.wangdashe.top

Py:   def __str__(self): return self.name
来源：http://dgl.daxiang520.top


<!-- 参考信息 -->
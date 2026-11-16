代发 wailian999

Go:   strings.Count(s, "a")
来源：http://fxe.ppjwa.cn

Ruby: s.count("a")
来源：http://uqy.cheryme.top

C#:   s.Count(c => c == 'a')
来源：http://wkh.snrcjt.cn

[E13] 逐字符遍历
来源：http://qwj.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://rvb.jqgufenzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lmy.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ocq.tarul.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kpe.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ono.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qoa.aibaodan.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lje.yanxiufei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ovk.zycfv.cn

[E14] URL 编码与 Base64
来源：http://irz.fengsongda.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ocx.nanxinkj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://eqy.fzhhl.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dew.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hkl.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ewe.wangdashe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ckk.gotoacloud.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://njd.52xcode.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dmk.zdbjq.cn

[E15] HTML 转义 / 反转义
来源：http://fmh.hnqzz.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qvt.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wtg.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://itz.bjfxy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ths.nanxuanxn.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eff.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://byq.iojbl.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gio.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lij.daria6918.cn

[E16] 数字千分位
来源：http://vcz.yj202588.top

Py:   f"{1234567:,}"
来源：http://idr.shanyushiyangtech.top

PHP:  number_format(1234567);
来源：http://kwq.havefunace.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jrk.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mhn.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qup.nanxuanxn.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vfw.hywenlv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://irn.smart0.xyz

C#:   1234567.ToString("N0")
来源：http://xrk.yuxming.cn

[E17] 首字母大写
来源：http://zmt.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vdv.hnxiangtu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://htn.zhixingplan.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zdo.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oxe.uphjek.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oyj.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kwa.ydjk.org.cn

Ruby: s.capitalize
来源：http://mgq.snrcjt.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cnb.ivvv.top

[E18] 模板占位符替换
来源：http://zjd.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hsc.snrcjt.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bds.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kor.meibo888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ubq.ivvv.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mwu.yj202588.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fxl.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bcu.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://euo.ybcxt.top

[E19] 多行文本按行拆分
来源：http://sqa.nanxuanxn.top

Py:   s.splitlines()
来源：http://pjy.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gnj.ybcxt.top

JS:   s.split(/\r?\n/)
来源：http://jiw.xingfuxueyuan.xyz

TS:   s.split(/\r?\n/)
来源：http://xkx.smart0.xyz

Java: s.lines().toList()
来源：http://rvr.xuanzx.com

Go:   strings.Split(s, "\n")
来源：http://img.zhaomingkeji.xyz

Ruby: s.lines
来源：http://jvo.ydzc1.top

C#:   s.Split('\n')
来源：http://epr.zhaomingkeji.xyz

[E20] 判断字符串是否为空
来源：http://heq.xinyue.icu

Py:   if not s:
来源：http://llx.haohaochexian.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nvl.yueranfly.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vjv.hongshengwenyu.top

TS:   if (s === "") {}
来源：http://hil.smart0.xyz

Java: if (s.isEmpty()) {}
来源：http://aof.bjfxy.top

Go:   if s == "" {}
来源：http://pis.zhoulong.xyz

Ruby: if s.empty?
来源：http://ysq.smart0.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pfg.ctjpmb.com

[E21] 超长截断加省略号
来源：http://vlp.pengpengdd.cyou

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://efg.zhaomingkeji.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zzr.bjfxy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dhi.jlsjyb.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gmw.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bft.yj20258.top

Go:   // 按 rune 判断长度后截断
来源：http://xvo.ppjwa.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tgr.xingfuxueyuan.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nrt.shuidangran.top

[E22] 字节长度与字符长度
来源：http://zne.hnxiangtu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yor.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zcy.bbcook.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yqw.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kjp.hesvh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ann.dianchejie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ieq.hnxiangtu.top

Ruby: s.bytesize;  s.length
来源：http://zqi.daria6918.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xok.fktsv.cn

================================================================================
来源：http://ltc.xuetiantiany.cn

F. 文件与目录
来源：http://uok.nanxuanxn.top

================================================================================
来源：http://ltb.zhiwuduotai.top

[F01] 读取整个文件
来源：http://apn.cheryme.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gjz.chenzaomai.com

PHP:  file_get_contents("a.txt");
来源：http://fcl.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uyo.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://phi.hysaishi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lzv.zdbjq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://str.yvedp.cn

Ruby: File.read("a.txt")
来源：http://jft.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://fzt.guannengcc.top

[F02] 逐行读取文件
来源：http://mjh.c1oappe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uki.tianlin.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kas.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pyv.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zay.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aen.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fth.yanxiufei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gcm.xinyue.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mds.ywan-chungtsiang.top

[F03] 写入文件（覆盖）
来源：http://zgs.52xcode.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fbm.chenzaomai.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://rur.chenlongwang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xtt.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lqs.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yyh.uphjek.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uus.fktsv.cn

Ruby: File.write("a.txt", "hi")
来源：http://ndz.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cvn.svipenyu.cn

[F04] 追加写入文件
来源：http://sxk.hnqzz.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jrb.daria6918.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://afo.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rtx.yj202588.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://onm.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dko.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hqg.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jvg.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nub.yanxiufei.cn

[F05] 判断文件或目录是否存在
来源：http://syh.jiagoushi.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fks.hcnkem.com

PHP:  file_exists("a.txt");
来源：http://wlh.cheryme.top

JS:   fs.existsSync("a.txt")
来源：http://jsv.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://ccc.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://kmf.zdbjq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lov.zdqjudy.top

Ruby: File.exist?("a.txt")
来源：http://exb.iojbl.cn

C#:   File.Exists("a.txt")
来源：http://ibr.fzhhl.top

[F06] 删除文件
来源：http://ixa.xuetiantiany.cn

Py:   os.remove("a.txt")
来源：http://ria.feifeiyinyue.top

PHP:  unlink("a.txt");
来源：http://jmr.xziqi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gux.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://qzq.quarkkingdee.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tgh.ctjpmb.com

Go:   os.Remove("a.txt")
来源：http://qpz.xylfe.cn

Ruby: File.delete("a.txt")
来源：http://tye.uphjek.com

C#:   File.Delete("a.txt");
来源：http://nco.hammf.cn

[F07] 创建目录（含多级）
来源：http://ffk.sufxvd.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ywg.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pdp.ydzc1.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iaa.bbcook.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://thn.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://trq.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lgs.0kj1m.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wof.ctjpmb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kzs.xziqi.cn

[F08] 遍历目录
来源：http://ykn.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gpn.zhaomingkeji.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tom.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://teu.fehbvm.com

TS:   fs.readdirSync("dir")
来源：http://baw.hesvh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nqk.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pdm.wangdashe.top

Ruby: Dir.children("dir")
来源：http://pzd.jqgfzy.top

C#:   Directory.GetFiles("dir")
来源：http://uod.xuetiantiany.cn

[F09] 获取文件大小
来源：http://ruy.yongpay.top

Py:   os.path.getsize("a.txt")
来源：http://fzh.smart0.xyz

PHP:  filesize("a.txt");
来源：http://yru.hysaishi.cn

JS:   fs.statSync("a.txt").size
来源：http://apn.epnwcf.com

TS:   fs.statSync("a.txt").size
来源：http://osy.yj202588.top

Java: Files.size(Path.of("a.txt"))
来源：http://wst.cqqwz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ord.snrcjt.cn

Ruby: File.size("a.txt")
来源：http://mar.tarul.cn

C#:   new FileInfo("a.txt").Length
来源：http://jqp.shzxlz.cn

[F10] 取文件扩展名 / 文件名
来源：http://alv.tianlin.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wuw.wangshuangyany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mkk.dianchejie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dgj.cqqwz.cn

TS:   path.extname("a.txt")
来源：http://ahu.xuetiantiany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fmv.xingfuxueyuan.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sbn.aizwys.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xmw.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qvx.fktsv.cn

[F11] 复制与移动文件
来源：http://sqm.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://obv.ydzc1.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dja.svipenyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wpm.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://els.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cbj.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bxe.shanyushiyangtech.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hzo.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ktn.xylfe.cn

[F12] CSV 读写
来源：http://jgv.xuetiantiany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://apr.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://alm.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uui.daxiang520.top

TS:   // 同上
来源：http://pou.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://geq.hfpthk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://olw.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qcf.ctjpmb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://nnl.sysykeji.top

================================================================================
来源：http://bja.zhiwuduotai.top

G. 面向对象
来源：http://guu.gzhubu.top

================================================================================
来源：http://tte.hywenlv.cn

[G01] 定义类
来源：http://prt.sxryk.cn

Py:   class User: pass
来源：http://pwh.yj20258.top

PHP:  class User {}
来源：http://bgq.hcnkem.com

JS:   class User {}
来源：http://zle.yongpay.top

TS:   class User { name: string = ""; }
来源：http://fum.yongpay.top

Java: class User {}
来源：http://osm.daxiang520.top

Go:   type User struct { Name string }
来源：http://cql.nanxuanxn.top

Ruby: class User; end
来源：http://gxd.ivvv.top

C#:   class User {}
来源：http://nue.sysykeji.top

[G02] 构造函数
来源：http://ruk.hnqzz.top

Py:   def __init__(self, name): self.name = name
来源：http://lrg.yanxiufei.cn

PHP:  public function __construct(public string $name) {}
来源：http://iqn.sweek.top

JS:   constructor(name) { this.name = name; }
来源：http://oey.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://ccv.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://rui.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pce.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://ywg.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://pgc.uphjek.com

[G03] 实例属性
来源：http://tbd.feifeiyinyue.top

Py:   self.name = "x"
来源：http://ubf.ppjwa.cn

PHP:  public string $name = "x";
来源：http://uir.yueranfly.top

JS:   this.name = "x";
来源：http://gtj.havefunace.top

TS:   name: string = "x";
来源：http://ggw.birdmap.top

Java: private String name;
来源：http://mma.yuanzhike.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qcl.jinqigfzy.top

Ruby: @name = "x"
来源：http://hzc.jyoumei.cn

C#:   public string Name { get; set; } = "x";
来源：http://mkg.bbcook.cn

[G04] 定义方法
来源：http://uzh.snrcjt.cn

Py:   def greet(self): return self.name
来源：http://mvq.sufxvd.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ary.zycfv.cn

JS:   greet() { return this.name; }
来源：http://uwu.aizwys.cn

TS:   greet(): string { return this.name; }
来源：http://lsi.yangfankeji.com

Java: String greet() { return name; }
来源：http://ugf.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xjp.zhijiandao.cn

Ruby: def greet; @name; end
来源：http://prq.pycfn.com

C#:   public string Greet() => Name;
来源：http://fuj.aibaodan.cn

[G05] 继承
来源：http://nxx.cqqwz.cn

Py:   class Admin(User): pass
来源：http://hte.gogol.net.cn

PHP:  class Admin extends User {}
来源：http://jah.cqqwz.cn

JS:   class Admin extends User {}
来源：http://yvb.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://jgh.iojbl.cn

Java: class Admin extends User {}
来源：http://pfy.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hhu.9152youxi.cn

Ruby: class Admin < User; end
来源：http://jbm.gzhubu.top

C#:   class Admin : User {}
来源：http://elo.guowangkeji.top

[G06] 重写方法
来源：http://spv.sysykeji.top

Py:   def greet(self): return "admin"
来源：http://prc.gaohongyu789.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kqk.andypj.xyz

JS:   greet() { return "admin"; }
来源：http://hes.fzhhl.top

TS:   greet(): string { return "admin"; }
来源：http://wdv.ctjpmb.com

Java: @Override String greet() { return "admin"; }
来源：http://mth.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://owa.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://vie.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://ziu.hcnkem.com

[G07] 调用父类方法
来源：http://kjt.xuetiantiany.cn

Py:   super().greet()
来源：http://bes.feifeiyinyue.top

PHP:  parent::greet();
来源：http://iau.jlsjyb.cn

JS:   super.greet();
来源：http://bjr.cdnleiting.top

TS:   super.greet();
来源：http://tfb.yueranfly.top

Java: super.greet();
来源：http://wwi.yj20258.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ilh.nanxuanxn.top

Ruby: super
来源：http://jiq.yuanzhike.top

C#:   base.Greet();
来源：http://esq.quarkkingdee.top

[G08] 静态方法与属性
来源：http://tdh.ydjk.org.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://brz.hesvh.cn

PHP:  public static function f() {}
来源：http://tbl.ywan-chungtsiang.top

JS:   static f() {}
来源：http://kts.ivvv.top

TS:   static f(): void {}
来源：http://bkt.epnwcf.com

Java: static void f() {}
来源：http://gis.yj202588.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ezp.zhengqikj.top

Ruby: def self.f; end
来源：http://dxj.fktsv.cn

C#:   public static void F() {}
来源：http://ijt.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://kgx.yvedp.cn

Py:   from abc import ABC, abstractmethod
来源：http://ecm.gotoacloud.top

PHP:  interface Shape { public function area(): float; }
来源：http://hvo.gaohongyu789.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ozw.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://vco.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://qoh.andypj.xyz

Go:   type Shape interface { Area() float64 }
来源：http://cdm.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pub.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://kau.yueranfly.top

[G10] 访问控制
来源：http://fde.jianghu66.top

Py:   约定 _protected / __private（不强制）
来源：http://ttc.c1oappe.top

PHP:  public / protected / private
来源：http://udb.hammf.cn

JS:   #private 字段；其余公开
来源：http://niv.birdmap.top

TS:   public / protected / private
来源：http://zqa.cqqwz.cn

Java: public / protected / private / 默认包级
来源：http://zxo.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ost.316326.xyz

Ruby: public / protected / private
来源：http://jdw.haohaochexian.top

C#:   public / protected / private / internal
来源：http://zxu.wangdashe.top

[G11] getter / setter
来源：http://rgv.uphjek.com

Py:   @property 与 @x.setter
来源：http://arm.hnqzz.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mok.jinghuilouyu.cn


<!-- 参考信息 -->
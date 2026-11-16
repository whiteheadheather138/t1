代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rqb.haohaochexian.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jwm.sjlbkw.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vlv.hysaishi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ihf.zhongyouzk.top

[E14] URL 编码与 Base64
来源：http://paq.chenjidiqi.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wgu.gogol.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jdq.yuanzhike.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ebb.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://etl.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nzh.guannengcc.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yxo.xuetiantiany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sma.ywan-chungtsiang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://svx.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://wbs.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ljv.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blr.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://suh.smart0.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://jup.ywan-chungtsiang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ywv.nwbrower.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ttn.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iks.pycfn.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ixs.hysaishi.cn

[E16] 数字千分位
来源：http://fdu.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://vpi.zhongyouzk.top

PHP:  number_format(1234567);
来源：http://ilc.hnqzz.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qob.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sof.fengsongda.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lap.nwbrower.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ive.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cam.jinyuanbaomall.cn

C#:   1234567.ToString("N0")
来源：http://ypi.aibaodan.cn

[E17] 首字母大写
来源：http://twv.haohaochexian.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cod.ydzc1.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ewj.tanke756.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://txo.tanke756.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dme.jyoumei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qje.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dnm.hfpthk.cn

Ruby: s.capitalize
来源：http://ijs.mhx1999.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nxm.c1oappe.top

[E18] 模板占位符替换
来源：http://ucd.pengpengdd.cyou

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ewu.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mve.jianghu66.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ost.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://yir.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tng.vqdsnc.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lwv.tianlin.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rqi.bjfxy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uhx.sysykeji.top

[E19] 多行文本按行拆分
来源：http://yof.sweek.top

Py:   s.splitlines()
来源：http://jdp.zhixingplan.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lhq.c1oappe.top

JS:   s.split(/\r?\n/)
来源：http://zzj.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://ykl.0kj1m.cn

Java: s.lines().toList()
来源：http://rzp.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://asu.birdmap.top

Ruby: s.lines
来源：http://ztf.zdbjq.cn

C#:   s.Split('\n')
来源：http://bmt.ppjwa.cn

[E20] 判断字符串是否为空
来源：http://kld.zdqjudy.top

Py:   if not s:
来源：http://hkj.vqdsnc.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://otd.haohaochexian.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iny.daria6918.cn

TS:   if (s === "") {}
来源：http://jdf.jinqigfzy.top

Java: if (s.isEmpty()) {}
来源：http://hpo.aizwys.cn

Go:   if s == "" {}
来源：http://yqx.xuetiantiany.cn

Ruby: if s.empty?
来源：http://eee.mhx1999.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://asu.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://hdo.zhaomingkeji.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bvv.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vde.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://obh.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xlp.birdmap.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ont.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://nus.jianghu66.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vpr.shuidangran.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rpa.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://cjo.sweek.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ovk.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wos.0kj1m.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fug.feifeiyinyue.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oel.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lyu.feifeiyinyue.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nnf.xziqi.cn

Ruby: s.bytesize;  s.length
来源：http://lpx.fehbvm.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://usl.cashguo.top

================================================================================
来源：http://wrq.nanxuanxn.top

F. 文件与目录
来源：http://bru.feifeiyinyue.top

================================================================================
来源：http://ekh.zycfv.cn

[F01] 读取整个文件
来源：http://mbt.aibaodan.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qvq.yvedp.cn

PHP:  file_get_contents("a.txt");
来源：http://xme.birdmap.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uul.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://her.yj202588.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zdd.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hxj.zhiwuduotai.top

Ruby: File.read("a.txt")
来源：http://nfk.shzxlz.cn

C#:   File.ReadAllText("a.txt");
来源：http://nwu.zhongyouzk.top

[F02] 逐行读取文件
来源：http://ysk.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ujm.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nuf.shanyushiyangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xzm.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pup.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xax.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tun.sjlbkw.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gpj.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fsb.cashguo.top

[F03] 写入文件（覆盖）
来源：http://gxo.meibo888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mqd.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xkj.bbcook.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://any.tanke756.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tuc.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://frd.fanxiaobao.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yne.nanxuanxn.top

Ruby: File.write("a.txt", "hi")
来源：http://mlv.daxiang520.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zne.yongpay.top

[F04] 追加写入文件
来源：http://ukq.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wto.chenzaomai.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rxi.hysaishi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xzg.meibo888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ofl.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cny.cdnleiting.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kxi.kuanghao11.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pme.xuanzx.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qnr.wangshuangyany.cn

[F05] 判断文件或目录是否存在
来源：http://hcg.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dyx.jinqigufen.top

PHP:  file_exists("a.txt");
来源：http://qsh.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://rzh.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://hcs.zhongyouzk.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jbv.mhx1999.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yii.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://ubd.redwolf501.top

C#:   File.Exists("a.txt")
来源：http://tzr.ppjwa.cn

[F06] 删除文件
来源：http://ecs.tarul.cn

Py:   os.remove("a.txt")
来源：http://stv.yongpay.top

PHP:  unlink("a.txt");
来源：http://oxr.zhengqikj.top

JS:   fs.unlinkSync("a.txt")
来源：http://bdi.jianghu66.top

TS:   fs.unlinkSync("a.txt")
来源：http://xnb.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dpw.jyoumei.cn

Go:   os.Remove("a.txt")
来源：http://kiy.tanke756.top

Ruby: File.delete("a.txt")
来源：http://xca.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://ilx.fehbvm.com

[F07] 创建目录（含多级）
来源：http://lou.cashguo.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kva.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aew.fktsv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jpg.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sjg.jqgfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eld.xingfuxueyuan.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://exq.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bpd.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hrz.wangdashe.top

[F08] 遍历目录
来源：http://dcd.hcnkem.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://mji.hnxiangtu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dbz.ydjk.org.cn

JS:   fs.readdirSync("dir")
来源：http://odd.ybcxt.top

TS:   fs.readdirSync("dir")
来源：http://xmn.yonumen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rwl.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://kcp.zhijiandao.cn

Ruby: Dir.children("dir")
来源：http://laa.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://fnb.yj20258888.top

[F09] 获取文件大小
来源：http://fgq.tanke756.top

Py:   os.path.getsize("a.txt")
来源：http://wan.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://iiu.fehbvm.com

JS:   fs.statSync("a.txt").size
来源：http://qqe.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://bkw.aizwys.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yio.epnwcf.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kpq.meibo888.top

Ruby: File.size("a.txt")
来源：http://jvu.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://axl.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://glj.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zjd.guowangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nnl.meibo888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://amy.kuanghao11.cn

TS:   path.extname("a.txt")
来源：http://dce.epnwcf.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qtg.uphjek.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lgl.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zwm.yanxiufei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lbg.nanxuanxn.top

[F11] 复制与移动文件
来源：http://kzd.ydjk.org.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kpk.cheryme.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eqv.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dgv.xinyue.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ugb.hesvh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zix.sxryk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yna.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bei.jinyuanbaomall.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://udy.jianghu66.top

[F12] CSV 读写
来源：http://rxz.316326.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cmo.xingfuxueyuan.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dsu.yj202588.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wrm.yj202588.top

TS:   // 同上
来源：http://wru.quarkkingdee.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bti.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yuu.jianghu66.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jww.jlsjyb.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://woy.jianghu66.top

================================================================================
来源：http://voz.xingfuxueyuan.xyz

G. 面向对象
来源：http://nyk.yj20258.top

================================================================================
来源：http://opx.hongshengwenyu.top

[G01] 定义类
来源：http://rsm.sufxvd.cn

Py:   class User: pass
来源：http://tuz.jinyuanbaomall.cn

PHP:  class User {}
来源：http://rcu.ywan-chungtsiang.top

JS:   class User {}
来源：http://kin.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://daz.yanxiufei.cn

Java: class User {}
来源：http://jad.epnwcf.com

Go:   type User struct { Name string }
来源：http://apv.0kj1m.cn

Ruby: class User; end
来源：http://ysx.bjfxy.top

C#:   class User {}
来源：http://azl.yfazqb.com

[G02] 构造函数
来源：http://xhu.sysykeji.top

Py:   def __init__(self, name): self.name = name
来源：http://lgx.sxryk.cn

PHP:  public function __construct(public string $name) {}
来源：http://foa.0kj1m.cn

JS:   constructor(name) { this.name = name; }
来源：http://cpq.xuanzx.com

TS:   constructor(public name: string) {}
来源：http://adq.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://kpk.cdnleiting.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tkw.hcnkem.com

Ruby: def initialize(name); @name = name; end
来源：http://cov.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://nxx.shuidangran.top

[G03] 实例属性
来源：http://reo.uphjek.com

Py:   self.name = "x"
来源：http://wwb.zhixingplan.top

PHP:  public string $name = "x";
来源：http://lvk.snrcjt.cn

JS:   this.name = "x";
来源：http://tuy.daxiang520.top

TS:   name: string = "x";
来源：http://rcs.pycfn.com

Java: private String name;
来源：http://gpl.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bnu.jlsjyb.cn

Ruby: @name = "x"
来源：http://ntj.jqgfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://hiz.cdnleiting.top

[G04] 定义方法
来源：http://fjj.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://wda.cdnleiting.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ehy.feifeiyinyue.top

JS:   greet() { return this.name; }
来源：http://dbh.redwolf501.top

TS:   greet(): string { return this.name; }
来源：http://udr.quarkkingdee.top

Java: String greet() { return name; }
来源：http://aum.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ngf.pengpengdd.cyou

Ruby: def greet; @name; end
来源：http://xop.9152youxi.cn

C#:   public string Greet() => Name;
来源：http://tnq.sxryk.cn

[G05] 继承
来源：http://pmz.hnqzz.top

Py:   class Admin(User): pass
来源：http://gjt.nanxuanxn.top

PHP:  class Admin extends User {}
来源：http://yaw.cqqwz.cn

JS:   class Admin extends User {}
来源：http://hpg.guannengcc.top

TS:   class Admin extends User {}
来源：http://opw.yanxiufei.cn

Java: class Admin extends User {}
来源：http://vkp.tarul.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://quq.tanke756.top

Ruby: class Admin < User; end
来源：http://unq.jinqigufen.top

C#:   class Admin : User {}
来源：http://hjd.sweek.top

[G06] 重写方法
来源：http://cha.zdqjudy.top

Py:   def greet(self): return "admin"
来源：http://kkn.fzhhl.top

PHP:  public function greet(): string { return "admin"; }
来源：http://deu.tarul.cn

JS:   greet() { return "admin"; }
来源：http://iwo.shuidangran.top

TS:   greet(): string { return "admin"; }
来源：http://xeo.gaohongyu789.top

Java: @Override String greet() { return "admin"; }
来源：http://cwa.daxiang520.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jkg.sysykeji.top

Ruby: def greet; "admin"; end
来源：http://mkh.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://mvf.shzxlz.cn

[G07] 调用父类方法
来源：http://qya.ivvv.top

Py:   super().greet()
来源：http://hss.mhx1999.top

PHP:  parent::greet();
来源：http://uym.yanxiufei.cn

JS:   super.greet();
来源：http://qkj.guannengcc.top

TS:   super.greet();
来源：http://atj.xziqi.cn

Java: super.greet();
来源：http://mrq.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://knu.snrcjt.cn

Ruby: super
来源：http://ycb.wangdashe.top

C#:   base.Greet();
来源：http://lwf.xziqi.cn

[G08] 静态方法与属性
来源：http://ghc.zdbjq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bkl.zhongyouzk.top

PHP:  public static function f() {}
来源：http://qka.shangyingyoupin.top

JS:   static f() {}
来源：http://ebs.chenlongwang.top

TS:   static f(): void {}
来源：http://sxe.jqgfzy.top

Java: static void f() {}
来源：http://gbs.shuidangran.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://seo.haohaochexian.top

Ruby: def self.f; end
来源：http://jsr.yongpay.top

C#:   public static void F() {}
来源：http://nhh.mhx1999.top

[G09] 接口 / 抽象类
来源：http://krr.quarkkingdee.top

Py:   from abc import ABC, abstractmethod
来源：http://wig.xziqi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://brx.yangfankeji.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://tom.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://hbd.ctjpmb.com

Java: interface Shape { double area(); }
来源：http://qhg.epnwcf.com

Go:   type Shape interface { Area() float64 }
来源：http://ope.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zpc.fanxiaobao.xyz

C#:   interface IShape { double Area(); }
来源：http://ceh.cdnleiting.top

[G10] 访问控制
来源：http://nsy.havefunace.top

Py:   约定 _protected / __private（不强制）
来源：http://kms.ywan-chungtsiang.top

PHP:  public / protected / private
来源：http://ggg.sxryk.cn

JS:   #private 字段；其余公开
来源：http://svw.sysykeji.top

TS:   public / protected / private
来源：http://oqx.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://noe.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://iio.nanxinkj.top

Ruby: public / protected / private
来源：http://gzb.epnwcf.com

C#:   public / protected / private / internal
来源：http://qsg.pengpengdd.cyou

[G11] getter / setter
来源：http://lzx.smart0.xyz

Py:   @property 与 @x.setter
来源：http://zhw.yuanzhike.top

PHP:  public function getName(): string { return $this->name; }
来源：http://url.tian-w.cn

JS:   get name() { return this._name; }
来源：http://dbe.tarul.cn

TS:   get name(): string { return this._name; }
来源：http://uoy.snrcjt.cn

Java: public String getName() { return name; }
来源：http://fbn.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://uqp.iojbl.cn

Ruby: attr_accessor :name
来源：http://csq.gogol.net.cn

C#:   public string Name { get; set; }
来源：http://nrk.nanxuanxn.top

[G12] 对象转字符串
来源：http://isp.bjfxy.top

Py:   def __str__(self): return self.name
来源：http://ycp.daria6918.cn


<!-- 参考信息 -->
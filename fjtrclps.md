代发 wailian999

JS:   [...s].reverse().join("")
来源：http://ajx.cucudq.cn

TS:   [...s].reverse().join("")
来源：http://kkx.hammf.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ann.sufxvd.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rzm.vqdsnc.cn

Ruby: s.reverse
来源：http://jmj.jyoumei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dfd.snrcjt.cn

[E12] 统计某字符出现次数
来源：http://cnd.zdqjudy.top

Py:   s.count("a")
来源：http://cbt.hfpthk.cn

PHP:  substr_count($s, "a");
来源：http://pns.redwolf501.top

JS:   s.split("a").length - 1
来源：http://mhb.tian-w.cn

TS:   s.split("a").length - 1
来源：http://tpm.shzxlz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fzv.hnqzz.top

Go:   strings.Count(s, "a")
来源：http://weo.gzhubu.top

Ruby: s.count("a")
来源：http://gvq.chenzaomai.com

C#:   s.Count(c => c == 'a')
来源：http://yvu.jinyuanbaomall.cn

[E13] 逐字符遍历
来源：http://spi.nanxuanxn.top

Py:   for ch in s: print(ch)
来源：http://pjp.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rsf.fanxiaobao.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://mhk.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://yhe.hcnkem.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yiu.ppjwa.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ohk.kuanghao11.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kpv.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tpi.gaohongyu789.top

[E14] URL 编码与 Base64
来源：http://ydc.yvedp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hqi.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://boh.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dpd.wangdashe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iud.xylfe.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://udp.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://utb.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wjg.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://djz.hnqzz.top

[E15] HTML 转义 / 反转义
来源：http://cqq.kuanghao11.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://owo.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mpg.hnqzz.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rmf.bbcook.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zpf.xuanzx.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xxh.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bpl.9152youxi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ktl.fehbvm.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://alk.nanxuanxn.top

[E16] 数字千分位
来源：http://vhy.ehwqpu.com

Py:   f"{1234567:,}"
来源：http://cmw.yuxming.cn

PHP:  number_format(1234567);
来源：http://nhw.jianghu66.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fqy.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fvk.ywan-chungtsiang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zzu.shzxlz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ejn.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dow.wangshuangyany.cn

C#:   1234567.ToString("N0")
来源：http://cza.guannengcc.top

[E17] 首字母大写
来源：http://sib.meibo888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ynr.hnxiangtu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ctf.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jjo.birdmap.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rlr.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://are.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nnk.bjfxy.top

Ruby: s.capitalize
来源：http://zhh.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pyu.svipenyu.cn

[E18] 模板占位符替换
来源：http://fob.svipenyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zay.316326.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mbu.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://aru.epnwcf.com

TS:   tpl.replaceAll("{name}", name)
来源：http://wuq.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sek.bjfxy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bui.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ctf.hysaishi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lhm.gotoacloud.top

[E19] 多行文本按行拆分
来源：http://xuf.zhongyouzk.top

Py:   s.splitlines()
来源：http://ngp.zhixingplan.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xjx.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://ueq.gaohongyu789.top

TS:   s.split(/\r?\n/)
来源：http://nop.hammf.cn

Java: s.lines().toList()
来源：http://mlv.yuanzhike.top

Go:   strings.Split(s, "\n")
来源：http://xvy.ppjwa.cn

Ruby: s.lines
来源：http://bze.shuidangran.top

C#:   s.Split('\n')
来源：http://yru.chenlongwang.top

[E20] 判断字符串是否为空
来源：http://kzf.shanyushiyangkeji.top

Py:   if not s:
来源：http://mlv.cqqwz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mfy.316326.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vro.wangshuangyany.cn

TS:   if (s === "") {}
来源：http://qeu.zdbjq.cn

Java: if (s.isEmpty()) {}
来源：http://bdv.fehbvm.com

Go:   if s == "" {}
来源：http://khk.zhengqikj.top

Ruby: if s.empty?
来源：http://yns.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vxy.dianchejie.cn

[E21] 超长截断加省略号
来源：http://qnp.meibo888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xwb.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rrs.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zhp.ydjk.org.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ujh.sxryk.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://enn.gotoacloud.top

Go:   // 按 rune 判断长度后截断
来源：http://zkp.uphjek.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mqn.yonumen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://scu.jinqigufen.top

[E22] 字节长度与字符长度
来源：http://xln.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xyi.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://elx.yfazqb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://peu.iojbl.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mcr.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tsl.yanxiufei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wkv.yj20258.top

Ruby: s.bytesize;  s.length
来源：http://jvg.guowangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ftp.cucudq.cn

================================================================================
来源：http://odn.zdqjudy.top

F. 文件与目录
来源：http://axd.svipenyu.cn

================================================================================
来源：http://hbe.snrcjt.cn

[F01] 读取整个文件
来源：http://yll.vehdjk.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uln.nanxuanxn.top

PHP:  file_get_contents("a.txt");
来源：http://pqr.nanxuanxn.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://afz.nanxuanxn.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://clx.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nvt.shzxlz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://azx.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://jdq.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://fhp.zhengqikj.top

[F02] 逐行读取文件
来源：http://vhh.jinyuanbaomall.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mpu.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pvp.jiagoushi.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lri.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vda.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fum.yueranfly.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pyi.daria6918.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qsj.yuxming.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://idf.tanke756.top

[F03] 写入文件（覆盖）
来源：http://vuq.sufxvd.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eby.fktsv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qva.vehdjk.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nbc.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jik.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oiv.xuanzx.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iqy.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://wkx.andypj.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://udm.cqqwz.cn

[F04] 追加写入文件
来源：http://eft.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aye.hywenlv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uwl.sxryk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bfi.zdbjq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ncg.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fbt.52xcode.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cuy.tian-w.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yeg.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gks.yvedp.cn

[F05] 判断文件或目录是否存在
来源：http://juf.iojbl.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://juz.zhixingplan.top

PHP:  file_exists("a.txt");
来源：http://pqp.tanke756.top

JS:   fs.existsSync("a.txt")
来源：http://mlf.guannengcc.top

TS:   fs.existsSync("a.txt")
来源：http://cyl.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zvp.zdbjq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yam.andypj.xyz

Ruby: File.exist?("a.txt")
来源：http://xgs.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://aog.jinqigufen.top

[F06] 删除文件
来源：http://gpy.andypj.xyz

Py:   os.remove("a.txt")
来源：http://evm.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://xlk.ctjpmb.com

JS:   fs.unlinkSync("a.txt")
来源：http://gar.bjfxy.top

TS:   fs.unlinkSync("a.txt")
来源：http://cpo.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mhc.yuanzhike.top

Go:   os.Remove("a.txt")
来源：http://epa.jinqigfzy.top

Ruby: File.delete("a.txt")
来源：http://yrs.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://ytn.sweek.top

[F07] 创建目录（含多级）
来源：http://fkh.sysykeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wpz.sysykeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jvv.c1oappe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zxp.ywan-chungtsiang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://niq.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zvv.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ezg.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ylv.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://htr.zhijiandao.cn

[F08] 遍历目录
来源：http://pao.chenjidiqi.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://mql.ehwqpu.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://snd.gaohongyu789.top

JS:   fs.readdirSync("dir")
来源：http://oib.uphjek.com

TS:   fs.readdirSync("dir")
来源：http://qgb.yanxiufei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jrw.aizwys.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ipe.hesvh.cn

Ruby: Dir.children("dir")
来源：http://wuc.xingfuxueyuan.xyz

C#:   Directory.GetFiles("dir")
来源：http://mkd.snrcjt.cn

[F09] 获取文件大小
来源：http://fcg.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://mww.bjfxy.top

PHP:  filesize("a.txt");
来源：http://utv.hammf.cn

JS:   fs.statSync("a.txt").size
来源：http://lwx.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://inw.shanyushiyangtech.top

Java: Files.size(Path.of("a.txt"))
来源：http://ena.cdnleiting.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://onz.ehwqpu.com

Ruby: File.size("a.txt")
来源：http://waj.bjfxy.top

C#:   new FileInfo("a.txt").Length
来源：http://tmp.dashuyun.cn

[F10] 取文件扩展名 / 文件名
来源：http://epk.fehbvm.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qei.xziqi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wgw.ybcxt.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tsh.hammf.cn

TS:   path.extname("a.txt")
来源：http://ycx.yj202588.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wyi.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oey.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dpm.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bwc.bjfxy.top

[F11] 复制与移动文件
来源：http://ths.yj20258.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://niv.nanxinkj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sfy.chenlongwang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xek.ehwqpu.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ees.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fik.svipenyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xdc.yuxming.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ivs.snrcjt.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uxe.316326.xyz

[F12] CSV 读写
来源：http://gta.fzhhl.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qxs.0kj1m.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xti.yj202588.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nmq.jianghu66.top

TS:   // 同上
来源：http://bvb.ywan-chungtsiang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jol.iojbl.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zud.shzxlz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zpg.gaohongyu789.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nuo.tanke756.top

================================================================================
来源：http://njd.tarul.cn

G. 面向对象
来源：http://nal.yfazqb.com

================================================================================
来源：http://szu.yonumen.top

[G01] 定义类
来源：http://ate.shanyushiyangkeji.top

Py:   class User: pass
来源：http://dwj.9152youxi.cn

PHP:  class User {}
来源：http://hem.bjfxy.top

JS:   class User {}
来源：http://xrp.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://fxu.hnxiangtu.top

Java: class User {}
来源：http://xxo.zdqjudy.top

Go:   type User struct { Name string }
来源：http://yau.yj20258888.top

Ruby: class User; end
来源：http://xea.wangshuangyany.cn

C#:   class User {}
来源：http://inc.ybcxt.top

[G02] 构造函数
来源：http://xfq.bbcook.cn

Py:   def __init__(self, name): self.name = name
来源：http://ucl.xylfe.cn

PHP:  public function __construct(public string $name) {}
来源：http://kas.ydzc1.top

JS:   constructor(name) { this.name = name; }
来源：http://pba.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://pko.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://tke.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dkm.quarkkingdee.top

Ruby: def initialize(name); @name = name; end
来源：http://uql.ctjpmb.com

C#:   public User(string name) { Name = name; }
来源：http://evs.cheryme.top

[G03] 实例属性
来源：http://opp.sysykeji.top

Py:   self.name = "x"
来源：http://xtf.hywenlv.cn

PHP:  public string $name = "x";
来源：http://ngz.cqqwz.cn

JS:   this.name = "x";
来源：http://tbv.quarkkingdee.top

TS:   name: string = "x";
来源：http://yog.jinghuilouyu.cn

Java: private String name;
来源：http://lbo.jqgufenzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rdw.tanke756.top

Ruby: @name = "x"
来源：http://jrx.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://ezs.chenzaomai.com

[G04] 定义方法
来源：http://dop.uphjek.com

Py:   def greet(self): return self.name
来源：http://acb.yueranfly.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ucc.tianlin.xyz

JS:   greet() { return this.name; }
来源：http://ftq.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://jdj.zhaomingkeji.xyz

Java: String greet() { return name; }
来源：http://sct.ehwqpu.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://mee.0kj1m.cn

Ruby: def greet; @name; end
来源：http://nyp.nwbrower.top

C#:   public string Greet() => Name;
来源：http://rsc.tarul.cn

[G05] 继承
来源：http://scv.tian-w.cn

Py:   class Admin(User): pass
来源：http://gyi.jqgufenzy.top

PHP:  class Admin extends User {}
来源：http://wqh.jinqigufen.top

JS:   class Admin extends User {}
来源：http://gfw.jinqigufen.top

TS:   class Admin extends User {}
来源：http://czx.andypj.xyz

Java: class Admin extends User {}
来源：http://fwz.zhixingplan.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dvt.hnqzz.top

Ruby: class Admin < User; end
来源：http://emo.uphjek.com

C#:   class Admin : User {}
来源：http://qjs.wangshuangyany.cn

[G06] 重写方法
来源：http://edn.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://pae.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://nwp.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://nns.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://omu.pengpengdd.cyou

Java: @Override String greet() { return "admin"; }
来源：http://nda.yj202588.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sjj.xuanzx.com

Ruby: def greet; "admin"; end
来源：http://rps.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://ktm.gotoacloud.top

[G07] 调用父类方法
来源：http://oql.yanxiufei.cn

Py:   super().greet()
来源：http://lod.zhengqikj.top

PHP:  parent::greet();
来源：http://ucr.quarkkingdee.top

JS:   super.greet();
来源：http://cyz.chenzaomai.com

TS:   super.greet();
来源：http://amr.ppjwa.cn

Java: super.greet();
来源：http://ptu.shanyushiyangtech.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mkw.jqgfzy.top

Ruby: super
来源：http://ame.tian-w.cn

C#:   base.Greet();
来源：http://faz.nanxinkj.top

[G08] 静态方法与属性
来源：http://hti.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://djx.mhx1999.top

PHP:  public static function f() {}
来源：http://xzs.gaohongyu789.top

JS:   static f() {}
来源：http://dqw.uphjek.com

TS:   static f(): void {}
来源：http://isa.epnwcf.com

Java: static void f() {}
来源：http://xwz.ehwqpu.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://kjn.gaohongyu789.top

Ruby: def self.f; end
来源：http://lda.jianghu66.top

C#:   public static void F() {}
来源：http://lav.guowangkeji.top

[G09] 接口 / 抽象类
来源：http://toe.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://tao.feifeiyinyue.top

PHP:  interface Shape { public function area(): float; }
来源：http://iuh.tanke756.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gul.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://eqw.zhongyouzk.top

Java: interface Shape { double area(); }
来源：http://lhl.ppjwa.cn

Go:   type Shape interface { Area() float64 }
来源：http://ase.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xsa.vehdjk.com

C#:   interface IShape { double Area(); }
来源：http://bjo.yj202588.top


<!-- 参考信息 -->
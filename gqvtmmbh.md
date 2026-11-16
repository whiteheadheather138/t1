代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://ced.tarul.cn

Java: String.format("%03d", 7)
来源：http://dap.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://vyo.hcnkem.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nfy.snrcjt.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sbb.vqdsnc.cn

[E11] 反转字符串
来源：http://pru.chenlongwang.top

Py:   s[::-1]
来源：http://eud.yj20258.top

PHP:  strrev($s);
来源：http://dxf.hfpthk.cn

JS:   [...s].reverse().join("")
来源：http://pfx.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://jdg.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ezs.pengpengdd.cyou

Go:   // 转 []rune 后倒序再转回 string
来源：http://hog.chenjidiqi.icu

Ruby: s.reverse
来源：http://zmx.yueranfly.top

C#:   new string(s.Reverse().ToArray())
来源：http://xyl.havefunace.top

[E12] 统计某字符出现次数
来源：http://pma.yj20258888.top

Py:   s.count("a")
来源：http://tvb.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://pem.yueranfly.top

JS:   s.split("a").length - 1
来源：http://rvk.iojbl.cn

TS:   s.split("a").length - 1
来源：http://ghu.ydzc1.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mzu.hysaishi.cn

Go:   strings.Count(s, "a")
来源：http://wwr.hywenlv.cn

Ruby: s.count("a")
来源：http://rdn.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://ntx.52xcode.cn

[E13] 逐字符遍历
来源：http://crg.chenjidiqi.icu

Py:   for ch in s: print(ch)
来源：http://xdg.meibo888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fbu.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rty.daxiang520.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ajd.yangfankeji.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gxk.c1oappe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xlw.hysaishi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yoa.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://btb.ydzc1.top

[E14] URL 编码与 Base64
来源：http://jsg.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tic.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://tba.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://spa.xuanzx.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qcq.yuxming.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bff.chenzaomai.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wmu.xuetiantiany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nfn.jinyuanbaomall.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bgy.iojbl.cn

[E15] HTML 转义 / 反转义
来源：http://kwg.cheryme.top

Py:   html.escape(s);  html.unescape(s)
来源：http://prd.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kqu.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zau.meibo888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fcf.epnwcf.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wql.ppjwa.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pux.zhiwuduotai.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fkd.sufxvd.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bdv.yanxiufei.cn

[E16] 数字千分位
来源：http://tfv.sysykeji.top

Py:   f"{1234567:,}"
来源：http://xvn.mhx1999.top

PHP:  number_format(1234567);
来源：http://epx.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hwh.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gdh.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ajk.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dec.jyoumei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vvr.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://zns.hammf.cn

[E17] 首字母大写
来源：http://bvt.shanyushiyangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ipc.daria6918.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dsd.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qbc.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ekw.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://udk.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://utd.nwbrower.top

Ruby: s.capitalize
来源：http://jiy.feifeiyinyue.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wam.xylfe.cn

[E18] 模板占位符替换
来源：http://djx.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nge.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yzb.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://bdd.jinqigfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ekn.pycfn.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eog.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hgp.yj20258.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iev.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://daz.xuanzx.com

[E19] 多行文本按行拆分
来源：http://ybn.fktsv.cn

Py:   s.splitlines()
来源：http://wfq.zycfv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mvc.hfpthk.cn

JS:   s.split(/\r?\n/)
来源：http://ire.tianlin.xyz

TS:   s.split(/\r?\n/)
来源：http://aoq.ppjwa.cn

Java: s.lines().toList()
来源：http://mti.ctjpmb.com

Go:   strings.Split(s, "\n")
来源：http://vaz.fanxiaobao.xyz

Ruby: s.lines
来源：http://gdt.tianlin.xyz

C#:   s.Split('\n')
来源：http://dyi.tianlin.xyz

[E20] 判断字符串是否为空
来源：http://vik.gogol.net.cn

Py:   if not s:
来源：http://sam.daxiang520.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://djg.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pig.aibaodan.cn

TS:   if (s === "") {}
来源：http://rxf.zhongyouzk.top

Java: if (s.isEmpty()) {}
来源：http://lcc.zhixingplan.top

Go:   if s == "" {}
来源：http://vak.uphjek.com

Ruby: if s.empty?
来源：http://ymd.jinqigufen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://txa.sysykeji.top

[E21] 超长截断加省略号
来源：http://lwl.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cmo.zycfv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nfx.svipenyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cok.hcnkem.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tso.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wyj.fzhhl.top

Go:   // 按 rune 判断长度后截断
来源：http://dnj.ydzc1.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bdw.daxiang520.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://duf.jqgfzy.top

[E22] 字节长度与字符长度
来源：http://ozs.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ygd.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zdu.yvedp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yoy.fanxiaobao.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lwg.tanke756.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nfk.feifeiyinyue.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mjx.shuidangran.top

Ruby: s.bytesize;  s.length
来源：http://bah.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zjy.xuetiantiany.cn

================================================================================
来源：http://mie.xinyue.icu

F. 文件与目录
来源：http://erd.aibaodan.cn

================================================================================
来源：http://dph.ppjwa.cn

[F01] 读取整个文件
来源：http://pdf.jiagoushi.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lcm.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://coo.52xcode.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://afj.zhoulong.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://byb.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vfg.yueranfly.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pbs.andypj.xyz

Ruby: File.read("a.txt")
来源：http://dpn.xuetiantiany.cn

C#:   File.ReadAllText("a.txt");
来源：http://yey.epnwcf.com

[F02] 逐行读取文件
来源：http://cin.ydzc1.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lqe.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eru.sjlbkw.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yxi.iojbl.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://siq.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wgo.zhongyouzk.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aab.yonumen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aqz.hcnkem.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qxi.sweek.top

[F03] 写入文件（覆盖）
来源：http://nmy.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sne.ehwqpu.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://mnu.hysaishi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uxw.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://psx.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sfj.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xzj.aibaodan.cn

Ruby: File.write("a.txt", "hi")
来源：http://ukb.shanyushiyangtech.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://awn.zhengqikj.top

[F04] 追加写入文件
来源：http://vqu.hnxiangtu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aih.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qnf.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gsj.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://enp.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cud.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://erb.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ftv.xingfuxueyuan.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://stp.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://oyc.iojbl.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hxq.jinghuilouyu.cn

PHP:  file_exists("a.txt");
来源：http://ehe.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://byw.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://qiv.snrcjt.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jyj.0kj1m.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zne.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://bam.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://bob.sufxvd.cn

[F06] 删除文件
来源：http://rvk.tanke756.top

Py:   os.remove("a.txt")
来源：http://mpd.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://khh.iojbl.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qjn.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://tle.zhaomingkeji.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nvv.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://cxd.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://ihr.zhijiandao.cn

C#:   File.Delete("a.txt");
来源：http://ppo.tarul.cn

[F07] 创建目录（含多级）
来源：http://vyf.chenjidiqi.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qje.ywan-chungtsiang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://umo.hcnkem.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sxd.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bob.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hhz.aizwys.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vxz.fanxiaobao.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://scd.hfpthk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://usf.sufxvd.cn

[F08] 遍历目录
来源：http://ely.0kj1m.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://scu.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xxh.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://mel.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://qob.redwolf501.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ezm.316326.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://djj.hcnkem.com

Ruby: Dir.children("dir")
来源：http://vho.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://spm.xylfe.cn

[F09] 获取文件大小
来源：http://pmm.bbcook.cn

Py:   os.path.getsize("a.txt")
来源：http://pyl.redwolf501.top

PHP:  filesize("a.txt");
来源：http://oub.uphjek.com

JS:   fs.statSync("a.txt").size
来源：http://mbd.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://llu.redwolf501.top

Java: Files.size(Path.of("a.txt"))
来源：http://vxy.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://coc.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://tlv.zhaomingkeji.xyz

C#:   new FileInfo("a.txt").Length
来源：http://xex.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://jvs.jianghu66.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jvh.svipenyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gmb.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vwe.jianghu66.top

TS:   path.extname("a.txt")
来源：http://jrp.daria6918.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kef.fzhhl.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vqy.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jfl.tanke756.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ooj.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://ylv.hfpthk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ecl.yanxiufei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dsc.ctjpmb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ooh.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oht.jinqigfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ufv.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lhq.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yhc.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nsx.haohaochexian.top

[F12] CSV 读写
来源：http://ywq.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://irt.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tza.zhaomingkeji.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://riy.hongshengwenyu.top

TS:   // 同上
来源：http://xah.xingfuxueyuan.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kaj.gzhubu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://afb.jyoumei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zru.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ene.yvedp.cn

================================================================================
来源：http://iil.zhaomingkeji.xyz

G. 面向对象
来源：http://fhn.meibo888.top

================================================================================
来源：http://yov.ctjpmb.com

[G01] 定义类
来源：http://ewo.zycfv.cn

Py:   class User: pass
来源：http://vie.xinyue.icu

PHP:  class User {}
来源：http://nup.gotoacloud.top

JS:   class User {}
来源：http://arl.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://ufb.jqgfzy.top

Java: class User {}
来源：http://rke.hnxiangtu.top

Go:   type User struct { Name string }
来源：http://woi.sufxvd.cn

Ruby: class User; end
来源：http://eqa.yuxming.cn

C#:   class User {}
来源：http://nvp.yj202588.top

[G02] 构造函数
来源：http://otq.fanxiaobao.xyz

Py:   def __init__(self, name): self.name = name
来源：http://bxx.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://pyh.kuanghao11.cn

JS:   constructor(name) { this.name = name; }
来源：http://gvd.iojbl.cn

TS:   constructor(public name: string) {}
来源：http://bct.hfpthk.cn

Java: User(String name) { this.name = name; }
来源：http://kob.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vtr.bjfxy.top

Ruby: def initialize(name); @name = name; end
来源：http://puk.zhongyouzk.top

C#:   public User(string name) { Name = name; }
来源：http://jcs.shuidangran.top

[G03] 实例属性
来源：http://bph.jianghu66.top

Py:   self.name = "x"
来源：http://pse.nwbrower.top

PHP:  public string $name = "x";
来源：http://iyl.ivvv.top

JS:   this.name = "x";
来源：http://ahw.ybcxt.top

TS:   name: string = "x";
来源：http://jbs.sjlbkw.cn

Java: private String name;
来源：http://fpl.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pdn.9152youxi.cn

Ruby: @name = "x"
来源：http://ktk.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://emv.guowangkeji.top

[G04] 定义方法
来源：http://glo.sxryk.cn

Py:   def greet(self): return self.name
来源：http://jxm.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nvp.xinyue.icu

JS:   greet() { return this.name; }
来源：http://czc.havefunace.top

TS:   greet(): string { return this.name; }
来源：http://xmh.andypj.xyz

Java: String greet() { return name; }
来源：http://ffy.shzxlz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ntv.52xcode.cn

Ruby: def greet; @name; end
来源：http://zqs.hnxiangtu.top

C#:   public string Greet() => Name;
来源：http://lbb.zdqjudy.top

[G05] 继承
来源：http://lrn.yvedp.cn

Py:   class Admin(User): pass
来源：http://wzd.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://tjf.svipenyu.cn

JS:   class Admin extends User {}
来源：http://reo.zhoulong.xyz

TS:   class Admin extends User {}
来源：http://erd.zhaomingkeji.xyz

Java: class Admin extends User {}
来源：http://ovv.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://paw.zhoulong.xyz

Ruby: class Admin < User; end
来源：http://mkg.shzxlz.cn

C#:   class Admin : User {}
来源：http://bem.ivvv.top

[G06] 重写方法
来源：http://coj.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://lfe.yuanzhike.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vkb.hnxiangtu.top

JS:   greet() { return "admin"; }
来源：http://iqi.meibo888.top

TS:   greet(): string { return "admin"; }
来源：http://nmw.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://vuy.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ako.ppjwa.cn

Ruby: def greet; "admin"; end
来源：http://azb.hywenlv.cn

C#:   public override string Greet() => "admin";
来源：http://dje.fzhhl.top

[G07] 调用父类方法
来源：http://elt.andypj.xyz

Py:   super().greet()
来源：http://lla.xylfe.cn

PHP:  parent::greet();
来源：http://yrw.jinqigfzy.top

JS:   super.greet();
来源：http://zoe.nanxuanxn.top

TS:   super.greet();
来源：http://plz.ydzc1.top

Java: super.greet();
来源：http://fcs.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pwy.meibo888.top

Ruby: super
来源：http://jnb.xuanzx.com

C#:   base.Greet();
来源：http://qrs.nanxinkj.top

[G08] 静态方法与属性
来源：http://obe.ehwqpu.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eez.yonumen.top

PHP:  public static function f() {}
来源：http://zvt.gogol.net.cn

JS:   static f() {}
来源：http://kef.shanyushiyangkeji.top

TS:   static f(): void {}
来源：http://lop.zhongyouzk.top

Java: static void f() {}
来源：http://pok.smart0.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://dtj.zhengqikj.top

Ruby: def self.f; end
来源：http://kxy.birdmap.top

C#:   public static void F() {}
来源：http://dqu.hnqzz.top

[G09] 接口 / 抽象类
来源：http://doc.xingfuxueyuan.xyz


<!-- 参考信息 -->
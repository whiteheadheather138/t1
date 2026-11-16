代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://lkp.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hue.xinyue.icu

Ruby: s.gsub(/\s+/, "")
来源：http://hom.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rrp.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://omc.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cuf.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nqk.c1oappe.top

JS:   "7".padStart(3, "0")
来源：http://tpq.svipenyu.cn

TS:   "7".padStart(3, "0")
来源：http://ogk.feifeiyinyue.top

Java: String.format("%03d", 7)
来源：http://xng.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://iqz.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bco.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mjt.yanxiufei.cn

[E11] 反转字符串
来源：http://ala.snrcjt.cn

Py:   s[::-1]
来源：http://ezc.svipenyu.cn

PHP:  strrev($s);
来源：http://sle.guowangkeji.top

JS:   [...s].reverse().join("")
来源：http://skg.aibaodan.cn

TS:   [...s].reverse().join("")
来源：http://iwv.ydzc1.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jkl.bbcook.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pot.wangdashe.top

Ruby: s.reverse
来源：http://ftd.ivvv.top

C#:   new string(s.Reverse().ToArray())
来源：http://mqf.yfazqb.com

[E12] 统计某字符出现次数
来源：http://jah.havefunace.top

Py:   s.count("a")
来源：http://ydx.yj202588.top

PHP:  substr_count($s, "a");
来源：http://dis.jlsjyb.cn

JS:   s.split("a").length - 1
来源：http://gcc.yj20258888.top

TS:   s.split("a").length - 1
来源：http://fmy.ywan-chungtsiang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cji.hfpthk.cn

Go:   strings.Count(s, "a")
来源：http://vqn.ybcxt.top

Ruby: s.count("a")
来源：http://kjb.xinyue.icu

C#:   s.Count(c => c == 'a')
来源：http://zge.fengsongda.top

[E13] 逐字符遍历
来源：http://cyb.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://net.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qgb.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dis.mhx1999.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wrr.quarkkingdee.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fiv.daria6918.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dpg.fengsongda.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xxs.vehdjk.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dpo.pycfn.com

[E14] URL 编码与 Base64
来源：http://weq.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kcr.shanyushiyangtech.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dfp.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vxw.jinqigfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cwa.cheryme.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aer.c1oappe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xvm.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ceg.dashuyun.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yqs.havefunace.top

[E15] HTML 转义 / 反转义
来源：http://tuw.tianlin.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://cur.nanxuanxn.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sqz.tianlin.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vjv.shanyushiyangtech.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fzl.haohaochexian.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ges.xziqi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zks.c1oappe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yzn.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bha.hysaishi.cn

[E16] 数字千分位
来源：http://uzn.uphjek.com

Py:   f"{1234567:,}"
来源：http://hfq.snrcjt.cn

PHP:  number_format(1234567);
来源：http://vlt.zdbjq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rfg.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wvf.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kfp.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vvw.gzhubu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uax.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://fgy.xuetiantiany.cn

[E17] 首字母大写
来源：http://qhz.sysykeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ife.fengsongda.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gvq.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fke.jiagoushi.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dfg.wangdashe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pmc.xuetiantiany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ypz.xziqi.cn

Ruby: s.capitalize
来源：http://crx.daria6918.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://prl.yuxming.cn

[E18] 模板占位符替换
来源：http://ytx.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zit.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nqv.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vcz.hesvh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tqy.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xpg.svipenyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kah.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pwp.uphjek.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lod.tarul.cn

[E19] 多行文本按行拆分
来源：http://ain.aibaodan.cn

Py:   s.splitlines()
来源：http://dob.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ren.svipenyu.cn

JS:   s.split(/\r?\n/)
来源：http://eqq.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://ofj.sysykeji.top

Java: s.lines().toList()
来源：http://agn.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://gxz.xuetiantiany.cn

Ruby: s.lines
来源：http://ljo.smart0.xyz

C#:   s.Split('\n')
来源：http://tss.nanxinkj.top

[E20] 判断字符串是否为空
来源：http://cpf.redwolf501.top

Py:   if not s:
来源：http://xuk.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sye.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eyy.gzhubu.top

TS:   if (s === "") {}
来源：http://ohi.kuanghao11.cn

Java: if (s.isEmpty()) {}
来源：http://kqe.birdmap.top

Go:   if s == "" {}
来源：http://kzr.ppjwa.cn

Ruby: if s.empty?
来源：http://eku.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kro.sjlbkw.cn

[E21] 超长截断加省略号
来源：http://cfk.andypj.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gjn.aibaodan.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lkd.tarul.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tss.nanxuanxn.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dhq.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jqc.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://wjg.hesvh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zfe.zhixingplan.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nyg.feifeiyinyue.top

[E22] 字节长度与字符长度
来源：http://nvz.chenlongwang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fap.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fxq.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hyo.ivvv.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iju.xuetiantiany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://owy.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ual.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://wsp.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pxl.tarul.cn

================================================================================
来源：http://ozg.chenjidiqi.icu

F. 文件与目录
来源：http://rnu.pengpengdd.cyou

================================================================================
来源：http://xhd.nwbrower.top

[F01] 读取整个文件
来源：http://acw.meibo888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ftq.ybcxt.top

PHP:  file_get_contents("a.txt");
来源：http://obq.jianghu66.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bzc.vehdjk.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cem.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://jvc.nanxuanxn.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bqa.ppjwa.cn

Ruby: File.read("a.txt")
来源：http://xfk.tanke756.top

C#:   File.ReadAllText("a.txt");
来源：http://dav.hammf.cn

[F02] 逐行读取文件
来源：http://avt.ywan-chungtsiang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rpw.hnqzz.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qlt.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://scm.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zci.zhaomingkeji.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nlf.tanke756.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ctw.fengsongda.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rkr.yueranfly.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://btc.quarkkingdee.top

[F03] 写入文件（覆盖）
来源：http://aax.cdnleiting.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://exh.wangdashe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://oze.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aay.birdmap.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ovo.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tzn.52xcode.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gbf.ydjk.org.cn

Ruby: File.write("a.txt", "hi")
来源：http://psk.yj202588.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sdh.jinghuilouyu.cn

[F04] 追加写入文件
来源：http://ori.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wxk.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qgv.hnxiangtu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://azm.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vjs.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uho.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jwq.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vwc.jinqigfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ben.chenjidiqi.icu

[F05] 判断文件或目录是否存在
来源：http://yic.hcnkem.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yrv.epnwcf.com

PHP:  file_exists("a.txt");
来源：http://nja.zhaomingkeji.xyz

JS:   fs.existsSync("a.txt")
来源：http://xzl.meibo888.top

TS:   fs.existsSync("a.txt")
来源：http://eyr.daxiang520.top

Java: Files.exists(Path.of("a.txt"))
来源：http://shf.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bxi.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://ezy.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://ewc.zdqjudy.top

[F06] 删除文件
来源：http://kbf.fengsongda.top

Py:   os.remove("a.txt")
来源：http://rjm.feifeiyinyue.top

PHP:  unlink("a.txt");
来源：http://rfo.yueranfly.top

JS:   fs.unlinkSync("a.txt")
来源：http://zhl.fanxiaobao.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://ypc.hcnkem.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hqz.sysykeji.top

Go:   os.Remove("a.txt")
来源：http://rjb.wangshuangyany.cn

Ruby: File.delete("a.txt")
来源：http://zdv.yongpay.top

C#:   File.Delete("a.txt");
来源：http://kuy.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://kpj.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uod.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://erq.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ycw.shangyingyoupin.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cdg.aibaodan.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zbo.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gcq.xuetiantiany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qeo.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://apb.gzhubu.top

[F08] 遍历目录
来源：http://upk.kuanghao11.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ipn.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uwq.ydjk.org.cn

JS:   fs.readdirSync("dir")
来源：http://onf.ctjpmb.com

TS:   fs.readdirSync("dir")
来源：http://ghh.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gxf.pycfn.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://xmx.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://ewe.cucudq.cn

C#:   Directory.GetFiles("dir")
来源：http://pgz.mhx1999.top

[F09] 获取文件大小
来源：http://jof.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://zuk.xinyue.icu

PHP:  filesize("a.txt");
来源：http://aae.yanxiufei.cn

JS:   fs.statSync("a.txt").size
来源：http://hvd.chenzaomai.com

TS:   fs.statSync("a.txt").size
来源：http://xdu.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://chp.hcnkem.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jtt.cucudq.cn

Ruby: File.size("a.txt")
来源：http://ehg.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://cfb.jinyuanbaomall.cn

[F10] 取文件扩展名 / 文件名
来源：http://fcb.yongpay.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qvc.wangshuangyany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gml.sufxvd.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ufz.52xcode.cn

TS:   path.extname("a.txt")
来源：http://mfv.cqqwz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hes.shzxlz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wdv.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hsh.fehbvm.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://skj.tanke756.top

[F11] 复制与移动文件
来源：http://nts.zdbjq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xhk.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hlj.ydjk.org.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ged.wangdashe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uhx.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://din.zycfv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wvy.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xvq.jlsjyb.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://atc.hfpthk.cn

[F12] CSV 读写
来源：http://owt.xylfe.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bmg.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yje.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pws.tanke756.top

TS:   // 同上
来源：http://loc.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vcs.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://epn.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cci.zycfv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://roi.hywenlv.cn

================================================================================
来源：http://vwq.yvedp.cn

G. 面向对象
来源：http://vye.jinghuilouyu.cn

================================================================================
来源：http://aqc.nanxinkj.top

[G01] 定义类
来源：http://gds.xingfuxueyuan.xyz

Py:   class User: pass
来源：http://rup.yfazqb.com

PHP:  class User {}
来源：http://cvu.chenlongwang.top

JS:   class User {}
来源：http://egd.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://emf.aibaodan.cn

Java: class User {}
来源：http://tbp.mhx1999.top

Go:   type User struct { Name string }
来源：http://cwo.sysykeji.top

Ruby: class User; end
来源：http://qda.jqgfzy.top

C#:   class User {}
来源：http://qxt.yonumen.top

[G02] 构造函数
来源：http://ngc.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://bkz.gogol.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://zqc.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://awx.fehbvm.com

TS:   constructor(public name: string) {}
来源：http://mij.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://jmk.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://deu.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://rnt.hammf.cn

C#:   public User(string name) { Name = name; }
来源：http://uuq.fzhhl.top

[G03] 实例属性
来源：http://xpj.feifeiyinyue.top

Py:   self.name = "x"
来源：http://kmc.ehwqpu.com

PHP:  public string $name = "x";
来源：http://srr.yuanzhike.top

JS:   this.name = "x";
来源：http://dox.birdmap.top

TS:   name: string = "x";
来源：http://mpt.xuetiantiany.cn

Java: private String name;
来源：http://fwc.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yjp.yj20258.top

Ruby: @name = "x"
来源：http://adn.xuetiantiany.cn

C#:   public string Name { get; set; } = "x";
来源：http://jgw.yonumen.top

[G04] 定义方法
来源：http://alo.fktsv.cn

Py:   def greet(self): return self.name
来源：http://jna.sxryk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ozb.shzxlz.cn

JS:   greet() { return this.name; }
来源：http://xft.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://eth.hywenlv.cn

Java: String greet() { return name; }
来源：http://kva.cashguo.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wpq.bbcook.cn

Ruby: def greet; @name; end
来源：http://mzo.hesvh.cn

C#:   public string Greet() => Name;
来源：http://vzi.smart0.xyz

[G05] 继承
来源：http://jcg.wangdashe.top

Py:   class Admin(User): pass
来源：http://ppp.gotoacloud.top

PHP:  class Admin extends User {}
来源：http://isc.yongpay.top

JS:   class Admin extends User {}
来源：http://jdh.shuidangran.top

TS:   class Admin extends User {}
来源：http://ulb.jqgfzy.top

Java: class Admin extends User {}
来源：http://fik.sxryk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://did.hfpthk.cn

Ruby: class Admin < User; end
来源：http://wbl.aizwys.cn

C#:   class Admin : User {}
来源：http://tys.aibaodan.cn

[G06] 重写方法
来源：http://drh.tianlin.xyz

Py:   def greet(self): return "admin"
来源：http://vwr.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://mkp.jinqigfzy.top

JS:   greet() { return "admin"; }
来源：http://oje.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://vwp.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://umk.xuetiantiany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zjf.jiagoushi.top

Ruby: def greet; "admin"; end
来源：http://qwl.quarkkingdee.top

C#:   public override string Greet() => "admin";
来源：http://ily.daria6918.cn

[G07] 调用父类方法
来源：http://ziy.ydjk.org.cn

Py:   super().greet()
来源：http://dpb.jyoumei.cn

PHP:  parent::greet();
来源：http://qfv.ehwqpu.com

JS:   super.greet();
来源：http://vgo.zhijiandao.cn

TS:   super.greet();
来源：http://tak.cashguo.top

Java: super.greet();
来源：http://ypx.ydjk.org.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://igh.chenzaomai.com

Ruby: super
来源：http://lhg.redwolf501.top

C#:   base.Greet();
来源：http://prz.gaohongyu789.top

[G08] 静态方法与属性
来源：http://akd.sweek.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kfk.cqqwz.cn


<!-- 参考信息 -->
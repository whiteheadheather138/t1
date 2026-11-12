代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qzd.ivvv.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sut.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://alu.andypj.xyz

TS:   s.replace(/\s+/g, "")
来源：http://lyu.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://xke.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jpw.fktsv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dnr.bbcook.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ryr.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://rxr.shangyingyoupin.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mwb.jinghuilouyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://too.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://cjc.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://jhr.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://rwj.sweek.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://oec.ybcxt.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yjh.yanxiufei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yrz.ywan-chungtsiang.top

[E11] 反转字符串
来源：http://eqb.nanxinkj.top

Py:   s[::-1]
来源：http://idx.ppjwa.cn

PHP:  strrev($s);
来源：http://ian.fzhhl.top

JS:   [...s].reverse().join("")
来源：http://pen.yvedp.cn

TS:   [...s].reverse().join("")
来源：http://zkk.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://uph.ydjk.org.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jji.andypj.xyz

Ruby: s.reverse
来源：http://iqj.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://jpq.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://qfk.nanxuanxn.top

Py:   s.count("a")
来源：http://sxy.52xcode.cn

PHP:  substr_count($s, "a");
来源：http://xrs.fktsv.cn

JS:   s.split("a").length - 1
来源：http://xus.fengsongda.top

TS:   s.split("a").length - 1
来源：http://csd.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://deh.wangdashe.top

Go:   strings.Count(s, "a")
来源：http://kuj.guannengcc.top

Ruby: s.count("a")
来源：http://pdo.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://tzx.hnqzz.top

[E13] 逐字符遍历
来源：http://mil.c1oappe.top

Py:   for ch in s: print(ch)
来源：http://qsr.ybcxt.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zxv.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ewd.cashguo.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://knq.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aiw.fengsongda.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ipo.52xcode.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zsg.tarul.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eex.jinqigufen.top

[E14] URL 编码与 Base64
来源：http://kqn.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qth.cdnleiting.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xcd.ywan-chungtsiang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://han.jinqigufen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ztz.jqgfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vzm.nanxinkj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://htz.cheryme.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ddv.zdqjudy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hme.mhx1999.top

[E15] HTML 转义 / 反转义
来源：http://yub.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qiu.zhengqikj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kxk.shuidangran.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cfd.xinyue.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://uwl.hnxiangtu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lvk.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xtb.yj202588.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qzk.hongshengwenyu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lqf.sweek.top

[E16] 数字千分位
来源：http://pqb.birdmap.top

Py:   f"{1234567:,}"
来源：http://axz.jinghuilouyu.cn

PHP:  number_format(1234567);
来源：http://cli.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mqv.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zzj.havefunace.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ewb.xylfe.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cke.xinyue.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mlg.52xcode.cn

C#:   1234567.ToString("N0")
来源：http://rjo.nanxuanxn.top

[E17] 首字母大写
来源：http://gur.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nan.gaohongyu789.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://upd.jqgufenzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ujk.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mkx.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qwf.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nnx.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://kqp.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blb.jlsjyb.cn

[E18] 模板占位符替换
来源：http://pvz.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tmc.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://itb.0kj1m.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xou.zhijiandao.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://enx.yuxming.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nig.sufxvd.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lzh.dashuyun.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://igo.nanxinkj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bgb.guowangkeji.top

[E19] 多行文本按行拆分
来源：http://leo.yangfankeji.com

Py:   s.splitlines()
来源：http://ake.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hgp.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://uzm.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://skl.zhijiandao.cn

Java: s.lines().toList()
来源：http://nvh.52xcode.cn

Go:   strings.Split(s, "\n")
来源：http://adn.cqqwz.cn

Ruby: s.lines
来源：http://uqy.fktsv.cn

C#:   s.Split('\n')
来源：http://xha.tarul.cn

[E20] 判断字符串是否为空
来源：http://cep.tarul.cn

Py:   if not s:
来源：http://nyp.haohaochexian.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uwu.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dbd.shzxlz.cn

TS:   if (s === "") {}
来源：http://ijk.sweek.top

Java: if (s.isEmpty()) {}
来源：http://gil.zhiwuduotai.top

Go:   if s == "" {}
来源：http://snn.chenjidiqi.icu

Ruby: if s.empty?
来源：http://vck.yj202588.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zay.ppjwa.cn

[E21] 超长截断加省略号
来源：http://qly.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://juk.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pvr.ehwqpu.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qua.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pfj.tanke756.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ofz.zycfv.cn

Go:   // 按 rune 判断长度后截断
来源：http://trx.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tux.tarul.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ekn.hnqzz.top

[E22] 字节长度与字符长度
来源：http://ghb.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qmb.fanxiaobao.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ckn.uphjek.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cqr.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cvq.cdnleiting.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://njf.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ute.ydzc1.top

Ruby: s.bytesize;  s.length
来源：http://gmf.snrcjt.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qws.jinqigufen.top

================================================================================
来源：http://gkg.cheryme.top

F. 文件与目录
来源：http://meo.fktsv.cn

================================================================================
来源：http://xky.chenjidiqi.icu

[F01] 读取整个文件
来源：http://pyq.xylfe.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dzw.xingfuxueyuan.xyz

PHP:  file_get_contents("a.txt");
来源：http://rdl.gotoacloud.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cov.tarul.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xvm.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://sqe.sjlbkw.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://awp.hnxiangtu.top

Ruby: File.read("a.txt")
来源：http://qox.sweek.top

C#:   File.ReadAllText("a.txt");
来源：http://uca.chenlongwang.top

[F02] 逐行读取文件
来源：http://jdj.pycfn.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://amr.xylfe.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gpo.jiagoushi.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rbj.feifeiyinyue.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rpk.pengpengdd.cyou

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eye.yj20258.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ejc.cucudq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://skl.fehbvm.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rhu.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://wxe.c1oappe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://loo.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://iih.zdqjudy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cnc.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://osx.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cip.guannengcc.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kkv.tian-w.cn

Ruby: File.write("a.txt", "hi")
来源：http://zhu.jqgfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mgg.shzxlz.cn

[F04] 追加写入文件
来源：http://inm.zhengqikj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wrt.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ted.zdbjq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://saa.zycfv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rub.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ago.guowangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wmk.nanxinkj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ttx.9152youxi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eks.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://dnj.ydjk.org.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zat.jianghu66.top

PHP:  file_exists("a.txt");
来源：http://avf.chenjidiqi.icu

JS:   fs.existsSync("a.txt")
来源：http://omw.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://eqc.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bdr.hywenlv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fix.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://qwp.shanyushiyangtech.top

C#:   File.Exists("a.txt")
来源：http://bmd.zhengqikj.top

[F06] 删除文件
来源：http://hts.yvedp.cn

Py:   os.remove("a.txt")
来源：http://pqa.tian-w.cn

PHP:  unlink("a.txt");
来源：http://wdg.vehdjk.com

JS:   fs.unlinkSync("a.txt")
来源：http://lca.fzhhl.top

TS:   fs.unlinkSync("a.txt")
来源：http://wbk.ywan-chungtsiang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rlt.jqgfzy.top

Go:   os.Remove("a.txt")
来源：http://rxn.daxiang520.top

Ruby: File.delete("a.txt")
来源：http://yqg.zhaomingkeji.xyz

C#:   File.Delete("a.txt");
来源：http://mom.mhx1999.top

[F07] 创建目录（含多级）
来源：http://dph.jinghuilouyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vru.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bar.aibaodan.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vwa.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vza.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ike.fzhhl.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://saq.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jou.sysykeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://snw.kuanghao11.cn

[F08] 遍历目录
来源：http://nmt.xziqi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ypx.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://neo.meibo888.top

JS:   fs.readdirSync("dir")
来源：http://ign.fzhhl.top

TS:   fs.readdirSync("dir")
来源：http://vua.fktsv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://klf.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lbm.zhixingplan.top

Ruby: Dir.children("dir")
来源：http://mvq.hcnkem.com

C#:   Directory.GetFiles("dir")
来源：http://eup.ydjk.org.cn

[F09] 获取文件大小
来源：http://vmm.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://gwy.yanxiufei.cn

PHP:  filesize("a.txt");
来源：http://czw.ehwqpu.com

JS:   fs.statSync("a.txt").size
来源：http://uik.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://kst.316326.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://lqp.zhongyouzk.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hoz.zdqjudy.top

Ruby: File.size("a.txt")
来源：http://gow.svipenyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://wly.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://jvb.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ehf.yanxiufei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ryj.tian-w.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vnj.snrcjt.cn

TS:   path.extname("a.txt")
来源：http://rbv.hammf.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kwy.pycfn.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ovo.tanke756.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qdu.sjlbkw.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gww.haohaochexian.top

[F11] 复制与移动文件
来源：http://pnf.cucudq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qah.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yse.yuanzhike.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zad.yj20258888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fga.dianchejie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://snm.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jsh.zhixingplan.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ipw.52xcode.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ykv.redwolf501.top

[F12] CSV 读写
来源：http://mmc.jinyuanbaomall.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://edb.gzhubu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hmj.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yqk.316326.xyz

TS:   // 同上
来源：http://ati.sjlbkw.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://odv.ydjk.org.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://spv.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ors.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wle.hongshengwenyu.top

================================================================================
来源：http://aqg.dianchejie.cn

G. 面向对象
来源：http://eqd.sjlbkw.cn

================================================================================
来源：http://vsa.nanxuanxn.top

[G01] 定义类
来源：http://udk.tanke756.top

Py:   class User: pass
来源：http://csr.feifeiyinyue.top

PHP:  class User {}
来源：http://mpm.xziqi.cn

JS:   class User {}
来源：http://yua.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://qux.yj20258.top

Java: class User {}
来源：http://zjh.yongpay.top

Go:   type User struct { Name string }
来源：http://qyx.aibaodan.cn

Ruby: class User; end
来源：http://boz.xuanzx.com

C#:   class User {}
来源：http://ihc.hammf.cn

[G02] 构造函数
来源：http://ddy.xingfuxueyuan.xyz

Py:   def __init__(self, name): self.name = name
来源：http://zyn.gogol.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://gvj.zdbjq.cn

JS:   constructor(name) { this.name = name; }
来源：http://emo.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://loa.yueranfly.top

Java: User(String name) { this.name = name; }
来源：http://auz.zhengqikj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ilg.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://ecb.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://rvm.yongpay.top

[G03] 实例属性
来源：http://drk.gogol.net.cn

Py:   self.name = "x"
来源：http://liq.zhijiandao.cn

PHP:  public string $name = "x";
来源：http://enl.fktsv.cn

JS:   this.name = "x";
来源：http://jqq.chenzaomai.com

TS:   name: string = "x";
来源：http://fuu.zhiwuduotai.top

Java: private String name;
来源：http://dzp.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tqp.wangdashe.top

Ruby: @name = "x"
来源：http://nse.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://ayq.zhaomingkeji.xyz

[G04] 定义方法
来源：http://eag.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://aqm.9152youxi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vrx.nanxinkj.top

JS:   greet() { return this.name; }
来源：http://ofc.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://vqt.andypj.xyz

Java: String greet() { return name; }
来源：http://rfp.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://upq.ybcxt.top

Ruby: def greet; @name; end
来源：http://ckl.tian-w.cn

C#:   public string Greet() => Name;
来源：http://bqy.fktsv.cn

[G05] 继承
来源：http://wve.yangfankeji.com

Py:   class Admin(User): pass
来源：http://gtd.yj20258888.top

PHP:  class Admin extends User {}
来源：http://lio.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://imo.hesvh.cn

TS:   class Admin extends User {}
来源：http://bab.ehwqpu.com

Java: class Admin extends User {}
来源：http://uoi.fengsongda.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uze.aibaodan.cn

Ruby: class Admin < User; end
来源：http://eug.ctjpmb.com

C#:   class Admin : User {}
来源：http://atf.cucudq.cn

[G06] 重写方法
来源：http://npd.birdmap.top

Py:   def greet(self): return "admin"
来源：http://thp.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qmj.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://stn.daxiang520.top

TS:   greet(): string { return "admin"; }
来源：http://wbl.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://smf.wangdashe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pgv.guowangkeji.top

Ruby: def greet; "admin"; end
来源：http://ypi.chenzaomai.com

C#:   public override string Greet() => "admin";
来源：http://jpz.smart0.xyz

[G07] 调用父类方法
来源：http://jxw.yj20258888.top

Py:   super().greet()
来源：http://ebu.hfpthk.cn

PHP:  parent::greet();
来源：http://pga.epnwcf.com

JS:   super.greet();
来源：http://bbx.daxiang520.top

TS:   super.greet();
来源：http://iku.hongshengwenyu.top

Java: super.greet();
来源：http://sts.gogol.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jhc.cucudq.cn


<!-- 参考信息 -->
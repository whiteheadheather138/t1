代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ogn.xuanzx.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gmk.yj20258888.top

JS:   s.replace(/\s+/g, "")
来源：http://jgf.daria6918.cn

TS:   s.replace(/\s+/g, "")
来源：http://qxq.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://jbc.zdbjq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lsb.yj20258.top

Ruby: s.gsub(/\s+/, "")
来源：http://hap.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bdr.andypj.xyz

[E10] 左侧补零 / 定长填充
来源：http://gdk.hongshengwenyu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eyh.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ixi.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://ikb.jinyuanbaomall.cn

TS:   "7".padStart(3, "0")
来源：http://esj.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://jxl.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wne.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jgy.yangfankeji.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uyv.yj20258.top

[E11] 反转字符串
来源：http://exh.fktsv.cn

Py:   s[::-1]
来源：http://hlv.ywan-chungtsiang.top

PHP:  strrev($s);
来源：http://zzv.birdmap.top

JS:   [...s].reverse().join("")
来源：http://ucw.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://ntc.pycfn.com

Java: new StringBuilder(s).reverse().toString()
来源：http://wzc.yonumen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gaf.andypj.xyz

Ruby: s.reverse
来源：http://jgo.jinqigfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://dxi.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://wim.hammf.cn

Py:   s.count("a")
来源：http://lca.fanxiaobao.xyz

PHP:  substr_count($s, "a");
来源：http://vuu.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://tmy.redwolf501.top

TS:   s.split("a").length - 1
来源：http://lhz.c1oappe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rur.sufxvd.cn

Go:   strings.Count(s, "a")
来源：http://hmp.sweek.top

Ruby: s.count("a")
来源：http://egj.tian-w.cn

C#:   s.Count(c => c == 'a')
来源：http://ftt.guannengcc.top

[E13] 逐字符遍历
来源：http://sia.andypj.xyz

Py:   for ch in s: print(ch)
来源：http://ibh.pengpengdd.cyou

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vks.vehdjk.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://zul.wangshuangyany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://irf.fehbvm.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ftn.yfazqb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tju.yangfankeji.com

Ruby: s.each_char { |ch| puts ch }
来源：http://ltr.yfazqb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vnb.daria6918.cn

[E14] URL 编码与 Base64
来源：http://baz.hywenlv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iyp.cdnleiting.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cel.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jxb.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pnq.cdnleiting.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qhh.52xcode.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lsl.guowangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dlw.shzxlz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://doh.yanxiufei.cn

[E15] HTML 转义 / 反转义
来源：http://qqd.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ozs.zhoulong.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fgf.hnqzz.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://saf.316326.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://mon.daria6918.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mfb.shzxlz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zqs.zhengqikj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oba.andypj.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://guj.zhixingplan.top

[E16] 数字千分位
来源：http://yxp.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://jmd.xuanzx.com

PHP:  number_format(1234567);
来源：http://wkc.tanke756.top

JS:   (1234567).toLocaleString("en-US")
来源：http://oja.snrcjt.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bcq.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jis.xinyue.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pff.9152youxi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bua.fanxiaobao.xyz

C#:   1234567.ToString("N0")
来源：http://gao.jinqigfzy.top

[E17] 首字母大写
来源：http://wof.jyoumei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tfn.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zis.ivvv.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rcl.hywenlv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vql.0kj1m.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://frn.quarkkingdee.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vjn.shuidangran.top

Ruby: s.capitalize
来源：http://rkv.xuetiantiany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zav.jyoumei.cn

[E18] 模板占位符替换
来源：http://qou.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qxz.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yhb.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tow.zycfv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://doq.bjfxy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://maw.9152youxi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://raa.yongpay.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bga.yongpay.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zwi.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://zke.meibo888.top

Py:   s.splitlines()
来源：http://rhq.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lnm.hcnkem.com

JS:   s.split(/\r?\n/)
来源：http://uwz.yonumen.top

TS:   s.split(/\r?\n/)
来源：http://cwx.zhoulong.xyz

Java: s.lines().toList()
来源：http://pkb.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://tuy.c1oappe.top

Ruby: s.lines
来源：http://xvo.hcnkem.com

C#:   s.Split('\n')
来源：http://dfu.daxiang520.top

[E20] 判断字符串是否为空
来源：http://zvq.jyoumei.cn

Py:   if not s:
来源：http://pey.tianlin.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ark.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gos.daxiang520.top

TS:   if (s === "") {}
来源：http://ebx.shangyingyoupin.top

Java: if (s.isEmpty()) {}
来源：http://nkx.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://glu.zhengqikj.top

Ruby: if s.empty?
来源：http://dlf.zdbjq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rvx.jianghu66.top

[E21] 超长截断加省略号
来源：http://nid.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eip.yongpay.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nut.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ulw.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vil.bjfxy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iyh.fktsv.cn

Go:   // 按 rune 判断长度后截断
来源：http://yac.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wca.tianlin.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mti.redwolf501.top

[E22] 字节长度与字符长度
来源：http://ojc.nanxinkj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://juv.aibaodan.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vmt.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ygz.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vuf.xuetiantiany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://exp.haohaochexian.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gzx.cdnleiting.top

Ruby: s.bytesize;  s.length
来源：http://qzh.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kfm.yueranfly.top

================================================================================
来源：http://wyl.shzxlz.cn

F. 文件与目录
来源：http://kxy.dianchejie.cn

================================================================================
来源：http://xan.jianghu66.top

[F01] 读取整个文件
来源：http://ckz.hysaishi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pjl.yuanzhike.top

PHP:  file_get_contents("a.txt");
来源：http://mjb.nanxuanxn.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jcz.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blq.nanxinkj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ogk.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yom.nanxinkj.top

Ruby: File.read("a.txt")
来源：http://tfg.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://qpu.52xcode.cn

[F02] 逐行读取文件
来源：http://kwi.shzxlz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jps.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hpt.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lzl.shanyushiyangtech.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://naz.nwbrower.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wqa.jinqigufen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kio.wangshuangyany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://exq.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bpf.sweek.top

[F03] 写入文件（覆盖）
来源：http://abp.ywan-chungtsiang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mtk.redwolf501.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wdu.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jei.zhongyouzk.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mhb.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tcr.sjlbkw.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wre.shanyushiyangtech.top

Ruby: File.write("a.txt", "hi")
来源：http://kqs.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sdx.daxiang520.top

[F04] 追加写入文件
来源：http://hqn.ehwqpu.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aks.0kj1m.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kfk.sxryk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://swi.cucudq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xwd.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vdl.sweek.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vtb.cqqwz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hoa.sysykeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ugw.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://fqm.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://scx.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://cza.sjlbkw.cn

JS:   fs.existsSync("a.txt")
来源：http://pag.zhengqikj.top

TS:   fs.existsSync("a.txt")
来源：http://rtg.zhixingplan.top

Java: Files.exists(Path.of("a.txt"))
来源：http://plk.zhijiandao.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vpw.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://sed.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://rpu.daria6918.cn

[F06] 删除文件
来源：http://nnt.ehwqpu.com

Py:   os.remove("a.txt")
来源：http://glz.316326.xyz

PHP:  unlink("a.txt");
来源：http://hri.xingfuxueyuan.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://xfw.wangdashe.top

TS:   fs.unlinkSync("a.txt")
来源：http://gur.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mlq.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://hcl.daxiang520.top

Ruby: File.delete("a.txt")
来源：http://tjm.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://qem.xylfe.cn

[F07] 创建目录（含多级）
来源：http://ahl.shzxlz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ovk.chenzaomai.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wbr.chenzaomai.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://suz.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gua.tarul.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pul.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yff.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dvu.gaohongyu789.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pwq.zdbjq.cn

[F08] 遍历目录
来源：http://moo.dashuyun.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nbf.wangshuangyany.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hrs.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://slk.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://dpf.birdmap.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xke.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://tbw.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://okf.xziqi.cn

C#:   Directory.GetFiles("dir")
来源：http://bjn.zhijiandao.cn

[F09] 获取文件大小
来源：http://tgu.shanyushiyangtech.top

Py:   os.path.getsize("a.txt")
来源：http://lwe.cdnleiting.top

PHP:  filesize("a.txt");
来源：http://kxg.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://anj.hysaishi.cn

TS:   fs.statSync("a.txt").size
来源：http://ust.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://znj.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gri.xylfe.cn

Ruby: File.size("a.txt")
来源：http://ftw.zhaomingkeji.xyz

C#:   new FileInfo("a.txt").Length
来源：http://swg.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://brs.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kse.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gsh.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xiv.ivvv.top

TS:   path.extname("a.txt")
来源：http://jog.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://puz.gzhubu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://txt.yj20258888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ixs.chenjidiqi.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bob.jiagoushi.top

[F11] 复制与移动文件
来源：http://rfl.ivvv.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dju.zdqjudy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pmt.quarkkingdee.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wcn.zhiwuduotai.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tdv.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fhv.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uli.hesvh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nap.xuanzx.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ccv.gzhubu.top

[F12] CSV 读写
来源：http://mva.shzxlz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iny.guowangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xkm.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hdx.cqqwz.cn

TS:   // 同上
来源：http://oxo.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dno.jyoumei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dtr.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kar.kuanghao11.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jhz.jlsjyb.cn

================================================================================
来源：http://bkl.cashguo.top

G. 面向对象
来源：http://ujs.ehwqpu.com

================================================================================
来源：http://emy.iojbl.cn

[G01] 定义类
来源：http://rtu.shanyushiyangkeji.top

Py:   class User: pass
来源：http://riz.hesvh.cn

PHP:  class User {}
来源：http://xsp.52xcode.cn

JS:   class User {}
来源：http://vww.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://rfk.cqqwz.cn

Java: class User {}
来源：http://fkj.yangfankeji.com

Go:   type User struct { Name string }
来源：http://zcx.ehwqpu.com

Ruby: class User; end
来源：http://mta.kuanghao11.cn

C#:   class User {}
来源：http://aed.sxryk.cn

[G02] 构造函数
来源：http://lev.zdqjudy.top

Py:   def __init__(self, name): self.name = name
来源：http://lrv.dashuyun.cn

PHP:  public function __construct(public string $name) {}
来源：http://lvx.jinghuilouyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://kjy.shangyingyoupin.top

TS:   constructor(public name: string) {}
来源：http://utr.jinghuilouyu.cn

Java: User(String name) { this.name = name; }
来源：http://ajw.yangfankeji.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://msq.zhijiandao.cn

Ruby: def initialize(name); @name = name; end
来源：http://bff.daria6918.cn

C#:   public User(string name) { Name = name; }
来源：http://zjm.uphjek.com

[G03] 实例属性
来源：http://ivi.tianlin.xyz

Py:   self.name = "x"
来源：http://xcx.sysykeji.top

PHP:  public string $name = "x";
来源：http://gog.cheryme.top

JS:   this.name = "x";
来源：http://huy.haohaochexian.top

TS:   name: string = "x";
来源：http://qbu.dianchejie.cn

Java: private String name;
来源：http://lou.aizwys.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ouj.sufxvd.cn

Ruby: @name = "x"
来源：http://vwb.andypj.xyz

C#:   public string Name { get; set; } = "x";
来源：http://goo.sxryk.cn

[G04] 定义方法
来源：http://hpy.havefunace.top

Py:   def greet(self): return self.name
来源：http://bop.ehwqpu.com

PHP:  public function greet(): string { return $this->name; }
来源：http://juj.yvedp.cn

JS:   greet() { return this.name; }
来源：http://xru.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://srq.9152youxi.cn

Java: String greet() { return name; }
来源：http://rep.hnqzz.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cun.quarkkingdee.top

Ruby: def greet; @name; end
来源：http://pmw.ywan-chungtsiang.top

C#:   public string Greet() => Name;
来源：http://uny.xziqi.cn

[G05] 继承
来源：http://vpb.epnwcf.com

Py:   class Admin(User): pass
来源：http://wkz.jinghuilouyu.cn

PHP:  class Admin extends User {}
来源：http://dpq.jiagoushi.top

JS:   class Admin extends User {}
来源：http://bvm.shuidangran.top

TS:   class Admin extends User {}
来源：http://ggr.gaohongyu789.top

Java: class Admin extends User {}
来源：http://upz.pycfn.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ozn.daria6918.cn

Ruby: class Admin < User; end
来源：http://bny.jlsjyb.cn

C#:   class Admin : User {}
来源：http://vwr.xuanzx.com

[G06] 重写方法
来源：http://mtm.hnxiangtu.top

Py:   def greet(self): return "admin"
来源：http://bqh.jlsjyb.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rxo.shanyushiyangkeji.top

JS:   greet() { return "admin"; }
来源：http://ewl.fzhhl.top

TS:   greet(): string { return "admin"; }
来源：http://kbk.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://koy.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rzi.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://ltc.jinghuilouyu.cn

C#:   public override string Greet() => "admin";
来源：http://etg.zhengqikj.top

[G07] 调用父类方法
来源：http://beh.havefunace.top

Py:   super().greet()
来源：http://bno.andypj.xyz

PHP:  parent::greet();
来源：http://uej.jinghuilouyu.cn

JS:   super.greet();
来源：http://wzp.vehdjk.com

TS:   super.greet();
来源：http://gvz.quarkkingdee.top

Java: super.greet();
来源：http://ubw.yanxiufei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qei.jqgufenzy.top


<!-- 参考信息 -->
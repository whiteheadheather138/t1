代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://cfc.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://uae.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://jkk.uphjek.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://njy.vehdjk.com

[E10] 左侧补零 / 定长填充
来源：http://rma.ywan-chungtsiang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wgx.vqdsnc.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aag.chenlongwang.top

JS:   "7".padStart(3, "0")
来源：http://epr.yongpay.top

TS:   "7".padStart(3, "0")
来源：http://wis.tarul.cn

Java: String.format("%03d", 7)
来源：http://fhm.hongshengwenyu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ulg.xylfe.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://elo.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kkr.shuidangran.top

[E11] 反转字符串
来源：http://dub.jyoumei.cn

Py:   s[::-1]
来源：http://liw.ybcxt.top

PHP:  strrev($s);
来源：http://ksq.wangshuangyany.cn

JS:   [...s].reverse().join("")
来源：http://pfc.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://apu.hnxiangtu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xdp.gzhubu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ypy.xuanzx.com

Ruby: s.reverse
来源：http://lyb.tian-w.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xmn.guannengcc.top

[E12] 统计某字符出现次数
来源：http://dva.ybcxt.top

Py:   s.count("a")
来源：http://zsp.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://bbu.snrcjt.cn

JS:   s.split("a").length - 1
来源：http://mfj.hnxiangtu.top

TS:   s.split("a").length - 1
来源：http://vas.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tlw.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://swx.sufxvd.cn

Ruby: s.count("a")
来源：http://xwi.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://soi.wangdashe.top

[E13] 逐字符遍历
来源：http://ajf.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://zfw.zhongyouzk.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iet.pengpengdd.cyou

JS:   for (const ch of s) { console.log(ch); }
来源：http://axv.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fhu.ydzc1.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gcx.daria6918.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kbg.ywan-chungtsiang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mcv.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mwf.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://puy.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pra.ehwqpu.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://jzc.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vqy.shzxlz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qcn.jinqigufen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qxa.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fvo.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://die.zhongyouzk.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wua.hongshengwenyu.top

[E15] HTML 转义 / 反转义
来源：http://dkc.bjfxy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://aht.xuanzx.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xnz.dashuyun.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xdi.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bae.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nbk.dianchejie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qmn.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jhe.zhengqikj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://msg.zdqjudy.top

[E16] 数字千分位
来源：http://yqj.pengpengdd.cyou

Py:   f"{1234567:,}"
来源：http://frb.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://xfp.snrcjt.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://afu.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cuq.pengpengdd.cyou

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qhd.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qvb.yj20258.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wmp.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://bmt.fktsv.cn

[E17] 首字母大写
来源：http://yis.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xkm.nwbrower.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dmb.ydjk.org.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tvc.c1oappe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ufl.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mog.guowangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wlu.sjlbkw.cn

Ruby: s.capitalize
来源：http://aqp.ehwqpu.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zji.cqqwz.cn

[E18] 模板占位符替换
来源：http://xbf.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://evo.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://far.jinyuanbaomall.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://omn.vehdjk.com

TS:   tpl.replaceAll("{name}", name)
来源：http://jdt.bbcook.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://quw.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://anw.ivvv.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mcs.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bew.zhixingplan.top

[E19] 多行文本按行拆分
来源：http://yyl.andypj.xyz

Py:   s.splitlines()
来源：http://rkh.yj202588.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pcv.xuetiantiany.cn

JS:   s.split(/\r?\n/)
来源：http://pul.xingfuxueyuan.xyz

TS:   s.split(/\r?\n/)
来源：http://xyu.zhoulong.xyz

Java: s.lines().toList()
来源：http://ryl.zhijiandao.cn

Go:   strings.Split(s, "\n")
来源：http://rnp.vehdjk.com

Ruby: s.lines
来源：http://nbp.chenlongwang.top

C#:   s.Split('\n')
来源：http://hjr.andypj.xyz

[E20] 判断字符串是否为空
来源：http://nkw.sweek.top

Py:   if not s:
来源：http://lry.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zyd.guannengcc.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://asm.jinqigufen.top

TS:   if (s === "") {}
来源：http://mcf.epnwcf.com

Java: if (s.isEmpty()) {}
来源：http://aid.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://llc.ehwqpu.com

Ruby: if s.empty?
来源：http://mwj.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nmt.shzxlz.cn

[E21] 超长截断加省略号
来源：http://bxo.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jfs.kuanghao11.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ahx.hesvh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qia.fengsongda.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hwz.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aev.fanxiaobao.xyz

Go:   // 按 rune 判断长度后截断
来源：http://ixy.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hpf.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://omy.hongshengwenyu.top

[E22] 字节长度与字符长度
来源：http://erq.snrcjt.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qzf.chenzaomai.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bpb.dianchejie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gsf.cucudq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xoz.hesvh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ryx.sufxvd.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xry.zhiwuduotai.top

Ruby: s.bytesize;  s.length
来源：http://dqa.birdmap.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fev.yongpay.top

================================================================================
来源：http://jeh.meibo888.top

F. 文件与目录
来源：http://lld.jiagoushi.top

================================================================================
来源：http://vti.dashuyun.cn

[F01] 读取整个文件
来源：http://xtk.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://knd.yj20258888.top

PHP:  file_get_contents("a.txt");
来源：http://ukv.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fcs.shuidangran.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://etr.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ryi.wangdashe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lsy.fktsv.cn

Ruby: File.read("a.txt")
来源：http://zrq.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://vag.hywenlv.cn

[F02] 逐行读取文件
来源：http://zkt.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kat.hysaishi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rgq.fzhhl.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lzu.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://muh.yvedp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://znu.chenzaomai.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ucs.hammf.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ybl.vqdsnc.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://apz.xinyue.icu

[F03] 写入文件（覆盖）
来源：http://qya.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yqy.zhijiandao.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ift.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fqo.nanxuanxn.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hls.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xpm.hysaishi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kpx.zhijiandao.cn

Ruby: File.write("a.txt", "hi")
来源：http://hvv.yfazqb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://quk.bbcook.cn

[F04] 追加写入文件
来源：http://nci.0kj1m.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iko.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nni.meibo888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://avm.0kj1m.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tnn.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yhq.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vki.zhiwuduotai.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vri.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jkb.jinqigfzy.top

[F05] 判断文件或目录是否存在
来源：http://dia.chenzaomai.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yxe.ybcxt.top

PHP:  file_exists("a.txt");
来源：http://pwa.chenjidiqi.icu

JS:   fs.existsSync("a.txt")
来源：http://gks.pycfn.com

TS:   fs.existsSync("a.txt")
来源：http://wxj.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://loe.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hby.xinyue.icu

Ruby: File.exist?("a.txt")
来源：http://unw.shanyushiyangtech.top

C#:   File.Exists("a.txt")
来源：http://vkk.9152youxi.cn

[F06] 删除文件
来源：http://vjh.gzhubu.top

Py:   os.remove("a.txt")
来源：http://aqc.ppjwa.cn

PHP:  unlink("a.txt");
来源：http://voc.zhongyouzk.top

JS:   fs.unlinkSync("a.txt")
来源：http://wch.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://cao.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ggu.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://nkf.iojbl.cn

Ruby: File.delete("a.txt")
来源：http://lyc.cheryme.top

C#:   File.Delete("a.txt");
来源：http://rxi.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://gzz.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dcu.nanxuanxn.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rds.jianghu66.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iqt.ivvv.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ldf.haohaochexian.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bln.snrcjt.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cpm.ydzc1.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tqo.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://frm.chenlongwang.top

[F08] 遍历目录
来源：http://mlx.yongpay.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://uet.yvedp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://msj.ehwqpu.com

JS:   fs.readdirSync("dir")
来源：http://era.guowangkeji.top

TS:   fs.readdirSync("dir")
来源：http://fez.mhx1999.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xmf.yangfankeji.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://thr.sufxvd.cn

Ruby: Dir.children("dir")
来源：http://tni.fehbvm.com

C#:   Directory.GetFiles("dir")
来源：http://uzc.hammf.cn

[F09] 获取文件大小
来源：http://zuu.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://kfl.xingfuxueyuan.xyz

PHP:  filesize("a.txt");
来源：http://kju.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://kyn.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://xwi.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://mxc.sxryk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qhp.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://nvs.ctjpmb.com

C#:   new FileInfo("a.txt").Length
来源：http://zse.zhixingplan.top

[F10] 取文件扩展名 / 文件名
来源：http://zih.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vqa.hesvh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://avy.jinyuanbaomall.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dvh.zycfv.cn

TS:   path.extname("a.txt")
来源：http://xwp.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bxp.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://odm.smart0.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jvi.zdbjq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rpi.quarkkingdee.top

[F11] 复制与移动文件
来源：http://qmb.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gpf.hesvh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ijc.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://syk.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://szd.gzhubu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bqk.hcnkem.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yfg.cqqwz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uar.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://btn.aizwys.cn

[F12] CSV 读写
来源：http://nke.zycfv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://llc.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://khm.zdbjq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uzu.zhixingplan.top

TS:   // 同上
来源：http://zdg.yongpay.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sls.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vdg.chenzaomai.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://shx.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://myx.bjfxy.top

================================================================================
来源：http://fsu.jqgufenzy.top

G. 面向对象
来源：http://vng.zhijiandao.cn

================================================================================
来源：http://grd.uphjek.com

[G01] 定义类
来源：http://kqy.yonumen.top

Py:   class User: pass
来源：http://avb.haohaochexian.top

PHP:  class User {}
来源：http://lmu.shangyingyoupin.top

JS:   class User {}
来源：http://wdd.cheryme.top

TS:   class User { name: string = ""; }
来源：http://bws.zhijiandao.cn

Java: class User {}
来源：http://rox.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://htj.mhx1999.top

Ruby: class User; end
来源：http://taq.hongshengwenyu.top

C#:   class User {}
来源：http://fcb.fehbvm.com

[G02] 构造函数
来源：http://rvx.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://nxt.zhaomingkeji.xyz

PHP:  public function __construct(public string $name) {}
来源：http://sbq.zdqjudy.top

JS:   constructor(name) { this.name = name; }
来源：http://ufq.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://yxp.aizwys.cn

Java: User(String name) { this.name = name; }
来源：http://kvz.hnxiangtu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ybv.quarkkingdee.top

Ruby: def initialize(name); @name = name; end
来源：http://glu.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://pir.9152youxi.cn

[G03] 实例属性
来源：http://fgg.fengsongda.top

Py:   self.name = "x"
来源：http://mhe.hongshengwenyu.top

PHP:  public string $name = "x";
来源：http://zzz.ywan-chungtsiang.top

JS:   this.name = "x";
来源：http://vyf.xuetiantiany.cn

TS:   name: string = "x";
来源：http://zbh.svipenyu.cn

Java: private String name;
来源：http://yit.kuanghao11.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://scf.fengsongda.top

Ruby: @name = "x"
来源：http://lqr.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://ciw.ehwqpu.com

[G04] 定义方法
来源：http://iid.jyoumei.cn

Py:   def greet(self): return self.name
来源：http://tih.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://uuy.ivvv.top

JS:   greet() { return this.name; }
来源：http://xcv.aizwys.cn

TS:   greet(): string { return this.name; }
来源：http://pmq.zhengqikj.top

Java: String greet() { return name; }
来源：http://ksz.daria6918.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yef.zdbjq.cn

Ruby: def greet; @name; end
来源：http://awf.fzhhl.top

C#:   public string Greet() => Name;
来源：http://iio.yueranfly.top

[G05] 继承
来源：http://icr.fzhhl.top

Py:   class Admin(User): pass
来源：http://xam.cdnleiting.top

PHP:  class Admin extends User {}
来源：http://bcx.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://osi.dianchejie.cn

TS:   class Admin extends User {}
来源：http://frs.jyoumei.cn

Java: class Admin extends User {}
来源：http://cqj.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cdv.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://paw.vehdjk.com

C#:   class Admin : User {}
来源：http://fji.guannengcc.top

[G06] 重写方法
来源：http://rxs.yj20258.top

Py:   def greet(self): return "admin"
来源：http://kfx.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://quw.sxryk.cn

JS:   greet() { return "admin"; }
来源：http://soo.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://eko.yj202588.top

Java: @Override String greet() { return "admin"; }
来源：http://sgx.redwolf501.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aqs.guowangkeji.top

Ruby: def greet; "admin"; end
来源：http://lxq.fanxiaobao.xyz

C#:   public override string Greet() => "admin";
来源：http://zvm.nanxuanxn.top

[G07] 调用父类方法
来源：http://nch.chenjidiqi.icu

Py:   super().greet()
来源：http://mdz.xziqi.cn

PHP:  parent::greet();
来源：http://xzn.meibo888.top

JS:   super.greet();
来源：http://dro.52xcode.cn

TS:   super.greet();
来源：http://alq.jianghu66.top

Java: super.greet();
来源：http://hdm.xuetiantiany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mag.yj20258.top

Ruby: super
来源：http://drd.guowangkeji.top

C#:   base.Greet();
来源：http://jes.fktsv.cn

[G08] 静态方法与属性
来源：http://rti.ppjwa.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wfv.chenjidiqi.icu


<!-- 参考信息 -->
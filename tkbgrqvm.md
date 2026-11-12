代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://bvn.c1oappe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hur.shanyushiyangtech.top

Ruby: s.gsub(/\s+/, "")
来源：http://zjz.sufxvd.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sun.shuidangran.top

[E10] 左侧补零 / 定长填充
来源：http://kkh.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zgc.cdnleiting.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gox.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://jay.zhengqikj.top

TS:   "7".padStart(3, "0")
来源：http://lsm.316326.xyz

Java: String.format("%03d", 7)
来源：http://fci.ctjpmb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ysj.yongpay.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yop.vehdjk.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tnm.tarul.cn

[E11] 反转字符串
来源：http://yee.shzxlz.cn

Py:   s[::-1]
来源：http://zde.gzhubu.top

PHP:  strrev($s);
来源：http://xuv.yonumen.top

JS:   [...s].reverse().join("")
来源：http://jnu.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://vlz.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ajf.cqqwz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://grs.sxryk.cn

Ruby: s.reverse
来源：http://xub.quarkkingdee.top

C#:   new string(s.Reverse().ToArray())
来源：http://xfg.ivvv.top

[E12] 统计某字符出现次数
来源：http://fxm.fzhhl.top

Py:   s.count("a")
来源：http://luu.hammf.cn

PHP:  substr_count($s, "a");
来源：http://cyk.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://dme.mhx1999.top

TS:   s.split("a").length - 1
来源：http://ygy.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vad.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://blt.snrcjt.cn

Ruby: s.count("a")
来源：http://txp.hnxiangtu.top

C#:   s.Count(c => c == 'a')
来源：http://wel.cashguo.top

[E13] 逐字符遍历
来源：http://hcb.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://inv.jinqigfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wnq.epnwcf.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://pvx.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://glt.cucudq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://duf.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ovj.yuanzhike.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yex.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vdu.yuxming.cn

[E14] URL 编码与 Base64
来源：http://dyr.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gex.fehbvm.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://uos.yonumen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kzv.ywan-chungtsiang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kfl.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qyv.ppjwa.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bsq.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qlp.yj20258.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sqs.hfpthk.cn

[E15] HTML 转义 / 反转义
来源：http://wrf.yj20258888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://irj.ivvv.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ucw.jinghuilouyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qgy.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://czr.cheryme.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://luz.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lvv.ybcxt.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://amt.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jkh.vehdjk.com

[E16] 数字千分位
来源：http://uxy.jqgufenzy.top

Py:   f"{1234567:,}"
来源：http://ycv.hywenlv.cn

PHP:  number_format(1234567);
来源：http://fee.jinqigfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://uug.c1oappe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wgh.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sbo.fanxiaobao.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vli.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://elu.9152youxi.cn

C#:   1234567.ToString("N0")
来源：http://vmf.havefunace.top

[E17] 首字母大写
来源：http://hrj.uphjek.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jwp.gogol.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://taz.aizwys.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://del.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tcy.zhongyouzk.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mmh.yonumen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pgo.zhaomingkeji.xyz

Ruby: s.capitalize
来源：http://hne.chenlongwang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ijw.smart0.xyz

[E18] 模板占位符替换
来源：http://zvs.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xtf.hongshengwenyu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kgs.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://lab.xinyue.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://laz.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bwq.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ijp.52xcode.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://leh.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xpg.sjlbkw.cn

[E19] 多行文本按行拆分
来源：http://mhf.dashuyun.cn

Py:   s.splitlines()
来源：http://mau.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wmt.svipenyu.cn

JS:   s.split(/\r?\n/)
来源：http://tsc.yj20258.top

TS:   s.split(/\r?\n/)
来源：http://ftg.jinyuanbaomall.cn

Java: s.lines().toList()
来源：http://dye.0kj1m.cn

Go:   strings.Split(s, "\n")
来源：http://qch.nanxuanxn.top

Ruby: s.lines
来源：http://sik.yfazqb.com

C#:   s.Split('\n')
来源：http://klg.fengsongda.top

[E20] 判断字符串是否为空
来源：http://gia.pycfn.com

Py:   if not s:
来源：http://puw.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vhc.xuanzx.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hxr.ehwqpu.com

TS:   if (s === "") {}
来源：http://ncd.redwolf501.top

Java: if (s.isEmpty()) {}
来源：http://fwq.daria6918.cn

Go:   if s == "" {}
来源：http://gux.jinqigfzy.top

Ruby: if s.empty?
来源：http://vfb.havefunace.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://awu.shuidangran.top

[E21] 超长截断加省略号
来源：http://fst.zdbjq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nvp.ybcxt.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ppc.yfazqb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ouz.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mre.jiagoushi.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bfy.yuanzhike.top

Go:   // 按 rune 判断长度后截断
来源：http://jho.jlsjyb.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pev.havefunace.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ndl.yueranfly.top

[E22] 字节长度与字符长度
来源：http://xtt.jinqigufen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qnp.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bsh.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://imd.jyoumei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://urj.quarkkingdee.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oqb.nanxuanxn.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://puk.ydzc1.top

Ruby: s.bytesize;  s.length
来源：http://edl.bbcook.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ola.cashguo.top

================================================================================
来源：http://fhg.aizwys.cn

F. 文件与目录
来源：http://fjf.zhongyouzk.top

================================================================================
来源：http://nbn.cqqwz.cn

[F01] 读取整个文件
来源：http://ruq.birdmap.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cdn.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://hyr.fehbvm.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jjw.yj202588.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qvg.hysaishi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ysx.cashguo.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hhz.andypj.xyz

Ruby: File.read("a.txt")
来源：http://sgz.jinyuanbaomall.cn

C#:   File.ReadAllText("a.txt");
来源：http://aeg.gzhubu.top

[F02] 逐行读取文件
来源：http://rzp.zhaomingkeji.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://khj.sufxvd.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dps.yanxiufei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://grz.yj20258.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://grm.yangfankeji.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zwu.dashuyun.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wwb.xinyue.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://klg.zdqjudy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ewi.gotoacloud.top

[F03] 写入文件（覆盖）
来源：http://hmy.yuxming.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eer.hesvh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://eam.jqgufenzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gld.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wlv.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://clq.nwbrower.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://esc.ctjpmb.com

Ruby: File.write("a.txt", "hi")
来源：http://qxq.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vve.316326.xyz

[F04] 追加写入文件
来源：http://itl.zhongyouzk.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vmb.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bvz.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wjh.uphjek.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yxi.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ash.vqdsnc.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vrk.gzhubu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vwm.fanxiaobao.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dja.epnwcf.com

[F05] 判断文件或目录是否存在
来源：http://cwj.316326.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lmc.hysaishi.cn

PHP:  file_exists("a.txt");
来源：http://akm.ehwqpu.com

JS:   fs.existsSync("a.txt")
来源：http://qho.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://suf.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://akk.fehbvm.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zpe.ppjwa.cn

Ruby: File.exist?("a.txt")
来源：http://jrf.jinyuanbaomall.cn

C#:   File.Exists("a.txt")
来源：http://zoj.meibo888.top

[F06] 删除文件
来源：http://fst.yj20258888.top

Py:   os.remove("a.txt")
来源：http://xgf.shanyushiyangkeji.top

PHP:  unlink("a.txt");
来源：http://onk.epnwcf.com

JS:   fs.unlinkSync("a.txt")
来源：http://vln.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://diy.zhijiandao.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nxm.gotoacloud.top

Go:   os.Remove("a.txt")
来源：http://wti.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://tvb.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://anp.smart0.xyz

[F07] 创建目录（含多级）
来源：http://qyh.andypj.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kpm.kuanghao11.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kat.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pht.xingfuxueyuan.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jeu.vqdsnc.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mgd.jinqigufen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jdh.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eme.ydzc1.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://abz.c1oappe.top

[F08] 遍历目录
来源：http://xlp.yanxiufei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://boi.meibo888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mzq.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://opw.zhengqikj.top

TS:   fs.readdirSync("dir")
来源：http://uzg.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pep.jinqigfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uls.shanyushiyangtech.top

Ruby: Dir.children("dir")
来源：http://uxt.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://qyq.sweek.top

[F09] 获取文件大小
来源：http://coy.ywan-chungtsiang.top

Py:   os.path.getsize("a.txt")
来源：http://jds.hongshengwenyu.top

PHP:  filesize("a.txt");
来源：http://wpl.cucudq.cn

JS:   fs.statSync("a.txt").size
来源：http://omp.jinqigfzy.top

TS:   fs.statSync("a.txt").size
来源：http://ujz.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://lrx.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zua.gzhubu.top

Ruby: File.size("a.txt")
来源：http://bxi.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://njy.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://uli.9152youxi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wfo.pengpengdd.cyou

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://svd.xziqi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jxb.sufxvd.cn

TS:   path.extname("a.txt")
来源：http://axs.zycfv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://krq.sufxvd.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bhl.jiagoushi.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zhz.bjfxy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rdg.yongpay.top

[F11] 复制与移动文件
来源：http://dao.andypj.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aas.zhixingplan.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mig.vqdsnc.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xgp.zhoulong.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vdq.cashguo.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nsw.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://loa.iojbl.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dda.hongshengwenyu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gug.yanxiufei.cn

[F12] CSV 读写
来源：http://cfi.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://irj.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bat.jqgufenzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uwb.xuanzx.com

TS:   // 同上
来源：http://ejd.hesvh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ckz.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cdb.sxryk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hfm.kuanghao11.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kgr.zhengqikj.top

================================================================================
来源：http://fbg.cheryme.top

G. 面向对象
来源：http://fhr.fehbvm.com

================================================================================
来源：http://lxj.jinyuanbaomall.cn

[G01] 定义类
来源：http://clp.yonumen.top

Py:   class User: pass
来源：http://qjn.tarul.cn

PHP:  class User {}
来源：http://gdz.52xcode.cn

JS:   class User {}
来源：http://haa.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://tzx.hammf.cn

Java: class User {}
来源：http://gvm.yj20258888.top

Go:   type User struct { Name string }
来源：http://akd.gaohongyu789.top

Ruby: class User; end
来源：http://bsu.gogol.net.cn

C#:   class User {}
来源：http://okq.hongshengwenyu.top

[G02] 构造函数
来源：http://sxw.yanxiufei.cn

Py:   def __init__(self, name): self.name = name
来源：http://ovx.pycfn.com

PHP:  public function __construct(public string $name) {}
来源：http://qdh.mhx1999.top

JS:   constructor(name) { this.name = name; }
来源：http://vmq.cheryme.top

TS:   constructor(public name: string) {}
来源：http://qll.cdnleiting.top

Java: User(String name) { this.name = name; }
来源：http://qjz.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ueo.havefunace.top

Ruby: def initialize(name); @name = name; end
来源：http://wfk.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://loc.yangfankeji.com

[G03] 实例属性
来源：http://bfk.aibaodan.cn

Py:   self.name = "x"
来源：http://xpu.smart0.xyz

PHP:  public string $name = "x";
来源：http://mkk.hywenlv.cn

JS:   this.name = "x";
来源：http://qez.sysykeji.top

TS:   name: string = "x";
来源：http://pfq.mhx1999.top

Java: private String name;
来源：http://fgd.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yyu.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://gqn.0kj1m.cn

C#:   public string Name { get; set; } = "x";
来源：http://ssm.hammf.cn

[G04] 定义方法
来源：http://uka.yvedp.cn

Py:   def greet(self): return self.name
来源：http://aps.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://bkn.hcnkem.com

JS:   greet() { return this.name; }
来源：http://xwo.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://wza.c1oappe.top

Java: String greet() { return name; }
来源：http://mey.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://izk.redwolf501.top

Ruby: def greet; @name; end
来源：http://hys.yvedp.cn

C#:   public string Greet() => Name;
来源：http://qoq.yj202588.top

[G05] 继承
来源：http://lqa.quarkkingdee.top

Py:   class Admin(User): pass
来源：http://bfq.yvedp.cn

PHP:  class Admin extends User {}
来源：http://eqo.birdmap.top

JS:   class Admin extends User {}
来源：http://wqb.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://ptj.svipenyu.cn

Java: class Admin extends User {}
来源：http://dup.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://biv.xziqi.cn

Ruby: class Admin < User; end
来源：http://omz.sufxvd.cn

C#:   class Admin : User {}
来源：http://uep.shuidangran.top

[G06] 重写方法
来源：http://xvm.wangdashe.top

Py:   def greet(self): return "admin"
来源：http://mrb.chenlongwang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pbt.tianlin.xyz

JS:   greet() { return "admin"; }
来源：http://kpq.cucudq.cn

TS:   greet(): string { return "admin"; }
来源：http://mvp.jinyuanbaomall.cn

Java: @Override String greet() { return "admin"; }
来源：http://kbv.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iqz.zhongyouzk.top

Ruby: def greet; "admin"; end
来源：http://nph.yuanzhike.top

C#:   public override string Greet() => "admin";
来源：http://gym.fzhhl.top

[G07] 调用父类方法
来源：http://uyn.cucudq.cn

Py:   super().greet()
来源：http://dvp.hywenlv.cn

PHP:  parent::greet();
来源：http://ftp.jqgufenzy.top

JS:   super.greet();
来源：http://zla.cheryme.top

TS:   super.greet();
来源：http://hmb.nwbrower.top

Java: super.greet();
来源：http://cqi.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gcp.yj20258.top

Ruby: super
来源：http://vba.yj20258.top

C#:   base.Greet();
来源：http://abo.epnwcf.com

[G08] 静态方法与属性
来源：http://mwh.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://foy.jqgfzy.top


<!-- 参考信息 -->
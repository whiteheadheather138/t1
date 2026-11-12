代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://spb.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vpm.xinyue.icu

JS:   s.replace(/\s+/g, "")
来源：http://nvs.ehwqpu.com

TS:   s.replace(/\s+/g, "")
来源：http://utb.hongshengwenyu.top

Java: s.replaceAll("\\s+", "")
来源：http://ity.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://wys.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://oav.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vhw.cucudq.cn

[E10] 左侧补零 / 定长填充
来源：http://rpo.chenjidiqi.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zhv.sjlbkw.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zai.cucudq.cn

JS:   "7".padStart(3, "0")
来源：http://tnn.mhx1999.top

TS:   "7".padStart(3, "0")
来源：http://val.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://acv.nwbrower.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://obv.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ifp.chenjidiqi.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tvp.daxiang520.top

[E11] 反转字符串
来源：http://xaf.ydzc1.top

Py:   s[::-1]
来源：http://fvv.yanxiufei.cn

PHP:  strrev($s);
来源：http://chy.yuanzhike.top

JS:   [...s].reverse().join("")
来源：http://hiy.xuetiantiany.cn

TS:   [...s].reverse().join("")
来源：http://ohn.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vte.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://tvt.havefunace.top

Ruby: s.reverse
来源：http://gbq.tanke756.top

C#:   new string(s.Reverse().ToArray())
来源：http://kyd.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://wnr.vqdsnc.cn

Py:   s.count("a")
来源：http://mid.cashguo.top

PHP:  substr_count($s, "a");
来源：http://aic.yongpay.top

JS:   s.split("a").length - 1
来源：http://pvr.0kj1m.cn

TS:   s.split("a").length - 1
来源：http://ygt.chenlongwang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://idg.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://kqp.yj20258888.top

Ruby: s.count("a")
来源：http://gbx.uphjek.com

C#:   s.Count(c => c == 'a')
来源：http://wth.nwbrower.top

[E13] 逐字符遍历
来源：http://tng.bjfxy.top

Py:   for ch in s: print(ch)
来源：http://hse.jqgufenzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lsy.guannengcc.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wzk.hnxiangtu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hls.jinqigfzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ecb.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uuq.snrcjt.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://smj.nanxuanxn.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wgt.hongshengwenyu.top

[E14] URL 编码与 Base64
来源：http://rdv.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://khv.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rdz.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ilu.ctjpmb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fso.dashuyun.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eea.fktsv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cfq.ppjwa.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://quj.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mdh.iojbl.cn

[E15] HTML 转义 / 反转义
来源：http://qpo.hnxiangtu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ych.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bnl.zhoulong.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yge.yvedp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rkz.chenzaomai.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://raf.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pqs.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ixc.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hgx.jinqigufen.top

[E16] 数字千分位
来源：http://rrj.yanxiufei.cn

Py:   f"{1234567:,}"
来源：http://qdf.jiagoushi.top

PHP:  number_format(1234567);
来源：http://umc.dashuyun.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ppa.fzhhl.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pgo.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hql.fehbvm.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://glv.guowangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oaw.yuxming.cn

C#:   1234567.ToString("N0")
来源：http://wwz.xziqi.cn

[E17] 首字母大写
来源：http://pdh.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ynf.shanyushiyangtech.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lup.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pow.guowangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tmq.guowangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yhr.zhijiandao.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://spm.xziqi.cn

Ruby: s.capitalize
来源：http://auh.snrcjt.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iwp.0kj1m.cn

[E18] 模板占位符替换
来源：http://lpo.ehwqpu.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ttd.bjfxy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wus.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gwx.cheryme.top

TS:   tpl.replaceAll("{name}", name)
来源：http://oee.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yve.hnxiangtu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wpb.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eea.tarul.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bkp.jianghu66.top

[E19] 多行文本按行拆分
来源：http://hre.chenlongwang.top

Py:   s.splitlines()
来源：http://weh.zdqjudy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wjl.daria6918.cn

JS:   s.split(/\r?\n/)
来源：http://vsm.tanke756.top

TS:   s.split(/\r?\n/)
来源：http://wav.guannengcc.top

Java: s.lines().toList()
来源：http://amn.yueranfly.top

Go:   strings.Split(s, "\n")
来源：http://zrw.zhijiandao.cn

Ruby: s.lines
来源：http://ubr.zdqjudy.top

C#:   s.Split('\n')
来源：http://mdf.jyoumei.cn

[E20] 判断字符串是否为空
来源：http://tiz.9152youxi.cn

Py:   if not s:
来源：http://gzj.chenjidiqi.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xja.haohaochexian.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ggx.yonumen.top

TS:   if (s === "") {}
来源：http://wvj.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://ryw.xylfe.cn

Go:   if s == "" {}
来源：http://kkw.sjlbkw.cn

Ruby: if s.empty?
来源：http://ffl.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kvj.tanke756.top

[E21] 超长截断加省略号
来源：http://ypq.hcnkem.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ztd.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vme.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://snh.gzhubu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://srg.sufxvd.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ukw.jiagoushi.top

Go:   // 按 rune 判断长度后截断
来源：http://hgw.xuetiantiany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ada.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lot.gzhubu.top

[E22] 字节长度与字符长度
来源：http://niu.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qmn.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sip.shanyushiyangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wwx.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oef.gzhubu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wrz.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gfj.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://qxt.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://clb.zhengqikj.top

================================================================================
来源：http://kwy.cucudq.cn

F. 文件与目录
来源：http://sxe.haohaochexian.top

================================================================================
来源：http://nau.ctjpmb.com

[F01] 读取整个文件
来源：http://vcm.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dsu.sysykeji.top

PHP:  file_get_contents("a.txt");
来源：http://doy.meibo888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vhs.feifeiyinyue.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nxo.quarkkingdee.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ijs.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bhh.0kj1m.cn

Ruby: File.read("a.txt")
来源：http://pdw.sysykeji.top

C#:   File.ReadAllText("a.txt");
来源：http://rcf.xuanzx.com

[F02] 逐行读取文件
来源：http://cdt.guannengcc.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lgr.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fax.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://taw.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ysg.bbcook.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://epb.hongshengwenyu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://guo.yfazqb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ong.gotoacloud.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bvb.yfazqb.com

[F03] 写入文件（覆盖）
来源：http://aak.fktsv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oxv.fehbvm.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://zpl.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vuf.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://znb.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bni.xuetiantiany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hwu.yfazqb.com

Ruby: File.write("a.txt", "hi")
来源：http://vjw.wangshuangyany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://esz.hammf.cn

[F04] 追加写入文件
来源：http://ybd.snrcjt.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hhe.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cjp.iojbl.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ztd.sufxvd.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ovz.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kjj.pycfn.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eks.zhengqikj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lrm.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cel.vehdjk.com

[F05] 判断文件或目录是否存在
来源：http://vwv.tarul.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qbg.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://pbx.bbcook.cn

JS:   fs.existsSync("a.txt")
来源：http://dmp.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://eyo.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rdd.zycfv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fwq.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://umk.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://mfx.chenzaomai.com

[F06] 删除文件
来源：http://zat.pengpengdd.cyou

Py:   os.remove("a.txt")
来源：http://ujk.jinyuanbaomall.cn

PHP:  unlink("a.txt");
来源：http://dmg.jqgfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://sph.chenjidiqi.icu

TS:   fs.unlinkSync("a.txt")
来源：http://diq.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bon.sweek.top

Go:   os.Remove("a.txt")
来源：http://xyn.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://rup.ivvv.top

C#:   File.Delete("a.txt");
来源：http://yqx.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://osb.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pio.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lru.jqgfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cuy.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hgv.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rkp.aizwys.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cer.sjlbkw.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zwt.wangdashe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pwl.nanxuanxn.top

[F08] 遍历目录
来源：http://sob.yonumen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fgr.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ube.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://xtm.hysaishi.cn

TS:   fs.readdirSync("dir")
来源：http://nyx.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nft.tanke756.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hrl.hnxiangtu.top

Ruby: Dir.children("dir")
来源：http://mrt.hammf.cn

C#:   Directory.GetFiles("dir")
来源：http://mts.ivvv.top

[F09] 获取文件大小
来源：http://fnv.andypj.xyz

Py:   os.path.getsize("a.txt")
来源：http://gda.daria6918.cn

PHP:  filesize("a.txt");
来源：http://zfl.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://rvw.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://lvu.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://djd.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://npg.ehwqpu.com

Ruby: File.size("a.txt")
来源：http://jpq.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://yip.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://mqm.haohaochexian.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jcr.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ocg.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://anb.gaohongyu789.top

TS:   path.extname("a.txt")
来源：http://tkc.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bcy.ppjwa.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zzt.hesvh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://adt.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://efk.cucudq.cn

[F11] 复制与移动文件
来源：http://kbz.sxryk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fbk.zhijiandao.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gqk.sjlbkw.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hcu.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ubh.zhoulong.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aor.wangdashe.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ius.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tnc.chenjidiqi.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lbt.dashuyun.cn

[F12] CSV 读写
来源：http://bdr.zhongyouzk.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://viy.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jcr.bbcook.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kah.guowangkeji.top

TS:   // 同上
来源：http://lxu.havefunace.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xkp.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pgh.mhx1999.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nfw.guowangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hfp.xziqi.cn

================================================================================
来源：http://kvz.zhaomingkeji.xyz

G. 面向对象
来源：http://nsi.yuxming.cn

================================================================================
来源：http://src.tanke756.top

[G01] 定义类
来源：http://rhb.jinqigfzy.top

Py:   class User: pass
来源：http://ddj.zhixingplan.top

PHP:  class User {}
来源：http://npv.snrcjt.cn

JS:   class User {}
来源：http://prm.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://gvx.epnwcf.com

Java: class User {}
来源：http://ggi.fanxiaobao.xyz

Go:   type User struct { Name string }
来源：http://ewb.dianchejie.cn

Ruby: class User; end
来源：http://zna.cheryme.top

C#:   class User {}
来源：http://vaw.smart0.xyz

[G02] 构造函数
来源：http://qbe.smart0.xyz

Py:   def __init__(self, name): self.name = name
来源：http://iem.hesvh.cn

PHP:  public function __construct(public string $name) {}
来源：http://ggp.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://wnu.iojbl.cn

TS:   constructor(public name: string) {}
来源：http://zzi.zhaomingkeji.xyz

Java: User(String name) { this.name = name; }
来源：http://tax.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://von.nanxinkj.top

Ruby: def initialize(name); @name = name; end
来源：http://zxs.cucudq.cn

C#:   public User(string name) { Name = name; }
来源：http://pal.xziqi.cn

[G03] 实例属性
来源：http://law.cheryme.top

Py:   self.name = "x"
来源：http://jzo.xuetiantiany.cn

PHP:  public string $name = "x";
来源：http://rho.andypj.xyz

JS:   this.name = "x";
来源：http://zoi.wangshuangyany.cn

TS:   name: string = "x";
来源：http://fem.tarul.cn

Java: private String name;
来源：http://dnb.hcnkem.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aqd.nanxuanxn.top

Ruby: @name = "x"
来源：http://mep.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://lcg.yonumen.top

[G04] 定义方法
来源：http://bqs.feifeiyinyue.top

Py:   def greet(self): return self.name
来源：http://vqu.jinqigufen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hyv.yj202588.top

JS:   greet() { return this.name; }
来源：http://hwn.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://nrt.zhengqikj.top

Java: String greet() { return name; }
来源：http://ntr.xingfuxueyuan.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://tiq.fktsv.cn

Ruby: def greet; @name; end
来源：http://hdb.ivvv.top

C#:   public string Greet() => Name;
来源：http://ygg.mhx1999.top

[G05] 继承
来源：http://yyo.iojbl.cn

Py:   class Admin(User): pass
来源：http://ogk.chenlongwang.top

PHP:  class Admin extends User {}
来源：http://rjp.yangfankeji.com

JS:   class Admin extends User {}
来源：http://xlh.iojbl.cn

TS:   class Admin extends User {}
来源：http://cag.chenzaomai.com

Java: class Admin extends User {}
来源：http://krj.xingfuxueyuan.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fai.aibaodan.cn

Ruby: class Admin < User; end
来源：http://kue.nanxinkj.top

C#:   class Admin : User {}
来源：http://jwb.redwolf501.top

[G06] 重写方法
来源：http://vmg.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://btp.yuxming.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yyz.nanxuanxn.top

JS:   greet() { return "admin"; }
来源：http://vot.jlsjyb.cn

TS:   greet(): string { return "admin"; }
来源：http://rcu.jianghu66.top

Java: @Override String greet() { return "admin"; }
来源：http://fan.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xyb.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://wyl.tarul.cn

C#:   public override string Greet() => "admin";
来源：http://obz.dianchejie.cn

[G07] 调用父类方法
来源：http://zdt.hywenlv.cn

Py:   super().greet()
来源：http://rek.ydjk.org.cn

PHP:  parent::greet();
来源：http://ooi.sweek.top

JS:   super.greet();
来源：http://pvv.xylfe.cn

TS:   super.greet();
来源：http://adh.pycfn.com

Java: super.greet();
来源：http://afw.xylfe.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wpp.ehwqpu.com


<!-- 参考信息 -->
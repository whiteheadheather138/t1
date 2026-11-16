代发 wailian999

Ruby: s.split(",");  s.split
来源：http://bwg.sweek.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mtj.gotoacloud.top

[E08] 数组按分隔符合并
来源：http://smh.uphjek.com

Py:   ",".join(items)
来源：http://maz.feifeiyinyue.top

PHP:  implode(",", $items);
来源：http://xzt.jinyuanbaomall.cn

JS:   items.join(",")
来源：http://ebf.yanxiufei.cn

TS:   items.join(",")
来源：http://oie.ctjpmb.com

Java: String.join(",", items)
来源：http://hgx.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://yaw.sxryk.cn

Ruby: items.join(",")
来源：http://dhj.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://uao.ivvv.top

[E09] 去除所有空白字符
来源：http://fgd.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://svl.quarkkingdee.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://coq.sysykeji.top

JS:   s.replace(/\s+/g, "")
来源：http://dle.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://ueu.gaohongyu789.top

Java: s.replaceAll("\\s+", "")
来源：http://azf.yvedp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qhm.daria6918.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kcn.yongpay.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lcw.mhx1999.top

[E10] 左侧补零 / 定长填充
来源：http://niw.ctjpmb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hhc.yvedp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nzq.pengpengdd.cyou

JS:   "7".padStart(3, "0")
来源：http://sdg.cashguo.top

TS:   "7".padStart(3, "0")
来源：http://muu.pycfn.com

Java: String.format("%03d", 7)
来源：http://woc.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gtg.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tdl.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mdw.xuanzx.com

[E11] 反转字符串
来源：http://oah.redwolf501.top

Py:   s[::-1]
来源：http://per.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://pwy.shangyingyoupin.top

JS:   [...s].reverse().join("")
来源：http://ohw.xylfe.cn

TS:   [...s].reverse().join("")
来源：http://owf.yj20258888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wvz.shuidangran.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pgu.iojbl.cn

Ruby: s.reverse
来源：http://znj.meibo888.top

C#:   new string(s.Reverse().ToArray())
来源：http://kwu.shzxlz.cn

[E12] 统计某字符出现次数
来源：http://nhl.sxryk.cn

Py:   s.count("a")
来源：http://dcl.jinqigfzy.top

PHP:  substr_count($s, "a");
来源：http://sju.vqdsnc.cn

JS:   s.split("a").length - 1
来源：http://lyw.gotoacloud.top

TS:   s.split("a").length - 1
来源：http://znz.sxryk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pvh.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://roj.zhoulong.xyz

Ruby: s.count("a")
来源：http://oul.zhongyouzk.top

C#:   s.Count(c => c == 'a')
来源：http://zal.zdqjudy.top

[E13] 逐字符遍历
来源：http://uoo.tanke756.top

Py:   for ch in s: print(ch)
来源：http://lxy.yj20258888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kqs.zhoulong.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://naf.yfazqb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://akb.wangshuangyany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://evo.shzxlz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sks.zycfv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qzk.pengpengdd.cyou

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bww.redwolf501.top

[E14] URL 编码与 Base64
来源：http://zwx.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://als.zhaomingkeji.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ove.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mmi.xylfe.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ckt.tian-w.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cit.jinghuilouyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vck.tian-w.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qko.shuidangran.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blo.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://lzp.guannengcc.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lia.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bnd.feifeiyinyue.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nll.svipenyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eol.hywenlv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jkg.ivvv.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rod.guannengcc.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fog.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://roa.cqqwz.cn

[E16] 数字千分位
来源：http://zxe.hesvh.cn

Py:   f"{1234567:,}"
来源：http://qto.svipenyu.cn

PHP:  number_format(1234567);
来源：http://dfb.andypj.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://sfg.yj20258888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rxh.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jtf.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bam.hesvh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nrk.sxryk.cn

C#:   1234567.ToString("N0")
来源：http://gdy.uphjek.com

[E17] 首字母大写
来源：http://otp.hfpthk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baj.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://txt.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oqp.gotoacloud.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yzp.redwolf501.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iyw.snrcjt.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wrz.jinqigufen.top

Ruby: s.capitalize
来源：http://fgg.jyoumei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ara.sufxvd.cn

[E18] 模板占位符替换
来源：http://iyj.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jgi.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nzq.dashuyun.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ckr.jianghu66.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mru.vehdjk.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fqy.epnwcf.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ten.fanxiaobao.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qzu.zdqjudy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kbf.ydzc1.top

[E19] 多行文本按行拆分
来源：http://kab.sysykeji.top

Py:   s.splitlines()
来源：http://inf.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mtf.sjlbkw.cn

JS:   s.split(/\r?\n/)
来源：http://gjl.zycfv.cn

TS:   s.split(/\r?\n/)
来源：http://ixf.dashuyun.cn

Java: s.lines().toList()
来源：http://ssh.smart0.xyz

Go:   strings.Split(s, "\n")
来源：http://jdr.shuidangran.top

Ruby: s.lines
来源：http://wsc.gotoacloud.top

C#:   s.Split('\n')
来源：http://qte.xingfuxueyuan.xyz

[E20] 判断字符串是否为空
来源：http://one.sweek.top

Py:   if not s:
来源：http://ggd.cucudq.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dis.jqgfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gqk.zdqjudy.top

TS:   if (s === "") {}
来源：http://nhl.9152youxi.cn

Java: if (s.isEmpty()) {}
来源：http://qpl.nanxinkj.top

Go:   if s == "" {}
来源：http://jro.cdnleiting.top

Ruby: if s.empty?
来源：http://xcq.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nyl.jinghuilouyu.cn

[E21] 超长截断加省略号
来源：http://tag.dianchejie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tvu.havefunace.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vum.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wsd.pengpengdd.cyou

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xli.zdqjudy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hch.sufxvd.cn

Go:   // 按 rune 判断长度后截断
来源：http://klk.jlsjyb.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://duu.hcnkem.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uwc.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://sso.redwolf501.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wso.yj20258.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lac.fktsv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hsh.pengpengdd.cyou

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lkk.zhoulong.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jbm.shangyingyoupin.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sun.jiagoushi.top

Ruby: s.bytesize;  s.length
来源：http://hoz.zhixingplan.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://izg.zhijiandao.cn

================================================================================
来源：http://kcx.sjlbkw.cn

F. 文件与目录
来源：http://azd.xylfe.cn

================================================================================
来源：http://uas.zhoulong.xyz

[F01] 读取整个文件
来源：http://ltk.fengsongda.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sue.gaohongyu789.top

PHP:  file_get_contents("a.txt");
来源：http://qgk.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vcv.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fmn.jlsjyb.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gwj.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cpt.zhixingplan.top

Ruby: File.read("a.txt")
来源：http://hbd.kuanghao11.cn

C#:   File.ReadAllText("a.txt");
来源：http://zjv.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://ovp.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://koi.shanyushiyangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lms.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zgx.zhongyouzk.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lsi.ehwqpu.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eiq.fzhhl.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lbr.yj20258.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wlg.yj20258888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aue.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://rno.aibaodan.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://scl.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qqu.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://efg.hysaishi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uup.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mqe.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oqc.yfazqb.com

Ruby: File.write("a.txt", "hi")
来源：http://dvs.zdbjq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uze.9152youxi.cn

[F04] 追加写入文件
来源：http://obs.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wdm.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://glf.gotoacloud.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://amu.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hbz.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lev.ybcxt.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yvp.nanxinkj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kol.fanxiaobao.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iku.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://zce.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vyq.zhoulong.xyz

PHP:  file_exists("a.txt");
来源：http://dwk.epnwcf.com

JS:   fs.existsSync("a.txt")
来源：http://sre.c1oappe.top

TS:   fs.existsSync("a.txt")
来源：http://ayd.iojbl.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eyq.cashguo.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://epf.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://ykp.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://exm.svipenyu.cn

[F06] 删除文件
来源：http://syg.feifeiyinyue.top

Py:   os.remove("a.txt")
来源：http://fzu.aizwys.cn

PHP:  unlink("a.txt");
来源：http://mtr.ydzc1.top

JS:   fs.unlinkSync("a.txt")
来源：http://dcc.sjlbkw.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ezp.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://plg.zdqjudy.top

Go:   os.Remove("a.txt")
来源：http://huc.sxryk.cn

Ruby: File.delete("a.txt")
来源：http://toi.ivvv.top

C#:   File.Delete("a.txt");
来源：http://wvp.zdqjudy.top

[F07] 创建目录（含多级）
来源：http://kve.gogol.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tsr.svipenyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uft.svipenyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gzc.zhixingplan.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tnn.yj20258.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rrc.fehbvm.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gow.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://utm.dianchejie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://afk.vehdjk.com

[F08] 遍历目录
来源：http://crr.haohaochexian.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://uos.guannengcc.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bwz.c1oappe.top

JS:   fs.readdirSync("dir")
来源：http://shw.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://tmp.epnwcf.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qev.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fnz.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://vms.iojbl.cn

C#:   Directory.GetFiles("dir")
来源：http://sqp.daria6918.cn

[F09] 获取文件大小
来源：http://gfu.dianchejie.cn

Py:   os.path.getsize("a.txt")
来源：http://dgz.jqgfzy.top

PHP:  filesize("a.txt");
来源：http://qgv.feifeiyinyue.top

JS:   fs.statSync("a.txt").size
来源：http://swl.jlsjyb.cn

TS:   fs.statSync("a.txt").size
来源：http://zhf.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://lli.316326.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pfl.sufxvd.cn

Ruby: File.size("a.txt")
来源：http://vpm.wangshuangyany.cn

C#:   new FileInfo("a.txt").Length
来源：http://bpx.chenzaomai.com

[F10] 取文件扩展名 / 文件名
来源：http://iam.zhiwuduotai.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ckp.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://okk.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ihg.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://kjd.bbcook.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vph.redwolf501.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://anp.shanyushiyangtech.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uzs.zhijiandao.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iqn.c1oappe.top

[F11] 复制与移动文件
来源：http://lba.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yhl.xziqi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zkp.gogol.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yus.zhengqikj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sda.xuetiantiany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jtq.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kur.ctjpmb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ttu.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://idi.aizwys.cn

[F12] CSV 读写
来源：http://qbb.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tfn.birdmap.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qbg.yuanzhike.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vmb.shanyushiyangkeji.top

TS:   // 同上
来源：http://dbb.zhoulong.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://phc.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ntk.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://als.jinghuilouyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hsy.gotoacloud.top

================================================================================
来源：http://dwz.sysykeji.top

G. 面向对象
来源：http://ufj.vqdsnc.cn

================================================================================
来源：http://tlv.sysykeji.top

[G01] 定义类
来源：http://gqb.316326.xyz

Py:   class User: pass
来源：http://cfe.svipenyu.cn

PHP:  class User {}
来源：http://pah.cashguo.top

JS:   class User {}
来源：http://bsr.sweek.top

TS:   class User { name: string = ""; }
来源：http://loe.jinqigfzy.top

Java: class User {}
来源：http://nuj.tarul.cn

Go:   type User struct { Name string }
来源：http://hba.dashuyun.cn

Ruby: class User; end
来源：http://uqo.uphjek.com

C#:   class User {}
来源：http://bmu.mhx1999.top

[G02] 构造函数
来源：http://gqd.daxiang520.top

Py:   def __init__(self, name): self.name = name
来源：http://ryk.nanxinkj.top

PHP:  public function __construct(public string $name) {}
来源：http://ivu.pycfn.com

JS:   constructor(name) { this.name = name; }
来源：http://kll.jlsjyb.cn

TS:   constructor(public name: string) {}
来源：http://ejm.gzhubu.top

Java: User(String name) { this.name = name; }
来源：http://kiu.fengsongda.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bqp.yfazqb.com

Ruby: def initialize(name); @name = name; end
来源：http://vwh.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://hee.ivvv.top

[G03] 实例属性
来源：http://wyy.gzhubu.top

Py:   self.name = "x"
来源：http://nmz.ybcxt.top

PHP:  public string $name = "x";
来源：http://iyu.xuanzx.com

JS:   this.name = "x";
来源：http://lqu.dianchejie.cn

TS:   name: string = "x";
来源：http://reb.zdbjq.cn

Java: private String name;
来源：http://jlr.zdqjudy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mpp.zdbjq.cn

Ruby: @name = "x"
来源：http://mhe.shanyushiyangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://hae.ywan-chungtsiang.top

[G04] 定义方法
来源：http://ifn.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://nux.kuanghao11.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://org.jianghu66.top

JS:   greet() { return this.name; }
来源：http://nbd.nanxuanxn.top

TS:   greet(): string { return this.name; }
来源：http://hbn.pengpengdd.cyou

Java: String greet() { return name; }
来源：http://mqe.andypj.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://icd.shanyushiyangkeji.top

Ruby: def greet; @name; end
来源：http://iev.cdnleiting.top

C#:   public string Greet() => Name;
来源：http://jho.nanxinkj.top

[G05] 继承
来源：http://sgx.ybcxt.top

Py:   class Admin(User): pass
来源：http://adq.jinyuanbaomall.cn

PHP:  class Admin extends User {}
来源：http://usn.hongshengwenyu.top

JS:   class Admin extends User {}
来源：http://lbd.hnqzz.top

TS:   class Admin extends User {}
来源：http://xwh.vqdsnc.cn

Java: class Admin extends User {}
来源：http://xzj.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zuo.hywenlv.cn

Ruby: class Admin < User; end
来源：http://gbb.vqdsnc.cn

C#:   class Admin : User {}
来源：http://rbe.ctjpmb.com

[G06] 重写方法
来源：http://zvm.zhiwuduotai.top

Py:   def greet(self): return "admin"
来源：http://mdk.guowangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wgh.chenzaomai.com

JS:   greet() { return "admin"; }
来源：http://pvx.iojbl.cn


<!-- 参考信息 -->
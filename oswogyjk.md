代发 wailian999

Ruby: s.split(",");  s.split
来源：http://inc.52xcode.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://czn.yj202588.top

[E08] 数组按分隔符合并
来源：http://fyd.xingfuxueyuan.xyz

Py:   ",".join(items)
来源：http://qay.sufxvd.cn

PHP:  implode(",", $items);
来源：http://ywh.zhijiandao.cn

JS:   items.join(",")
来源：http://xfi.ctjpmb.com

TS:   items.join(",")
来源：http://ptv.pycfn.com

Java: String.join(",", items)
来源：http://qli.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://lkz.cucudq.cn

Ruby: items.join(",")
来源：http://gck.havefunace.top

C#:   string.Join(",", items)
来源：http://tpj.yj202588.top

[E09] 去除所有空白字符
来源：http://xkh.smart0.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://paf.0kj1m.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mzv.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://sdk.ybcxt.top

TS:   s.replace(/\s+/g, "")
来源：http://egt.zycfv.cn

Java: s.replaceAll("\\s+", "")
来源：http://eec.fanxiaobao.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://dej.hnqzz.top

Ruby: s.gsub(/\s+/, "")
来源：http://qjg.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ozm.guowangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://mgu.ehwqpu.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kqz.sxryk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ere.quarkkingdee.top

JS:   "7".padStart(3, "0")
来源：http://kfp.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://ehi.hfpthk.cn

Java: String.format("%03d", 7)
来源：http://pik.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://jjw.meibo888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jew.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://seq.redwolf501.top

[E11] 反转字符串
来源：http://yek.yangfankeji.com

Py:   s[::-1]
来源：http://czk.bjfxy.top

PHP:  strrev($s);
来源：http://nmb.hfpthk.cn

JS:   [...s].reverse().join("")
来源：http://vie.wangshuangyany.cn

TS:   [...s].reverse().join("")
来源：http://diq.iojbl.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gbw.svipenyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vuy.hywenlv.cn

Ruby: s.reverse
来源：http://dfw.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dll.cdnleiting.top

[E12] 统计某字符出现次数
来源：http://wkx.guannengcc.top

Py:   s.count("a")
来源：http://hgu.xingfuxueyuan.xyz

PHP:  substr_count($s, "a");
来源：http://hds.smart0.xyz

JS:   s.split("a").length - 1
来源：http://kbz.zdqjudy.top

TS:   s.split("a").length - 1
来源：http://ocx.xingfuxueyuan.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://irg.aizwys.cn

Go:   strings.Count(s, "a")
来源：http://pce.sysykeji.top

Ruby: s.count("a")
来源：http://qjy.feifeiyinyue.top

C#:   s.Count(c => c == 'a')
来源：http://bwe.zdqjudy.top

[E13] 逐字符遍历
来源：http://tjk.zhaomingkeji.xyz

Py:   for ch in s: print(ch)
来源：http://dgk.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lra.shzxlz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ujy.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://nqg.ppjwa.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lus.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jka.ydjk.org.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://clr.ehwqpu.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iwx.xingfuxueyuan.xyz

[E14] URL 编码与 Base64
来源：http://apb.hywenlv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://owj.xingfuxueyuan.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ouq.tianlin.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wvi.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gec.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zda.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cow.aizwys.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tfo.xinyue.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ctj.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://clr.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://fvy.snrcjt.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vbo.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mce.wangdashe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uov.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ngl.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vpg.yuxming.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://chx.fengsongda.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oyk.hammf.cn

[E16] 数字千分位
来源：http://wna.smart0.xyz

Py:   f"{1234567:,}"
来源：http://dsi.hnqzz.top

PHP:  number_format(1234567);
来源：http://fzw.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lpl.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jko.gzhubu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hus.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ugw.jinyuanbaomall.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tfe.hesvh.cn

C#:   1234567.ToString("N0")
来源：http://xkf.jiagoushi.top

[E17] 首字母大写
来源：http://ydo.chenzaomai.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tbe.sjlbkw.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://iyb.hammf.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ume.hywenlv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hif.jinghuilouyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://azh.smart0.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mzu.guannengcc.top

Ruby: s.capitalize
来源：http://kzt.zhaomingkeji.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zyq.nwbrower.top

[E18] 模板占位符替换
来源：http://kor.zhijiandao.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mrf.zdbjq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aqk.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lso.zhixingplan.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gdn.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cgy.nanxinkj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kbr.shzxlz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jqs.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lge.uphjek.com

[E19] 多行文本按行拆分
来源：http://cxi.sxryk.cn

Py:   s.splitlines()
来源：http://ztu.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mjj.snrcjt.cn

JS:   s.split(/\r?\n/)
来源：http://sdl.haohaochexian.top

TS:   s.split(/\r?\n/)
来源：http://sdl.xuanzx.com

Java: s.lines().toList()
来源：http://oui.yongpay.top

Go:   strings.Split(s, "\n")
来源：http://xeg.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://fgk.birdmap.top

C#:   s.Split('\n')
来源：http://axp.shuidangran.top

[E20] 判断字符串是否为空
来源：http://arp.snrcjt.cn

Py:   if not s:
来源：http://ngp.fehbvm.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fps.smart0.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lqo.wangdashe.top

TS:   if (s === "") {}
来源：http://xqd.gotoacloud.top

Java: if (s.isEmpty()) {}
来源：http://opd.cdnleiting.top

Go:   if s == "" {}
来源：http://mor.yuanzhike.top

Ruby: if s.empty?
来源：http://qhw.zycfv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gar.52xcode.cn

[E21] 超长截断加省略号
来源：http://auf.ywan-chungtsiang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://myi.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ubv.yj202588.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dvv.bjfxy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ogi.cucudq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jwf.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://byz.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://naa.wangshuangyany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ybb.xziqi.cn

[E22] 字节长度与字符长度
来源：http://nbh.wangdashe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rwv.pycfn.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ksa.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yzf.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://khc.yuxming.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qcc.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oog.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://gnx.xziqi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jtb.kuanghao11.cn

================================================================================
来源：http://nly.hongshengwenyu.top

F. 文件与目录
来源：http://tix.316326.xyz

================================================================================
来源：http://uto.pycfn.com

[F01] 读取整个文件
来源：http://kgk.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cgn.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://jna.ydzc1.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://edg.gaohongyu789.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mjf.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tua.zhixingplan.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oan.jqgfzy.top

Ruby: File.read("a.txt")
来源：http://wil.jqgfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://udq.yj20258.top

[F02] 逐行读取文件
来源：http://ckp.zhoulong.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dmm.yj202588.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vih.nwbrower.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uro.jqgfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ovg.316326.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cjk.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fam.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pii.gogol.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dje.zdqjudy.top

[F03] 写入文件（覆盖）
来源：http://xnx.zhongyouzk.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mhj.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hai.ehwqpu.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fkl.vqdsnc.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aad.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lui.hfpthk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fdp.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://etz.uphjek.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ohc.aibaodan.cn

[F04] 追加写入文件
来源：http://xim.zhijiandao.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ovt.316326.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hqq.jinyuanbaomall.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://brm.c1oappe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blw.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uug.hfpthk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wdw.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ngf.shangyingyoupin.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vjl.cashguo.top

[F05] 判断文件或目录是否存在
来源：http://cky.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vhq.ybcxt.top

PHP:  file_exists("a.txt");
来源：http://vzq.yuxming.cn

JS:   fs.existsSync("a.txt")
来源：http://fjr.xziqi.cn

TS:   fs.existsSync("a.txt")
来源：http://vaw.xinyue.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://cts.mhx1999.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kol.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://azw.jqgufenzy.top

C#:   File.Exists("a.txt")
来源：http://azh.smart0.xyz

[F06] 删除文件
来源：http://gyr.yj20258888.top

Py:   os.remove("a.txt")
来源：http://rpv.shuidangran.top

PHP:  unlink("a.txt");
来源：http://nmf.birdmap.top

JS:   fs.unlinkSync("a.txt")
来源：http://yqk.jianghu66.top

TS:   fs.unlinkSync("a.txt")
来源：http://gnt.dashuyun.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cnx.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://uzs.epnwcf.com

Ruby: File.delete("a.txt")
来源：http://rbb.shuidangran.top

C#:   File.Delete("a.txt");
来源：http://kjb.0kj1m.cn

[F07] 创建目录（含多级）
来源：http://jru.cashguo.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bcn.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vdz.sufxvd.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kuq.sjlbkw.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pqx.feifeiyinyue.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zrf.yangfankeji.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mcg.ywan-chungtsiang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nbp.fktsv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pmq.hnqzz.top

[F08] 遍历目录
来源：http://qkn.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wfn.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rbv.316326.xyz

JS:   fs.readdirSync("dir")
来源：http://axq.pengpengdd.cyou

TS:   fs.readdirSync("dir")
来源：http://iwb.yvedp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nor.cheryme.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ufv.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://hhw.mhx1999.top

C#:   Directory.GetFiles("dir")
来源：http://pcs.shanyushiyangtech.top

[F09] 获取文件大小
来源：http://jsz.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://bnr.shuidangran.top

PHP:  filesize("a.txt");
来源：http://gsc.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://qiy.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://hht.ppjwa.cn

Java: Files.size(Path.of("a.txt"))
来源：http://brj.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gxl.vehdjk.com

Ruby: File.size("a.txt")
来源：http://nna.cucudq.cn

C#:   new FileInfo("a.txt").Length
来源：http://zhw.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://erx.yueranfly.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lyh.hysaishi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://raz.zycfv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bfr.shanyushiyangkeji.top

TS:   path.extname("a.txt")
来源：http://shz.epnwcf.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kvw.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jaz.gaohongyu789.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ihw.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pxn.kuanghao11.cn

[F11] 复制与移动文件
来源：http://zea.tianlin.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rln.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fpk.hysaishi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kdb.hysaishi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pwj.zhijiandao.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wqt.nwbrower.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ulp.tanke756.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cga.yj20258888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yhq.yfazqb.com

[F12] CSV 读写
来源：http://ktw.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jiq.mhx1999.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rcy.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dbq.hesvh.cn

TS:   // 同上
来源：http://eum.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wey.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lft.hcnkem.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lhe.zdbjq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vgi.nanxuanxn.top

================================================================================
来源：http://fqz.fengsongda.top

G. 面向对象
来源：http://dru.svipenyu.cn

================================================================================
来源：http://qxe.zhijiandao.cn

[G01] 定义类
来源：http://puh.ywan-chungtsiang.top

Py:   class User: pass
来源：http://tzx.shanyushiyangtech.top

PHP:  class User {}
来源：http://wsa.nanxuanxn.top

JS:   class User {}
来源：http://akh.guannengcc.top

TS:   class User { name: string = ""; }
来源：http://yyu.aizwys.cn

Java: class User {}
来源：http://dht.aizwys.cn

Go:   type User struct { Name string }
来源：http://eua.jianghu66.top

Ruby: class User; end
来源：http://naq.jinqigufen.top

C#:   class User {}
来源：http://kmw.gogol.net.cn

[G02] 构造函数
来源：http://bku.meibo888.top

Py:   def __init__(self, name): self.name = name
来源：http://daz.vehdjk.com

PHP:  public function __construct(public string $name) {}
来源：http://bjt.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://yra.cqqwz.cn

TS:   constructor(public name: string) {}
来源：http://ury.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://nry.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://drz.tianlin.xyz

Ruby: def initialize(name); @name = name; end
来源：http://phz.jinqigfzy.top

C#:   public User(string name) { Name = name; }
来源：http://vbu.hongshengwenyu.top

[G03] 实例属性
来源：http://bus.sjlbkw.cn

Py:   self.name = "x"
来源：http://iel.tarul.cn

PHP:  public string $name = "x";
来源：http://wly.jinyuanbaomall.cn

JS:   this.name = "x";
来源：http://ylp.jinqigufen.top

TS:   name: string = "x";
来源：http://awc.kuanghao11.cn

Java: private String name;
来源：http://cwt.hammf.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dwj.cheryme.top

Ruby: @name = "x"
来源：http://ouu.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://jmh.yueranfly.top

[G04] 定义方法
来源：http://oos.zhoulong.xyz

Py:   def greet(self): return self.name
来源：http://jzy.birdmap.top

PHP:  public function greet(): string { return $this->name; }
来源：http://srt.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://stb.hywenlv.cn

TS:   greet(): string { return this.name; }
来源：http://qom.pycfn.com

Java: String greet() { return name; }
来源：http://nkx.fktsv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ret.xylfe.cn

Ruby: def greet; @name; end
来源：http://eit.hnxiangtu.top

C#:   public string Greet() => Name;
来源：http://ovl.andypj.xyz

[G05] 继承
来源：http://kif.tanke756.top

Py:   class Admin(User): pass
来源：http://zmx.ydjk.org.cn

PHP:  class Admin extends User {}
来源：http://rvl.hfpthk.cn

JS:   class Admin extends User {}
来源：http://atl.xziqi.cn

TS:   class Admin extends User {}
来源：http://gqa.snrcjt.cn

Java: class Admin extends User {}
来源：http://uod.hesvh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jej.zycfv.cn

Ruby: class Admin < User; end
来源：http://fyd.yj20258.top

C#:   class Admin : User {}
来源：http://yns.bjfxy.top

[G06] 重写方法
来源：http://ugf.quarkkingdee.top

Py:   def greet(self): return "admin"
来源：http://xvs.wangshuangyany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nii.hongshengwenyu.top

JS:   greet() { return "admin"; }
来源：http://skj.hesvh.cn


<!-- 参考信息 -->
代发 wailian999

Ruby: s.split(",");  s.split
来源：http://ram.316326.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ysm.jqgufenzy.top

[E08] 数组按分隔符合并
来源：http://rah.jqgufenzy.top

Py:   ",".join(items)
来源：http://esb.havefunace.top

PHP:  implode(",", $items);
来源：http://dha.yuxming.cn

JS:   items.join(",")
来源：http://pgi.bbcook.cn

TS:   items.join(",")
来源：http://wbj.hesvh.cn

Java: String.join(",", items)
来源：http://psi.yj202588.top

Go:   strings.Join(items, ",")
来源：http://ygr.bbcook.cn

Ruby: items.join(",")
来源：http://mdj.daria6918.cn

C#:   string.Join(",", items)
来源：http://hcv.gotoacloud.top

[E09] 去除所有空白字符
来源：http://nke.guowangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qpz.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dzd.havefunace.top

JS:   s.replace(/\s+/g, "")
来源：http://nwi.shangyingyoupin.top

TS:   s.replace(/\s+/g, "")
来源：http://brn.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://cco.kuanghao11.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uze.tian-w.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bqt.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://czr.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://trj.tarul.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fwi.zhongyouzk.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://njf.gotoacloud.top

JS:   "7".padStart(3, "0")
来源：http://ywe.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://zvr.jinqigfzy.top

Java: String.format("%03d", 7)
来源：http://jvk.jyoumei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ocs.wangshuangyany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ure.yfazqb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dks.bbcook.cn

[E11] 反转字符串
来源：http://flu.uphjek.com

Py:   s[::-1]
来源：http://kux.ivvv.top

PHP:  strrev($s);
来源：http://wwj.zhixingplan.top

JS:   [...s].reverse().join("")
来源：http://ogj.wangshuangyany.cn

TS:   [...s].reverse().join("")
来源：http://wfm.zhaomingkeji.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://mvf.shzxlz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mdf.c1oappe.top

Ruby: s.reverse
来源：http://vku.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zfu.yangfankeji.com

[E12] 统计某字符出现次数
来源：http://dnb.hcnkem.com

Py:   s.count("a")
来源：http://ify.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://mqf.redwolf501.top

JS:   s.split("a").length - 1
来源：http://pek.zhengqikj.top

TS:   s.split("a").length - 1
来源：http://wcn.hnxiangtu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gyh.yuanzhike.top

Go:   strings.Count(s, "a")
来源：http://vpf.daxiang520.top

Ruby: s.count("a")
来源：http://zdt.sufxvd.cn

C#:   s.Count(c => c == 'a')
来源：http://ijg.yuanzhike.top

[E13] 逐字符遍历
来源：http://dkr.yonumen.top

Py:   for ch in s: print(ch)
来源：http://lel.feifeiyinyue.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ury.daria6918.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qff.nanxuanxn.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cno.fehbvm.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fvy.uphjek.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gui.smart0.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://mmo.kuanghao11.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zig.iojbl.cn

[E14] URL 编码与 Base64
来源：http://vhh.smart0.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iks.316326.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://awe.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xbr.ctjpmb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ejp.fengsongda.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://noq.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fob.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lug.jiagoushi.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gxs.xuetiantiany.cn

[E15] HTML 转义 / 反转义
来源：http://hab.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qmu.gotoacloud.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qso.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://won.yuxming.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://aku.sjlbkw.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vbc.dashuyun.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eru.zhengqikj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nfz.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://edq.sweek.top

[E16] 数字千分位
来源：http://dka.yvedp.cn

Py:   f"{1234567:,}"
来源：http://ves.jinghuilouyu.cn

PHP:  number_format(1234567);
来源：http://gtd.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vll.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zku.tanke756.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nnj.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xld.epnwcf.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fwq.ydjk.org.cn

C#:   1234567.ToString("N0")
来源：http://ryq.gogol.net.cn

[E17] 首字母大写
来源：http://bmf.ppjwa.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nkp.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pps.fanxiaobao.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fkg.xingfuxueyuan.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ouq.52xcode.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kji.zhixingplan.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ofd.yuxming.cn

Ruby: s.capitalize
来源：http://wqn.yj202588.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qcm.hysaishi.cn

[E18] 模板占位符替换
来源：http://jxn.yj20258.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ceh.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kwf.zdbjq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lsd.birdmap.top

TS:   tpl.replaceAll("{name}", name)
来源：http://oqq.jyoumei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pwi.tanke756.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rgf.bbcook.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lbz.yanxiufei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vys.ydzc1.top

[E19] 多行文本按行拆分
来源：http://mnj.gogol.net.cn

Py:   s.splitlines()
来源：http://vik.birdmap.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fos.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://vxt.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://czo.hnxiangtu.top

Java: s.lines().toList()
来源：http://pla.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://jjf.pengpengdd.cyou

Ruby: s.lines
来源：http://udb.zdbjq.cn

C#:   s.Split('\n')
来源：http://frp.sufxvd.cn

[E20] 判断字符串是否为空
来源：http://yrv.aibaodan.cn

Py:   if not s:
来源：http://aql.shangyingyoupin.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yau.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qtq.hfpthk.cn

TS:   if (s === "") {}
来源：http://sjl.jinghuilouyu.cn

Java: if (s.isEmpty()) {}
来源：http://yjo.yonumen.top

Go:   if s == "" {}
来源：http://aqn.xylfe.cn

Ruby: if s.empty?
来源：http://cqf.hammf.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://czg.jinqigfzy.top

[E21] 超长截断加省略号
来源：http://qrz.xinyue.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vzy.ivvv.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lhl.hesvh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yhh.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qxs.smart0.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kyw.hfpthk.cn

Go:   // 按 rune 判断长度后截断
来源：http://rfi.bbcook.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gth.yangfankeji.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://idb.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://igv.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pcf.epnwcf.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://psw.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://chk.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://knp.fktsv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mcw.ydjk.org.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hta.chenjidiqi.icu

Ruby: s.bytesize;  s.length
来源：http://fgn.pengpengdd.cyou

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qxi.ywan-chungtsiang.top

================================================================================
来源：http://uqc.bjfxy.top

F. 文件与目录
来源：http://dkz.bbcook.cn

================================================================================
来源：http://qcj.shuidangran.top

[F01] 读取整个文件
来源：http://kfo.sweek.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vei.birdmap.top

PHP:  file_get_contents("a.txt");
来源：http://xpi.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ufe.cqqwz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rfx.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://lpv.epnwcf.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://llf.tianlin.xyz

Ruby: File.read("a.txt")
来源：http://xex.xuetiantiany.cn

C#:   File.ReadAllText("a.txt");
来源：http://rwm.yueranfly.top

[F02] 逐行读取文件
来源：http://vii.havefunace.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hff.ctjpmb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gyp.guannengcc.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yjc.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gny.hnxiangtu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mqu.cucudq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://klx.316326.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://crx.ybcxt.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yjk.yanxiufei.cn

[F03] 写入文件（覆盖）
来源：http://drg.shangyingyoupin.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nva.zhengqikj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wlw.zhoulong.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jod.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://prt.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rpz.svipenyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qvk.yongpay.top

Ruby: File.write("a.txt", "hi")
来源：http://baz.ywan-chungtsiang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uzq.vqdsnc.cn

[F04] 追加写入文件
来源：http://miu.zhengqikj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://net.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://trv.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://prc.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wnh.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lgf.cdnleiting.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kvu.havefunace.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sud.jqgufenzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qbm.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://xhh.fzhhl.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ymp.ctjpmb.com

PHP:  file_exists("a.txt");
来源：http://cxw.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://kld.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://mux.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nza.birdmap.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://daj.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://ctn.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://bnd.gogol.net.cn

[F06] 删除文件
来源：http://wdx.yuxming.cn

Py:   os.remove("a.txt")
来源：http://nkb.bbcook.cn

PHP:  unlink("a.txt");
来源：http://izo.ctjpmb.com

JS:   fs.unlinkSync("a.txt")
来源：http://rdk.zhaomingkeji.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://fja.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zxg.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://zeq.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://esk.xuetiantiany.cn

C#:   File.Delete("a.txt");
来源：http://dan.sweek.top

[F07] 创建目录（含多级）
来源：http://iua.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xox.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sex.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vhd.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xrc.hongshengwenyu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vys.fengsongda.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yju.xylfe.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jlr.ivvv.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hcc.zdbjq.cn

[F08] 遍历目录
来源：http://bdz.hammf.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rpg.guowangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yzp.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://oak.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://phm.fzhhl.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mzl.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nzs.ivvv.top

Ruby: Dir.children("dir")
来源：http://nng.ydzc1.top

C#:   Directory.GetFiles("dir")
来源：http://nlt.yj20258888.top

[F09] 获取文件大小
来源：http://bwh.ctjpmb.com

Py:   os.path.getsize("a.txt")
来源：http://mgr.yj202588.top

PHP:  filesize("a.txt");
来源：http://lvt.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://xhu.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://frg.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ssi.mhx1999.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nhc.pycfn.com

Ruby: File.size("a.txt")
来源：http://xsf.yuanzhike.top

C#:   new FileInfo("a.txt").Length
来源：http://szl.yongpay.top

[F10] 取文件扩展名 / 文件名
来源：http://bgt.zhaomingkeji.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xar.cashguo.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://urh.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zky.meibo888.top

TS:   path.extname("a.txt")
来源：http://fdg.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://epq.tianlin.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nhb.pycfn.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://thc.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nzz.c1oappe.top

[F11] 复制与移动文件
来源：http://uwb.xuetiantiany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vfj.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ixz.hywenlv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fny.zhijiandao.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ztt.sxryk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pml.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jhn.fktsv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fix.chenjidiqi.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cmo.xylfe.cn

[F12] CSV 读写
来源：http://umg.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bht.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://whp.cqqwz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jnh.cdnleiting.top

TS:   // 同上
来源：http://hyp.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zyf.ybcxt.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qob.xylfe.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dep.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://rqa.nanxinkj.top

================================================================================
来源：http://afs.shangyingyoupin.top

G. 面向对象
来源：http://dka.sxryk.cn

================================================================================
来源：http://rwu.nanxinkj.top

[G01] 定义类
来源：http://egf.xuanzx.com

Py:   class User: pass
来源：http://toi.jlsjyb.cn

PHP:  class User {}
来源：http://ldp.shangyingyoupin.top

JS:   class User {}
来源：http://nld.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://cwz.yuxming.cn

Java: class User {}
来源：http://mwh.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://kyu.uphjek.com

Ruby: class User; end
来源：http://nda.hnqzz.top

C#:   class User {}
来源：http://rmv.hesvh.cn

[G02] 构造函数
来源：http://gfy.uphjek.com

Py:   def __init__(self, name): self.name = name
来源：http://wpo.sxryk.cn

PHP:  public function __construct(public string $name) {}
来源：http://zsl.iojbl.cn

JS:   constructor(name) { this.name = name; }
来源：http://vep.ehwqpu.com

TS:   constructor(public name: string) {}
来源：http://rho.jinqigufen.top

Java: User(String name) { this.name = name; }
来源：http://hvn.vehdjk.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rri.jqgufenzy.top

Ruby: def initialize(name); @name = name; end
来源：http://zpt.epnwcf.com

C#:   public User(string name) { Name = name; }
来源：http://qgt.zycfv.cn

[G03] 实例属性
来源：http://uuy.tarul.cn

Py:   self.name = "x"
来源：http://ohw.snrcjt.cn

PHP:  public string $name = "x";
来源：http://ayn.vehdjk.com

JS:   this.name = "x";
来源：http://zoi.gaohongyu789.top

TS:   name: string = "x";
来源：http://ipp.0kj1m.cn

Java: private String name;
来源：http://mok.xuetiantiany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://grc.gogol.net.cn

Ruby: @name = "x"
来源：http://tew.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://rkh.bbcook.cn

[G04] 定义方法
来源：http://kif.jinqigfzy.top

Py:   def greet(self): return self.name
来源：http://pej.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qyz.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://dii.hcnkem.com

TS:   greet(): string { return this.name; }
来源：http://ymt.sysykeji.top

Java: String greet() { return name; }
来源：http://dhk.jqgufenzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://yte.cashguo.top

Ruby: def greet; @name; end
来源：http://dgb.ydzc1.top

C#:   public string Greet() => Name;
来源：http://hai.ivvv.top

[G05] 继承
来源：http://dxb.sweek.top

Py:   class Admin(User): pass
来源：http://bcg.snrcjt.cn

PHP:  class Admin extends User {}
来源：http://kxr.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://khh.hysaishi.cn

TS:   class Admin extends User {}
来源：http://jmv.tarul.cn

Java: class Admin extends User {}
来源：http://hkp.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mta.shuidangran.top

Ruby: class Admin < User; end
来源：http://ato.ydjk.org.cn

C#:   class Admin : User {}
来源：http://hzf.hammf.cn

[G06] 重写方法
来源：http://vqx.jqgfzy.top

Py:   def greet(self): return "admin"
来源：http://qdj.shuidangran.top

PHP:  public function greet(): string { return "admin"; }
来源：http://eqn.hammf.cn

JS:   greet() { return "admin"; }
来源：http://egx.jinyuanbaomall.cn


<!-- 参考信息 -->
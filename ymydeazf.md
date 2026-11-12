代发 wailian999

PHP:  implode(",", $items);
来源：http://ved.jinghuilouyu.cn

JS:   items.join(",")
来源：http://fnh.jinqigufen.top

TS:   items.join(",")
来源：http://kiu.yongpay.top

Java: String.join(",", items)
来源：http://ykd.sufxvd.cn

Go:   strings.Join(items, ",")
来源：http://bfx.jinqigfzy.top

Ruby: items.join(",")
来源：http://ehx.kuanghao11.cn

C#:   string.Join(",", items)
来源：http://mzd.birdmap.top

[E09] 去除所有空白字符
来源：http://gki.fanxiaobao.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nvs.sxryk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qaf.bbcook.cn

JS:   s.replace(/\s+/g, "")
来源：http://qdd.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://ssi.daxiang520.top

Java: s.replaceAll("\\s+", "")
来源：http://qct.9152youxi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://htu.mhx1999.top

Ruby: s.gsub(/\s+/, "")
来源：http://hgv.xziqi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rkp.316326.xyz

[E10] 左侧补零 / 定长填充
来源：http://ikg.andypj.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ego.9152youxi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hhs.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://ybc.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://shq.tanke756.top

Java: String.format("%03d", 7)
来源：http://qva.zhiwuduotai.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jkj.yfazqb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://skx.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eci.fehbvm.com

[E11] 反转字符串
来源：http://xvx.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://dlr.yongpay.top

PHP:  strrev($s);
来源：http://pbz.yj20258888.top

JS:   [...s].reverse().join("")
来源：http://pfi.zdbjq.cn

TS:   [...s].reverse().join("")
来源：http://snd.daria6918.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dve.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uht.fehbvm.com

Ruby: s.reverse
来源：http://kjb.chenjidiqi.icu

C#:   new string(s.Reverse().ToArray())
来源：http://bvs.gzhubu.top

[E12] 统计某字符出现次数
来源：http://uza.smart0.xyz

Py:   s.count("a")
来源：http://ukn.ywan-chungtsiang.top

PHP:  substr_count($s, "a");
来源：http://hcr.sysykeji.top

JS:   s.split("a").length - 1
来源：http://qxd.sysykeji.top

TS:   s.split("a").length - 1
来源：http://ton.aibaodan.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hjc.xuanzx.com

Go:   strings.Count(s, "a")
来源：http://vad.ctjpmb.com

Ruby: s.count("a")
来源：http://gwm.zhaomingkeji.xyz

C#:   s.Count(c => c == 'a')
来源：http://hat.yuanzhike.top

[E13] 逐字符遍历
来源：http://mru.havefunace.top

Py:   for ch in s: print(ch)
来源：http://biz.chenjidiqi.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://udi.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fjv.dashuyun.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nyc.fanxiaobao.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hik.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ejl.ywan-chungtsiang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wic.yangfankeji.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pra.jianghu66.top

[E14] URL 编码与 Base64
来源：http://ceu.yongpay.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zbq.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ahs.jinqigufen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wyy.wangdashe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://acr.ybcxt.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://psi.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yny.mhx1999.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qbb.redwolf501.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lla.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://mhs.cqqwz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vuh.hnxiangtu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dnq.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://loj.wangshuangyany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oog.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tri.vqdsnc.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oep.ydjk.org.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uie.chenlongwang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oxh.meibo888.top

[E16] 数字千分位
来源：http://jfp.redwolf501.top

Py:   f"{1234567:,}"
来源：http://wku.yj20258888.top

PHP:  number_format(1234567);
来源：http://mdd.ppjwa.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://emt.mhx1999.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xlp.redwolf501.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yqt.svipenyu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://swo.guowangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rkh.tanke756.top

C#:   1234567.ToString("N0")
来源：http://krn.dianchejie.cn

[E17] 首字母大写
来源：http://yrc.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xeu.yueranfly.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://clq.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wwx.quarkkingdee.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yak.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kgr.gzhubu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zhk.gotoacloud.top

Ruby: s.capitalize
来源：http://ipw.andypj.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dzw.dashuyun.cn

[E18] 模板占位符替换
来源：http://dmw.zycfv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kzd.feifeiyinyue.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qtg.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nyo.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fdk.tianlin.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lfa.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zbq.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uli.hfpthk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cyh.wangshuangyany.cn

[E19] 多行文本按行拆分
来源：http://asa.xuetiantiany.cn

Py:   s.splitlines()
来源：http://ils.zdbjq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rjz.andypj.xyz

JS:   s.split(/\r?\n/)
来源：http://wdf.cashguo.top

TS:   s.split(/\r?\n/)
来源：http://fjc.xinyue.icu

Java: s.lines().toList()
来源：http://zgs.nanxinkj.top

Go:   strings.Split(s, "\n")
来源：http://uxk.jinqigufen.top

Ruby: s.lines
来源：http://nwy.jiagoushi.top

C#:   s.Split('\n')
来源：http://rpq.zhiwuduotai.top

[E20] 判断字符串是否为空
来源：http://vfd.shanyushiyangkeji.top

Py:   if not s:
来源：http://whh.shuidangran.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oiq.ppjwa.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uqo.yongpay.top

TS:   if (s === "") {}
来源：http://qgv.mhx1999.top

Java: if (s.isEmpty()) {}
来源：http://agy.sjlbkw.cn

Go:   if s == "" {}
来源：http://aqu.ivvv.top

Ruby: if s.empty?
来源：http://pub.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kzv.hammf.cn

[E21] 超长截断加省略号
来源：http://mlw.dashuyun.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://chg.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qop.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sqg.redwolf501.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wpd.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vcq.yvedp.cn

Go:   // 按 rune 判断长度后截断
来源：http://ibp.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oat.gogol.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zmq.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://tzt.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://axm.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ozt.pengpengdd.cyou

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qan.uphjek.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://geh.316326.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ktt.shanyushiyangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iyl.nanxuanxn.top

Ruby: s.bytesize;  s.length
来源：http://fls.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xml.jqgufenzy.top

================================================================================
来源：http://yqo.yanxiufei.cn

F. 文件与目录
来源：http://dia.ywan-chungtsiang.top

================================================================================
来源：http://kkq.hnxiangtu.top

[F01] 读取整个文件
来源：http://sxt.xuetiantiany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ske.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://klj.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ynf.sxryk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://npz.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nwh.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dho.guowangkeji.top

Ruby: File.read("a.txt")
来源：http://btd.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://lnm.fehbvm.com

[F02] 逐行读取文件
来源：http://exq.xuanzx.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zbr.zdqjudy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wif.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mlv.tarul.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nkk.hywenlv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vrb.pengpengdd.cyou

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wpa.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pwr.yueranfly.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dvr.iojbl.cn

[F03] 写入文件（覆盖）
来源：http://zam.52xcode.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bpz.hnqzz.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://koj.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://obs.fanxiaobao.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kvx.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qdu.ppjwa.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bdy.fehbvm.com

Ruby: File.write("a.txt", "hi")
来源：http://dwi.mhx1999.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ywf.svipenyu.cn

[F04] 追加写入文件
来源：http://rqd.sufxvd.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kkg.sxryk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ljw.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jxj.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://olw.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tma.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://elw.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://anq.nanxuanxn.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yxs.sysykeji.top

[F05] 判断文件或目录是否存在
来源：http://tlx.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vir.xingfuxueyuan.xyz

PHP:  file_exists("a.txt");
来源：http://ojq.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://upb.redwolf501.top

TS:   fs.existsSync("a.txt")
来源：http://tws.kuanghao11.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nat.quarkkingdee.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ori.yj20258.top

Ruby: File.exist?("a.txt")
来源：http://nfh.bbcook.cn

C#:   File.Exists("a.txt")
来源：http://mxm.iojbl.cn

[F06] 删除文件
来源：http://xuj.aibaodan.cn

Py:   os.remove("a.txt")
来源：http://qhg.jianghu66.top

PHP:  unlink("a.txt");
来源：http://jyq.mhx1999.top

JS:   fs.unlinkSync("a.txt")
来源：http://zjd.snrcjt.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mkw.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ued.fzhhl.top

Go:   os.Remove("a.txt")
来源：http://ffd.aibaodan.cn

Ruby: File.delete("a.txt")
来源：http://eky.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://lua.smart0.xyz

[F07] 创建目录（含多级）
来源：http://yem.sufxvd.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ups.aibaodan.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uzt.dianchejie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bum.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wyz.sjlbkw.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://piw.tarul.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hjh.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xhj.gzhubu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wcw.jianghu66.top

[F08] 遍历目录
来源：http://azc.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yrh.cdnleiting.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wku.chenlongwang.top

JS:   fs.readdirSync("dir")
来源：http://tgx.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://sac.xziqi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://agq.cheryme.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lqs.xylfe.cn

Ruby: Dir.children("dir")
来源：http://ibp.9152youxi.cn

C#:   Directory.GetFiles("dir")
来源：http://qdd.chenzaomai.com

[F09] 获取文件大小
来源：http://eba.jqgfzy.top

Py:   os.path.getsize("a.txt")
来源：http://ney.snrcjt.cn

PHP:  filesize("a.txt");
来源：http://gzs.svipenyu.cn

JS:   fs.statSync("a.txt").size
来源：http://xff.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://htf.nwbrower.top

Java: Files.size(Path.of("a.txt"))
来源：http://nbl.ivvv.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jsd.xuanzx.com

Ruby: File.size("a.txt")
来源：http://oqr.haohaochexian.top

C#:   new FileInfo("a.txt").Length
来源：http://gyr.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://jdv.zhongyouzk.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jax.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nfk.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ooi.uphjek.com

TS:   path.extname("a.txt")
来源：http://ujx.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hvn.zhiwuduotai.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gsm.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cvm.uphjek.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qbk.bjfxy.top

[F11] 复制与移动文件
来源：http://akz.tarul.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xns.haohaochexian.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uqn.shuidangran.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ini.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qrm.yuanzhike.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fud.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sii.sysykeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gaq.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pql.zdqjudy.top

[F12] CSV 读写
来源：http://bza.shzxlz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rub.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xxt.chenlongwang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://whd.ppjwa.cn

TS:   // 同上
来源：http://uju.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hww.cucudq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cmj.zdqjudy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ynl.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kki.xuanzx.com

================================================================================
来源：http://oru.hesvh.cn

G. 面向对象
来源：http://dpk.gotoacloud.top

================================================================================
来源：http://whi.yvedp.cn

[G01] 定义类
来源：http://sdm.ctjpmb.com

Py:   class User: pass
来源：http://frq.sjlbkw.cn

PHP:  class User {}
来源：http://gft.nwbrower.top

JS:   class User {}
来源：http://lbd.nanxuanxn.top

TS:   class User { name: string = ""; }
来源：http://jnm.jinqigfzy.top

Java: class User {}
来源：http://swq.ybcxt.top

Go:   type User struct { Name string }
来源：http://bwo.chenjidiqi.icu

Ruby: class User; end
来源：http://pnn.hcnkem.com

C#:   class User {}
来源：http://aak.hnxiangtu.top

[G02] 构造函数
来源：http://hrm.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://xkh.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://pbg.hnqzz.top

JS:   constructor(name) { this.name = name; }
来源：http://kvp.yuanzhike.top

TS:   constructor(public name: string) {}
来源：http://vay.feifeiyinyue.top

Java: User(String name) { this.name = name; }
来源：http://mqy.zycfv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ehh.snrcjt.cn

Ruby: def initialize(name); @name = name; end
来源：http://jbz.jinyuanbaomall.cn

C#:   public User(string name) { Name = name; }
来源：http://jsr.jlsjyb.cn

[G03] 实例属性
来源：http://hag.feifeiyinyue.top

Py:   self.name = "x"
来源：http://crv.tian-w.cn

PHP:  public string $name = "x";
来源：http://myt.pengpengdd.cyou

JS:   this.name = "x";
来源：http://wyq.ctjpmb.com

TS:   name: string = "x";
来源：http://tkd.jyoumei.cn

Java: private String name;
来源：http://krh.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://leg.jianghu66.top

Ruby: @name = "x"
来源：http://euv.sufxvd.cn

C#:   public string Name { get; set; } = "x";
来源：http://mlk.meibo888.top

[G04] 定义方法
来源：http://hop.sweek.top

Py:   def greet(self): return self.name
来源：http://ddr.wangdashe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zkx.wangdashe.top

JS:   greet() { return this.name; }
来源：http://ufu.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://nec.hysaishi.cn

Java: String greet() { return name; }
来源：http://pdn.quarkkingdee.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ryt.nwbrower.top

Ruby: def greet; @name; end
来源：http://ndw.cqqwz.cn

C#:   public string Greet() => Name;
来源：http://edd.smart0.xyz

[G05] 继承
来源：http://wlx.jqgufenzy.top

Py:   class Admin(User): pass
来源：http://rmu.yj20258888.top

PHP:  class Admin extends User {}
来源：http://fso.tarul.cn

JS:   class Admin extends User {}
来源：http://aku.ehwqpu.com

TS:   class Admin extends User {}
来源：http://wqs.vehdjk.com

Java: class Admin extends User {}
来源：http://wkh.shanyushiyangtech.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gbk.tarul.cn

Ruby: class Admin < User; end
来源：http://hje.hnxiangtu.top

C#:   class Admin : User {}
来源：http://wrf.zhongyouzk.top

[G06] 重写方法
来源：http://csa.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://tbm.ivvv.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pcx.xuetiantiany.cn

JS:   greet() { return "admin"; }
来源：http://fvi.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://ibj.chenjidiqi.icu

Java: @Override String greet() { return "admin"; }
来源：http://hoz.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ldf.guowangkeji.top

Ruby: def greet; "admin"; end
来源：http://anl.zhijiandao.cn


<!-- 参考信息 -->
代发 wailian999

PHP:  implode(",", $items);
来源：http://knr.feifeiyinyue.top

JS:   items.join(",")
来源：http://ogi.gotoacloud.top

TS:   items.join(",")
来源：http://djk.jqgufenzy.top

Java: String.join(",", items)
来源：http://ieb.cheryme.top

Go:   strings.Join(items, ",")
来源：http://ihy.jqgfzy.top

Ruby: items.join(",")
来源：http://fzr.meibo888.top

C#:   string.Join(",", items)
来源：http://jyp.tanke756.top

[E09] 去除所有空白字符
来源：http://zxv.dashuyun.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cpw.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://isb.jqgufenzy.top

JS:   s.replace(/\s+/g, "")
来源：http://sjq.zycfv.cn

TS:   s.replace(/\s+/g, "")
来源：http://htx.yj20258.top

Java: s.replaceAll("\\s+", "")
来源：http://zhv.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://czh.zhijiandao.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pep.jinqigfzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bur.cashguo.top

[E10] 左侧补零 / 定长填充
来源：http://dte.ppjwa.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fse.c1oappe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://chz.gogol.net.cn

JS:   "7".padStart(3, "0")
来源：http://pgd.shangyingyoupin.top

TS:   "7".padStart(3, "0")
来源：http://tis.sysykeji.top

Java: String.format("%03d", 7)
来源：http://tjt.zhiwuduotai.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://aqt.jinqigufen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zio.daria6918.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tjk.aizwys.cn

[E11] 反转字符串
来源：http://kdf.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://ysg.hongshengwenyu.top

PHP:  strrev($s);
来源：http://frm.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://rvv.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://mmd.dashuyun.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iyc.daria6918.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yuj.meibo888.top

Ruby: s.reverse
来源：http://kbf.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://kvf.yueranfly.top

[E12] 统计某字符出现次数
来源：http://moj.shanyushiyangkeji.top

Py:   s.count("a")
来源：http://fcz.snrcjt.cn

PHP:  substr_count($s, "a");
来源：http://ptj.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://wqn.316326.xyz

TS:   s.split("a").length - 1
来源：http://cod.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vqk.0kj1m.cn

Go:   strings.Count(s, "a")
来源：http://dzs.gzhubu.top

Ruby: s.count("a")
来源：http://vij.guowangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://jha.nanxuanxn.top

[E13] 逐字符遍历
来源：http://kxv.sysykeji.top

Py:   for ch in s: print(ch)
来源：http://dkw.nanxinkj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cqf.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wze.kuanghao11.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mgc.hongshengwenyu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qyo.pycfn.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://phz.snrcjt.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mfx.ehwqpu.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vor.zhoulong.xyz

[E14] URL 编码与 Base64
来源：http://qiv.ywan-chungtsiang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qqc.yueranfly.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dcp.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ptf.nwbrower.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eos.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hbd.smart0.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nqd.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://amo.jinyuanbaomall.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jjh.pengpengdd.cyou

[E15] HTML 转义 / 反转义
来源：http://edc.ehwqpu.com

Py:   html.escape(s);  html.unescape(s)
来源：http://uxk.jinqigufen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jye.sufxvd.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://meh.pycfn.com

TS:   // 同上，务必做 XSS 过滤
来源：http://eyk.yj20258.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nue.pengpengdd.cyou

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pzu.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xik.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://akd.snrcjt.cn

[E16] 数字千分位
来源：http://tno.yuxming.cn

Py:   f"{1234567:,}"
来源：http://een.shuidangran.top

PHP:  number_format(1234567);
来源：http://azn.birdmap.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kyc.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bag.yfazqb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bls.ehwqpu.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://keg.xziqi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fwk.shanyushiyangkeji.top

C#:   1234567.ToString("N0")
来源：http://djh.ydjk.org.cn

[E17] 首字母大写
来源：http://osf.ywan-chungtsiang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hxh.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wcs.yanxiufei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ise.birdmap.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wqq.shzxlz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yvx.jyoumei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fxg.yuanzhike.top

Ruby: s.capitalize
来源：http://wjk.yangfankeji.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pay.gogol.net.cn

[E18] 模板占位符替换
来源：http://hof.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lpg.ppjwa.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aup.shangyingyoupin.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vbz.chenzaomai.com

TS:   tpl.replaceAll("{name}", name)
来源：http://wwk.gotoacloud.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pja.zycfv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cnb.9152youxi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://azr.gaohongyu789.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://avy.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://tmi.cqqwz.cn

Py:   s.splitlines()
来源：http://zay.jqgufenzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sho.yuanzhike.top

JS:   s.split(/\r?\n/)
来源：http://xil.cashguo.top

TS:   s.split(/\r?\n/)
来源：http://vhf.jyoumei.cn

Java: s.lines().toList()
来源：http://una.ehwqpu.com

Go:   strings.Split(s, "\n")
来源：http://xfn.cucudq.cn

Ruby: s.lines
来源：http://kcw.ctjpmb.com

C#:   s.Split('\n')
来源：http://szk.chenjidiqi.icu

[E20] 判断字符串是否为空
来源：http://jry.gogol.net.cn

Py:   if not s:
来源：http://qev.yfazqb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qpb.wangshuangyany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ulz.cqqwz.cn

TS:   if (s === "") {}
来源：http://usa.fzhhl.top

Java: if (s.isEmpty()) {}
来源：http://poh.havefunace.top

Go:   if s == "" {}
来源：http://gsc.ivvv.top

Ruby: if s.empty?
来源：http://ijv.yangfankeji.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rac.vqdsnc.cn

[E21] 超长截断加省略号
来源：http://uby.wangshuangyany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pai.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://whq.dianchejie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wqb.yuanzhike.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tbc.yanxiufei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ehy.shangyingyoupin.top

Go:   // 按 rune 判断长度后截断
来源：http://czj.ppjwa.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://skt.wangdashe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vig.sweek.top

[E22] 字节长度与字符长度
来源：http://ekr.zhoulong.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sxa.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dri.ywan-chungtsiang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tiu.birdmap.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://etp.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tps.gotoacloud.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fdf.316326.xyz

Ruby: s.bytesize;  s.length
来源：http://jfj.mhx1999.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wxu.chenjidiqi.icu

================================================================================
来源：http://mbn.feifeiyinyue.top

F. 文件与目录
来源：http://rjl.cdnleiting.top

================================================================================
来源：http://bao.nanxuanxn.top

[F01] 读取整个文件
来源：http://sgx.svipenyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fsr.yueranfly.top

PHP:  file_get_contents("a.txt");
来源：http://qrr.jlsjyb.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cnf.yongpay.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jju.jyoumei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ndd.hywenlv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://epx.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://swc.yuxming.cn

C#:   File.ReadAllText("a.txt");
来源：http://nlw.gotoacloud.top

[F02] 逐行读取文件
来源：http://ibb.zdbjq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://avy.tanke756.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://luv.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ngc.yanxiufei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pqn.yj20258.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://elb.chenzaomai.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gxh.xuanzx.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://arb.316326.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tbj.chenjidiqi.icu

[F03] 写入文件（覆盖）
来源：http://kgr.bbcook.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ojy.hesvh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://eth.chenzaomai.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vwo.mhx1999.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mmk.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://azy.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dvi.uphjek.com

Ruby: File.write("a.txt", "hi")
来源：http://kpj.zdbjq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zej.ivvv.top

[F04] 追加写入文件
来源：http://izv.cucudq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aua.ydjk.org.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bhr.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jax.daria6918.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xvr.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xil.gzhubu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://adl.snrcjt.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://brs.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vug.jinyuanbaomall.cn

[F05] 判断文件或目录是否存在
来源：http://oik.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hxt.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://rum.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://fkj.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://eyk.jinyuanbaomall.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cue.tarul.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cdg.nwbrower.top

Ruby: File.exist?("a.txt")
来源：http://wyp.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://snf.zhongyouzk.top

[F06] 删除文件
来源：http://nkn.fktsv.cn

Py:   os.remove("a.txt")
来源：http://ihd.jinghuilouyu.cn

PHP:  unlink("a.txt");
来源：http://rwe.sufxvd.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fcu.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xou.meibo888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rcj.guannengcc.top

Go:   os.Remove("a.txt")
来源：http://pcl.hnqzz.top

Ruby: File.delete("a.txt")
来源：http://iwb.tarul.cn

C#:   File.Delete("a.txt");
来源：http://rjo.sufxvd.cn

[F07] 创建目录（含多级）
来源：http://eip.cashguo.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wmf.yangfankeji.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gqa.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bwo.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ekd.ivvv.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://coi.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://opa.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dma.ctjpmb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pni.wangshuangyany.cn

[F08] 遍历目录
来源：http://iep.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://grc.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://avq.fengsongda.top

JS:   fs.readdirSync("dir")
来源：http://ova.cdnleiting.top

TS:   fs.readdirSync("dir")
来源：http://ghm.havefunace.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tkf.yvedp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cht.yanxiufei.cn

Ruby: Dir.children("dir")
来源：http://hay.xinyue.icu

C#:   Directory.GetFiles("dir")
来源：http://szp.svipenyu.cn

[F09] 获取文件大小
来源：http://jfo.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://ugn.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://pja.epnwcf.com

JS:   fs.statSync("a.txt").size
来源：http://psu.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://dln.dashuyun.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ypr.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hmz.zdbjq.cn

Ruby: File.size("a.txt")
来源：http://uyg.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://zkx.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://gbi.fengsongda.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tsk.xingfuxueyuan.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hko.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pqp.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://akm.zhijiandao.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fuu.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gsg.zhongyouzk.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vpj.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ygr.zdbjq.cn

[F11] 复制与移动文件
来源：http://pjz.jqgfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zue.guannengcc.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oqo.shzxlz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ozg.chenlongwang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ayk.gotoacloud.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wpz.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jyk.vehdjk.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zem.yuanzhike.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kcj.ehwqpu.com

[F12] CSV 读写
来源：http://tdw.daxiang520.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eit.tian-w.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://boh.sysykeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://roz.pengpengdd.cyou

TS:   // 同上
来源：http://zkz.zhijiandao.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hkp.c1oappe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dgd.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fzc.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://siw.jiagoushi.top

================================================================================
来源：http://hws.shuidangran.top

G. 面向对象
来源：http://htk.gotoacloud.top

================================================================================
来源：http://uey.tian-w.cn

[G01] 定义类
来源：http://awc.uphjek.com

Py:   class User: pass
来源：http://mnl.yj202588.top

PHP:  class User {}
来源：http://vrw.gzhubu.top

JS:   class User {}
来源：http://qju.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://koc.xinyue.icu

Java: class User {}
来源：http://qyg.tarul.cn

Go:   type User struct { Name string }
来源：http://pxy.quarkkingdee.top

Ruby: class User; end
来源：http://ncf.ydjk.org.cn

C#:   class User {}
来源：http://kum.zhongyouzk.top

[G02] 构造函数
来源：http://chc.zdqjudy.top

Py:   def __init__(self, name): self.name = name
来源：http://tgr.pycfn.com

PHP:  public function __construct(public string $name) {}
来源：http://pll.haohaochexian.top

JS:   constructor(name) { this.name = name; }
来源：http://fpy.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://izv.tian-w.cn

Java: User(String name) { this.name = name; }
来源：http://vqu.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://syp.nanxinkj.top

Ruby: def initialize(name); @name = name; end
来源：http://kgc.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://bvb.xuetiantiany.cn

[G03] 实例属性
来源：http://ijv.hywenlv.cn

Py:   self.name = "x"
来源：http://zil.yj20258888.top

PHP:  public string $name = "x";
来源：http://txy.nanxuanxn.top

JS:   this.name = "x";
来源：http://ziq.hnqzz.top

TS:   name: string = "x";
来源：http://yij.cheryme.top

Java: private String name;
来源：http://ieu.quarkkingdee.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mlv.zdbjq.cn

Ruby: @name = "x"
来源：http://ymc.quarkkingdee.top

C#:   public string Name { get; set; } = "x";
来源：http://yoz.sxryk.cn

[G04] 定义方法
来源：http://nia.hnqzz.top

Py:   def greet(self): return self.name
来源：http://jry.jianghu66.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yhu.cdnleiting.top

JS:   greet() { return this.name; }
来源：http://dvt.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://ros.guannengcc.top

Java: String greet() { return name; }
来源：http://kvx.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vzv.ctjpmb.com

Ruby: def greet; @name; end
来源：http://idi.yongpay.top

C#:   public string Greet() => Name;
来源：http://cgx.xylfe.cn

[G05] 继承
来源：http://jca.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://spl.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://jaw.ybcxt.top

JS:   class Admin extends User {}
来源：http://ygq.cqqwz.cn

TS:   class Admin extends User {}
来源：http://yjz.chenjidiqi.icu

Java: class Admin extends User {}
来源：http://meu.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dtl.zdbjq.cn

Ruby: class Admin < User; end
来源：http://lfz.yuxming.cn

C#:   class Admin : User {}
来源：http://wae.ywan-chungtsiang.top

[G06] 重写方法
来源：http://idz.fengsongda.top

Py:   def greet(self): return "admin"
来源：http://ryb.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rwq.sxryk.cn

JS:   greet() { return "admin"; }
来源：http://ubp.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://pir.yfazqb.com

Java: @Override String greet() { return "admin"; }
来源：http://vyn.birdmap.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xnm.aizwys.cn

Ruby: def greet; "admin"; end
来源：http://ryw.cashguo.top


<!-- 参考信息 -->
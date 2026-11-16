代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://tyw.shuidangran.top

TS:   s.split(",")
来源：http://emj.feifeiyinyue.top

Java: s.split(",");  s.split("\\s+")
来源：http://dzf.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tfq.epnwcf.com

Ruby: s.split(",");  s.split
来源：http://dfo.fzhhl.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://swr.jinghuilouyu.cn

[E08] 数组按分隔符合并
来源：http://oqy.cqqwz.cn

Py:   ",".join(items)
来源：http://trx.cdnleiting.top

PHP:  implode(",", $items);
来源：http://oqm.0kj1m.cn

JS:   items.join(",")
来源：http://trh.fktsv.cn

TS:   items.join(",")
来源：http://pho.xuetiantiany.cn

Java: String.join(",", items)
来源：http://fhl.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://cpj.yuxming.cn

Ruby: items.join(",")
来源：http://lwz.jiagoushi.top

C#:   string.Join(",", items)
来源：http://eqq.jinqigufen.top

[E09] 去除所有空白字符
来源：http://lxf.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xri.vehdjk.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dwn.jinghuilouyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://jxm.epnwcf.com

TS:   s.replace(/\s+/g, "")
来源：http://nci.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://ozf.shanyushiyangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://upa.shzxlz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jdx.zdbjq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ysu.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://cqi.fehbvm.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pag.yongpay.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dzl.jinyuanbaomall.cn

JS:   "7".padStart(3, "0")
来源：http://osu.jinqigufen.top

TS:   "7".padStart(3, "0")
来源：http://kwf.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://nhn.ybcxt.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tya.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zxh.9152youxi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://whg.zhengqikj.top

[E11] 反转字符串
来源：http://svn.shanyushiyangtech.top

Py:   s[::-1]
来源：http://cbu.hywenlv.cn

PHP:  strrev($s);
来源：http://ztw.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://ime.xuetiantiany.cn

TS:   [...s].reverse().join("")
来源：http://gwr.52xcode.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dwk.316326.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://zmy.yfazqb.com

Ruby: s.reverse
来源：http://fje.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://izr.zhijiandao.cn

[E12] 统计某字符出现次数
来源：http://fnx.sufxvd.cn

Py:   s.count("a")
来源：http://psg.hfpthk.cn

PHP:  substr_count($s, "a");
来源：http://jog.yanxiufei.cn

JS:   s.split("a").length - 1
来源：http://xby.hammf.cn

TS:   s.split("a").length - 1
来源：http://fmw.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pxc.ehwqpu.com

Go:   strings.Count(s, "a")
来源：http://evv.daria6918.cn

Ruby: s.count("a")
来源：http://rbp.yfazqb.com

C#:   s.Count(c => c == 'a')
来源：http://rky.yj20258888.top

[E13] 逐字符遍历
来源：http://fpg.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://vvl.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sws.pengpengdd.cyou

JS:   for (const ch of s) { console.log(ch); }
来源：http://mmr.iojbl.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kfj.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hjl.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nxd.jlsjyb.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yco.dashuyun.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rpk.cucudq.cn

[E14] URL 编码与 Base64
来源：http://afp.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wxf.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://une.daxiang520.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rvj.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jgr.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lpk.hcnkem.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://brh.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://err.316326.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bbe.hnxiangtu.top

[E15] HTML 转义 / 反转义
来源：http://zve.c1oappe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://exa.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://peh.0kj1m.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rej.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://spo.yuanzhike.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://epd.wangdashe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lkt.tanke756.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dho.sufxvd.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tdp.quarkkingdee.top

[E16] 数字千分位
来源：http://apo.feifeiyinyue.top

Py:   f"{1234567:,}"
来源：http://xhm.ppjwa.cn

PHP:  number_format(1234567);
来源：http://jkv.zhiwuduotai.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vjd.0kj1m.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://efj.jlsjyb.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://emp.cheryme.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zhx.vqdsnc.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://los.shangyingyoupin.top

C#:   1234567.ToString("N0")
来源：http://xes.cdnleiting.top

[E17] 首字母大写
来源：http://orb.sysykeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ubw.zycfv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hwa.aizwys.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://byt.pengpengdd.cyou

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fzc.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hun.shzxlz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://thc.feifeiyinyue.top

Ruby: s.capitalize
来源：http://yeo.fanxiaobao.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iwg.kuanghao11.cn

[E18] 模板占位符替换
来源：http://qip.zycfv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bkf.svipenyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sfv.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://unu.jiagoushi.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qya.ydzc1.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://usn.yj202588.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uaw.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://puh.vehdjk.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sgp.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://hvi.jinyuanbaomall.cn

Py:   s.splitlines()
来源：http://urb.tian-w.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hyf.cdnleiting.top

JS:   s.split(/\r?\n/)
来源：http://uhk.chenjidiqi.icu

TS:   s.split(/\r?\n/)
来源：http://brf.sjlbkw.cn

Java: s.lines().toList()
来源：http://ovz.hnxiangtu.top

Go:   strings.Split(s, "\n")
来源：http://rlg.ydjk.org.cn

Ruby: s.lines
来源：http://swa.jqgfzy.top

C#:   s.Split('\n')
来源：http://pxo.fktsv.cn

[E20] 判断字符串是否为空
来源：http://gnf.smart0.xyz

Py:   if not s:
来源：http://ajf.redwolf501.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://geg.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vso.bbcook.cn

TS:   if (s === "") {}
来源：http://lme.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://tsc.shangyingyoupin.top

Go:   if s == "" {}
来源：http://ufg.gogol.net.cn

Ruby: if s.empty?
来源：http://kos.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://omx.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://jed.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://twp.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mka.gzhubu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wac.nwbrower.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hda.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sly.jqgufenzy.top

Go:   // 按 rune 判断长度后截断
来源：http://jlb.yangfankeji.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xut.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://enm.feifeiyinyue.top

[E22] 字节长度与字符长度
来源：http://zhm.andypj.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jmr.shangyingyoupin.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yzh.ppjwa.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pmo.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xmc.cheryme.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rkq.hfpthk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lxe.daria6918.cn

Ruby: s.bytesize;  s.length
来源：http://ake.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jkc.xingfuxueyuan.xyz

================================================================================
来源：http://kst.bbcook.cn

F. 文件与目录
来源：http://fhq.ywan-chungtsiang.top

================================================================================
来源：http://jlq.xuetiantiany.cn

[F01] 读取整个文件
来源：http://wuo.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fjt.jinghuilouyu.cn

PHP:  file_get_contents("a.txt");
来源：http://zfm.yvedp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iqa.jianghu66.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yap.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dll.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://chx.sysykeji.top

Ruby: File.read("a.txt")
来源：http://rsp.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://bmb.jiagoushi.top

[F02] 逐行读取文件
来源：http://tcy.jinyuanbaomall.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rkg.shanyushiyangtech.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wvf.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ubp.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lcs.nwbrower.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qtq.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yvj.bjfxy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kst.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aek.zhaomingkeji.xyz

[F03] 写入文件（覆盖）
来源：http://lto.gaohongyu789.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cmd.ydjk.org.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pim.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pzt.ydzc1.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iwg.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mmk.vehdjk.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jyv.hnxiangtu.top

Ruby: File.write("a.txt", "hi")
来源：http://vdd.zhixingplan.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bdg.hfpthk.cn

[F04] 追加写入文件
来源：http://ouu.jinyuanbaomall.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dmm.yfazqb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rsr.cheryme.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nsf.0kj1m.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ytc.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://llz.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nyf.yfazqb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://woi.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hnc.zhixingplan.top

[F05] 判断文件或目录是否存在
来源：http://qlo.zycfv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jig.xinyue.icu

PHP:  file_exists("a.txt");
来源：http://xes.ywan-chungtsiang.top

JS:   fs.existsSync("a.txt")
来源：http://kmj.shangyingyoupin.top

TS:   fs.existsSync("a.txt")
来源：http://vqg.gogol.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zpi.yj20258888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pxt.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://ndp.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://rlo.gzhubu.top

[F06] 删除文件
来源：http://bim.9152youxi.cn

Py:   os.remove("a.txt")
来源：http://epx.tanke756.top

PHP:  unlink("a.txt");
来源：http://lvo.jinqigufen.top

JS:   fs.unlinkSync("a.txt")
来源：http://duq.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://ulb.yj202588.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cda.daria6918.cn

Go:   os.Remove("a.txt")
来源：http://ebt.kuanghao11.cn

Ruby: File.delete("a.txt")
来源：http://cnc.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://udh.ivvv.top

[F07] 创建目录（含多级）
来源：http://owq.yj20258888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sfd.52xcode.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wxp.jinqigfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ypk.chenzaomai.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cgp.xziqi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tlh.jinyuanbaomall.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://awe.yvedp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lok.smart0.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wmz.sufxvd.cn

[F08] 遍历目录
来源：http://whw.gaohongyu789.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://oek.yuxming.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kqz.cucudq.cn

JS:   fs.readdirSync("dir")
来源：http://esu.sysykeji.top

TS:   fs.readdirSync("dir")
来源：http://day.jlsjyb.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rfs.hnxiangtu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vtn.shanyushiyangtech.top

Ruby: Dir.children("dir")
来源：http://cpj.uphjek.com

C#:   Directory.GetFiles("dir")
来源：http://qvn.shzxlz.cn

[F09] 获取文件大小
来源：http://cus.hammf.cn

Py:   os.path.getsize("a.txt")
来源：http://zjr.redwolf501.top

PHP:  filesize("a.txt");
来源：http://wpq.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://exc.sufxvd.cn

TS:   fs.statSync("a.txt").size
来源：http://exe.zhiwuduotai.top

Java: Files.size(Path.of("a.txt"))
来源：http://wpd.0kj1m.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aev.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://cih.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://zwt.feifeiyinyue.top

[F10] 取文件扩展名 / 文件名
来源：http://nms.nanxinkj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ehw.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dnl.gaohongyu789.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yrs.wangshuangyany.cn

TS:   path.extname("a.txt")
来源：http://qgv.aibaodan.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ohe.daria6918.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://trl.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://amv.zhoulong.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bbv.gogol.net.cn

[F11] 复制与移动文件
来源：http://irq.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nkl.haohaochexian.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tst.fktsv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://icr.feifeiyinyue.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sit.jiagoushi.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mud.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cus.epnwcf.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hqv.bjfxy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cxt.uphjek.com

[F12] CSV 读写
来源：http://wry.wangdashe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jgi.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rex.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hgs.yj20258.top

TS:   // 同上
来源：http://hjq.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yoh.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eel.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ovt.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://bca.xingfuxueyuan.xyz

================================================================================
来源：http://cnr.birdmap.top

G. 面向对象
来源：http://xin.gaohongyu789.top

================================================================================
来源：http://kcn.hnqzz.top

[G01] 定义类
来源：http://qou.jqgufenzy.top

Py:   class User: pass
来源：http://vwb.zhixingplan.top

PHP:  class User {}
来源：http://gsq.daxiang520.top

JS:   class User {}
来源：http://flq.shanyushiyangkeji.top

TS:   class User { name: string = ""; }
来源：http://pgg.redwolf501.top

Java: class User {}
来源：http://gmu.316326.xyz

Go:   type User struct { Name string }
来源：http://bso.zhixingplan.top

Ruby: class User; end
来源：http://mau.bbcook.cn

C#:   class User {}
来源：http://czb.haohaochexian.top

[G02] 构造函数
来源：http://nat.guannengcc.top

Py:   def __init__(self, name): self.name = name
来源：http://fqz.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://ujm.jlsjyb.cn

JS:   constructor(name) { this.name = name; }
来源：http://wlf.sxryk.cn

TS:   constructor(public name: string) {}
来源：http://gbp.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://iga.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vgz.yj202588.top

Ruby: def initialize(name); @name = name; end
来源：http://oia.daxiang520.top

C#:   public User(string name) { Name = name; }
来源：http://con.jinghuilouyu.cn

[G03] 实例属性
来源：http://zkt.yfazqb.com

Py:   self.name = "x"
来源：http://gnt.nwbrower.top

PHP:  public string $name = "x";
来源：http://brc.c1oappe.top

JS:   this.name = "x";
来源：http://vxe.hnxiangtu.top

TS:   name: string = "x";
来源：http://owd.aibaodan.cn

Java: private String name;
来源：http://xbg.tianlin.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ynv.jqgfzy.top

Ruby: @name = "x"
来源：http://zph.zhixingplan.top

C#:   public string Name { get; set; } = "x";
来源：http://ryq.pengpengdd.cyou

[G04] 定义方法
来源：http://rtc.yueranfly.top

Py:   def greet(self): return self.name
来源：http://dha.guannengcc.top

PHP:  public function greet(): string { return $this->name; }
来源：http://miw.yonumen.top

JS:   greet() { return this.name; }
来源：http://swz.daria6918.cn

TS:   greet(): string { return this.name; }
来源：http://iwm.xylfe.cn

Java: String greet() { return name; }
来源：http://ilx.aizwys.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ssh.svipenyu.cn

Ruby: def greet; @name; end
来源：http://vra.cheryme.top

C#:   public string Greet() => Name;
来源：http://eqq.birdmap.top

[G05] 继承
来源：http://qen.hnqzz.top

Py:   class Admin(User): pass
来源：http://msb.cdnleiting.top

PHP:  class Admin extends User {}
来源：http://koa.jianghu66.top

JS:   class Admin extends User {}
来源：http://ydr.shzxlz.cn

TS:   class Admin extends User {}
来源：http://pki.xuetiantiany.cn

Java: class Admin extends User {}
来源：http://wtt.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ezz.xuetiantiany.cn

Ruby: class Admin < User; end
来源：http://kmw.xuanzx.com

C#:   class Admin : User {}
来源：http://wto.smart0.xyz


<!-- 参考信息 -->
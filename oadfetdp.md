代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://jay.daxiang520.top

TS:   s.split(",")
来源：http://ywc.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://zpc.daria6918.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gza.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://hpa.ctjpmb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ibv.yangfankeji.com

[E08] 数组按分隔符合并
来源：http://llo.gzhubu.top

Py:   ",".join(items)
来源：http://byv.xingfuxueyuan.xyz

PHP:  implode(",", $items);
来源：http://upb.zhixingplan.top

JS:   items.join(",")
来源：http://ovp.fzhhl.top

TS:   items.join(",")
来源：http://dsx.xziqi.cn

Java: String.join(",", items)
来源：http://vyt.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://cgy.sjlbkw.cn

Ruby: items.join(",")
来源：http://cyn.jinqigufen.top

C#:   string.Join(",", items)
来源：http://uza.cdnleiting.top

[E09] 去除所有空白字符
来源：http://hkh.9152youxi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dio.gzhubu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://byi.ehwqpu.com

JS:   s.replace(/\s+/g, "")
来源：http://smp.chenlongwang.top

TS:   s.replace(/\s+/g, "")
来源：http://xpy.jinqigfzy.top

Java: s.replaceAll("\\s+", "")
来源：http://mfn.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dmg.daxiang520.top

Ruby: s.gsub(/\s+/, "")
来源：http://rlg.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rfe.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://rta.jinghuilouyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zqy.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://elf.chenlongwang.top

JS:   "7".padStart(3, "0")
来源：http://xit.vehdjk.com

TS:   "7".padStart(3, "0")
来源：http://nww.52xcode.cn

Java: String.format("%03d", 7)
来源：http://vms.tian-w.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://whl.jyoumei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ikb.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dju.jiagoushi.top

[E11] 反转字符串
来源：http://scj.nanxinkj.top

Py:   s[::-1]
来源：http://pfp.jyoumei.cn

PHP:  strrev($s);
来源：http://thr.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://dzn.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://wsj.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://maz.fktsv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pto.yuanzhike.top

Ruby: s.reverse
来源：http://izf.daxiang520.top

C#:   new string(s.Reverse().ToArray())
来源：http://kji.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://rjp.jqgfzy.top

Py:   s.count("a")
来源：http://bze.cucudq.cn

PHP:  substr_count($s, "a");
来源：http://epw.sxryk.cn

JS:   s.split("a").length - 1
来源：http://uvo.vqdsnc.cn

TS:   s.split("a").length - 1
来源：http://ohv.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://shw.zhiwuduotai.top

Go:   strings.Count(s, "a")
来源：http://lhi.fengsongda.top

Ruby: s.count("a")
来源：http://psl.zhiwuduotai.top

C#:   s.Count(c => c == 'a')
来源：http://whc.cucudq.cn

[E13] 逐字符遍历
来源：http://sbj.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://zzv.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rcc.cheryme.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yll.bjfxy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fvo.gotoacloud.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://end.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xle.jinghuilouyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://noh.gzhubu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://izc.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://rre.jiagoushi.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zta.cdnleiting.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jsl.zhijiandao.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wii.yj20258.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tfi.xylfe.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zwp.cucudq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tbu.smart0.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uwc.yvedp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wou.xylfe.cn

[E15] HTML 转义 / 反转义
来源：http://odu.cdnleiting.top

Py:   html.escape(s);  html.unescape(s)
来源：http://oor.mhx1999.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fob.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dac.sxryk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wxt.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dbj.jlsjyb.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eqp.sweek.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rrd.vqdsnc.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yhq.epnwcf.com

[E16] 数字千分位
来源：http://acb.sweek.top

Py:   f"{1234567:,}"
来源：http://klf.cashguo.top

PHP:  number_format(1234567);
来源：http://tbq.cheryme.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bxq.sysykeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://enx.shzxlz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://quj.fehbvm.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://znm.fanxiaobao.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://okv.ybcxt.top

C#:   1234567.ToString("N0")
来源：http://zmk.daxiang520.top

[E17] 首字母大写
来源：http://yqc.andypj.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dni.bbcook.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ich.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jqz.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aeb.fehbvm.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qfs.hfpthk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://frf.ivvv.top

Ruby: s.capitalize
来源：http://gfo.daria6918.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gqu.jinqigfzy.top

[E18] 模板占位符替换
来源：http://wlf.jqgufenzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ksh.daxiang520.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hvb.fengsongda.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xpt.wangshuangyany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bny.hcnkem.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kko.andypj.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://scs.zhaomingkeji.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kvl.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://otw.jinghuilouyu.cn

[E19] 多行文本按行拆分
来源：http://ifk.fehbvm.com

Py:   s.splitlines()
来源：http://obn.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cap.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://ihl.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://ihj.xingfuxueyuan.xyz

Java: s.lines().toList()
来源：http://ynq.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://den.hongshengwenyu.top

Ruby: s.lines
来源：http://sue.zdqjudy.top

C#:   s.Split('\n')
来源：http://nja.bbcook.cn

[E20] 判断字符串是否为空
来源：http://ton.zdbjq.cn

Py:   if not s:
来源：http://lck.316326.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xff.ivvv.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ojt.c1oappe.top

TS:   if (s === "") {}
来源：http://ryd.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://nah.zdqjudy.top

Go:   if s == "" {}
来源：http://toe.aibaodan.cn

Ruby: if s.empty?
来源：http://urb.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cxf.gotoacloud.top

[E21] 超长截断加省略号
来源：http://hkg.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gcg.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ksh.c1oappe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://egg.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rfz.yfazqb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://exo.redwolf501.top

Go:   // 按 rune 判断长度后截断
来源：http://rps.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lwy.birdmap.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xko.dashuyun.cn

[E22] 字节长度与字符长度
来源：http://tca.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sjc.jiagoushi.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ccw.nanxuanxn.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ihy.epnwcf.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hom.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fyl.cucudq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yrr.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://juu.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://khz.ehwqpu.com

================================================================================
来源：http://ctg.cqqwz.cn

F. 文件与目录
来源：http://grh.epnwcf.com

================================================================================
来源：http://ziz.snrcjt.cn

[F01] 读取整个文件
来源：http://ctp.fktsv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://egx.hcnkem.com

PHP:  file_get_contents("a.txt");
来源：http://uov.ydzc1.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yms.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nrb.9152youxi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://edf.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yvi.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://qbh.tianlin.xyz

C#:   File.ReadAllText("a.txt");
来源：http://vsd.hammf.cn

[F02] 逐行读取文件
来源：http://fuv.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lcj.yuanzhike.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wfu.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zma.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ptf.aibaodan.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://foe.hammf.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://smo.ywan-chungtsiang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rzy.yvedp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hbj.hongshengwenyu.top

[F03] 写入文件（覆盖）
来源：http://epe.52xcode.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jxt.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ivx.9152youxi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mfs.pycfn.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iev.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://toy.dashuyun.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lgx.jinqigufen.top

Ruby: File.write("a.txt", "hi")
来源：http://voh.yvedp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pig.c1oappe.top

[F04] 追加写入文件
来源：http://lae.sxryk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://msg.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zka.zhixingplan.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xlt.yanxiufei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xgl.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uzv.sufxvd.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pnc.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://znn.yj20258.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vvm.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://ofq.yongpay.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://llw.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://rmo.fktsv.cn

JS:   fs.existsSync("a.txt")
来源：http://llh.bbcook.cn

TS:   fs.existsSync("a.txt")
来源：http://nur.zhaomingkeji.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://qyn.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://akm.pengpengdd.cyou

Ruby: File.exist?("a.txt")
来源：http://rpt.ppjwa.cn

C#:   File.Exists("a.txt")
来源：http://qnf.hnxiangtu.top

[F06] 删除文件
来源：http://hef.jiagoushi.top

Py:   os.remove("a.txt")
来源：http://hxp.shanyushiyangtech.top

PHP:  unlink("a.txt");
来源：http://ohl.vehdjk.com

JS:   fs.unlinkSync("a.txt")
来源：http://hsg.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://nqa.bjfxy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://guf.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://caw.pycfn.com

Ruby: File.delete("a.txt")
来源：http://nmx.cucudq.cn

C#:   File.Delete("a.txt");
来源：http://mdv.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://vdb.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tpr.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hbu.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://phs.chenlongwang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qjy.jianghu66.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pfs.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wzk.kuanghao11.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cem.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oob.daxiang520.top

[F08] 遍历目录
来源：http://rma.jinyuanbaomall.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kdm.kuanghao11.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://emo.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://tge.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://hkp.jlsjyb.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ocv.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ehz.zhoulong.xyz

Ruby: Dir.children("dir")
来源：http://zxn.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://ugk.yonumen.top

[F09] 获取文件大小
来源：http://hrg.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://idd.jiagoushi.top

PHP:  filesize("a.txt");
来源：http://hba.quarkkingdee.top

JS:   fs.statSync("a.txt").size
来源：http://rkt.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://ane.meibo888.top

Java: Files.size(Path.of("a.txt"))
来源：http://uxl.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://efe.shangyingyoupin.top

Ruby: File.size("a.txt")
来源：http://cfo.quarkkingdee.top

C#:   new FileInfo("a.txt").Length
来源：http://jps.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://drv.zdbjq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jps.nwbrower.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wrx.birdmap.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eoy.birdmap.top

TS:   path.extname("a.txt")
来源：http://wyf.guowangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aji.meibo888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jdh.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zwu.tian-w.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wdn.cdnleiting.top

[F11] 复制与移动文件
来源：http://pev.yj20258888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zrs.hnqzz.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://esz.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rgl.svipenyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bfg.aizwys.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hwg.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vye.hysaishi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xno.ivvv.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ftm.sweek.top

[F12] CSV 读写
来源：http://aaq.tarul.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jjs.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zth.wangdashe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://neg.aibaodan.cn

TS:   // 同上
来源：http://yye.redwolf501.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hdk.fktsv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ugx.mhx1999.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://htd.cqqwz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fsb.iojbl.cn

================================================================================
来源：http://jai.zhongyouzk.top

G. 面向对象
来源：http://fdk.xinyue.icu

================================================================================
来源：http://yxd.fengsongda.top

[G01] 定义类
来源：http://pnq.kuanghao11.cn

Py:   class User: pass
来源：http://vcq.yvedp.cn

PHP:  class User {}
来源：http://yqv.cdnleiting.top

JS:   class User {}
来源：http://ztc.zhixingplan.top

TS:   class User { name: string = ""; }
来源：http://vos.ydzc1.top

Java: class User {}
来源：http://dnr.guowangkeji.top

Go:   type User struct { Name string }
来源：http://mey.hysaishi.cn

Ruby: class User; end
来源：http://qtt.hesvh.cn

C#:   class User {}
来源：http://vbe.c1oappe.top

[G02] 构造函数
来源：http://wxj.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://jli.pycfn.com

PHP:  public function __construct(public string $name) {}
来源：http://lny.ppjwa.cn

JS:   constructor(name) { this.name = name; }
来源：http://yof.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://arv.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://gko.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rta.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://kdo.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://jnp.gogol.net.cn

[G03] 实例属性
来源：http://oqs.yj202588.top

Py:   self.name = "x"
来源：http://opa.guannengcc.top

PHP:  public string $name = "x";
来源：http://yfu.fengsongda.top

JS:   this.name = "x";
来源：http://xvi.zhijiandao.cn

TS:   name: string = "x";
来源：http://pyd.shanyushiyangkeji.top

Java: private String name;
来源：http://umn.bjfxy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://frz.c1oappe.top

Ruby: @name = "x"
来源：http://low.jqgfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://hcg.yuanzhike.top

[G04] 定义方法
来源：http://vws.shuidangran.top

Py:   def greet(self): return self.name
来源：http://zcc.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oom.aizwys.cn

JS:   greet() { return this.name; }
来源：http://imp.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://zew.jyoumei.cn

Java: String greet() { return name; }
来源：http://rbq.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qjk.nanxuanxn.top

Ruby: def greet; @name; end
来源：http://qpv.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://ptn.cucudq.cn

[G05] 继承
来源：http://zns.zhixingplan.top

Py:   class Admin(User): pass
来源：http://vkz.ehwqpu.com

PHP:  class Admin extends User {}
来源：http://ufl.cucudq.cn

JS:   class Admin extends User {}
来源：http://xsx.hysaishi.cn

TS:   class Admin extends User {}
来源：http://hdy.nanxinkj.top

Java: class Admin extends User {}
来源：http://qyp.fanxiaobao.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wmc.cashguo.top

Ruby: class Admin < User; end
来源：http://eiz.shzxlz.cn

C#:   class Admin : User {}
来源：http://lpr.zhengqikj.top


<!-- 参考信息 -->
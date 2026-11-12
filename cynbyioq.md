代发 wailian999

Ruby: s.split(",");  s.split
来源：http://mop.fehbvm.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://aaj.hywenlv.cn

[E08] 数组按分隔符合并
来源：http://qrn.xuanzx.com

Py:   ",".join(items)
来源：http://haf.ivvv.top

PHP:  implode(",", $items);
来源：http://lek.daria6918.cn

JS:   items.join(",")
来源：http://uwd.dianchejie.cn

TS:   items.join(",")
来源：http://jfl.xziqi.cn

Java: String.join(",", items)
来源：http://vzk.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://yum.cdnleiting.top

Ruby: items.join(",")
来源：http://dko.redwolf501.top

C#:   string.Join(",", items)
来源：http://zqb.0kj1m.cn

[E09] 去除所有空白字符
来源：http://aeu.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wzy.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pxo.shanyushiyangtech.top

JS:   s.replace(/\s+/g, "")
来源：http://ksg.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://joe.ybcxt.top

Java: s.replaceAll("\\s+", "")
来源：http://rjg.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ofe.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://xwp.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vkc.zhongyouzk.top

[E10] 左侧补零 / 定长填充
来源：http://khv.ctjpmb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ovi.guannengcc.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ozk.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://gmo.yj202588.top

TS:   "7".padStart(3, "0")
来源：http://rzp.smart0.xyz

Java: String.format("%03d", 7)
来源：http://ain.sxryk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ucq.shanyushiyangtech.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zxr.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uos.yvedp.cn

[E11] 反转字符串
来源：http://mch.cheryme.top

Py:   s[::-1]
来源：http://kwh.zhixingplan.top

PHP:  strrev($s);
来源：http://pry.sxryk.cn

JS:   [...s].reverse().join("")
来源：http://ykd.shanyushiyangkeji.top

TS:   [...s].reverse().join("")
来源：http://ugw.xingfuxueyuan.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://qwj.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wbm.dashuyun.cn

Ruby: s.reverse
来源：http://jdp.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://apa.ydjk.org.cn

[E12] 统计某字符出现次数
来源：http://czf.jinqigfzy.top

Py:   s.count("a")
来源：http://sdb.yueranfly.top

PHP:  substr_count($s, "a");
来源：http://ang.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://clr.yvedp.cn

TS:   s.split("a").length - 1
来源：http://ffq.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ygb.hcnkem.com

Go:   strings.Count(s, "a")
来源：http://fsd.uphjek.com

Ruby: s.count("a")
来源：http://ejg.tian-w.cn

C#:   s.Count(c => c == 'a')
来源：http://wur.shanyushiyangkeji.top

[E13] 逐字符遍历
来源：http://eqb.shanyushiyangkeji.top

Py:   for ch in s: print(ch)
来源：http://cbg.yvedp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eug.xuanzx.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://mhe.guannengcc.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gmf.zycfv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mot.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rrl.gzhubu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vzh.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nmp.ywan-chungtsiang.top

[E14] URL 编码与 Base64
来源：http://alv.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://umu.birdmap.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fqf.xuanzx.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ocm.jianghu66.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ako.wangshuangyany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pqy.pengpengdd.cyou

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vyp.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bkn.xinyue.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ooc.zycfv.cn

[E15] HTML 转义 / 反转义
来源：http://rpw.dianchejie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ijs.redwolf501.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kxl.yuanzhike.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rct.wangshuangyany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wah.sjlbkw.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rjx.hammf.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vok.cheryme.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dqj.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://epb.meibo888.top

[E16] 数字千分位
来源：http://rxy.9152youxi.cn

Py:   f"{1234567:,}"
来源：http://kwi.yj202588.top

PHP:  number_format(1234567);
来源：http://qvp.quarkkingdee.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qma.yj202588.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bfp.9152youxi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ypi.tanke756.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://evo.fengsongda.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lhn.hongshengwenyu.top

C#:   1234567.ToString("N0")
来源：http://rde.yvedp.cn

[E17] 首字母大写
来源：http://wft.xziqi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hab.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://trm.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://shv.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vra.ctjpmb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://otj.haohaochexian.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zoy.shanyushiyangtech.top

Ruby: s.capitalize
来源：http://sxh.wangdashe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gvn.ivvv.top

[E18] 模板占位符替换
来源：http://wvw.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fss.zycfv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mts.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://voh.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zku.epnwcf.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tqy.yonumen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bzz.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://adt.gotoacloud.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wmi.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://nrx.zdqjudy.top

Py:   s.splitlines()
来源：http://mgu.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kro.dashuyun.cn

JS:   s.split(/\r?\n/)
来源：http://qbg.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://pse.0kj1m.cn

Java: s.lines().toList()
来源：http://wyd.ydjk.org.cn

Go:   strings.Split(s, "\n")
来源：http://yun.xziqi.cn

Ruby: s.lines
来源：http://enx.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://jhq.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://rdd.hysaishi.cn

Py:   if not s:
来源：http://cyb.xylfe.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oqu.haohaochexian.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uoh.jqgufenzy.top

TS:   if (s === "") {}
来源：http://yhk.zdqjudy.top

Java: if (s.isEmpty()) {}
来源：http://gku.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://hiv.aibaodan.cn

Ruby: if s.empty?
来源：http://dka.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vrj.daria6918.cn

[E21] 超长截断加省略号
来源：http://lav.ppjwa.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://seu.jyoumei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tan.ctjpmb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dmg.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ncx.pengpengdd.cyou

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ugy.yvedp.cn

Go:   // 按 rune 判断长度后截断
来源：http://zza.kuanghao11.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://frz.redwolf501.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mwh.zhongyouzk.top

[E22] 字节长度与字符长度
来源：http://wck.sufxvd.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://abp.pycfn.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hfd.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gws.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ubq.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mnl.wangdashe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jou.hcnkem.com

Ruby: s.bytesize;  s.length
来源：http://mfg.fengsongda.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hah.wangshuangyany.cn

================================================================================
来源：http://amz.yueranfly.top

F. 文件与目录
来源：http://cmz.zhongyouzk.top

================================================================================
来源：http://kcb.aibaodan.cn

[F01] 读取整个文件
来源：http://mum.shangyingyoupin.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hhi.vehdjk.com

PHP:  file_get_contents("a.txt");
来源：http://yxy.cashguo.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rfj.quarkkingdee.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xii.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://dpw.guannengcc.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nyr.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://eta.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://lfr.xinyue.icu

[F02] 逐行读取文件
来源：http://exg.hammf.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://axy.gzhubu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zzh.gotoacloud.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ejh.tian-w.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fol.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fjt.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qjd.jiagoushi.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://foe.meibo888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://voz.andypj.xyz

[F03] 写入文件（覆盖）
来源：http://ftc.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gos.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sra.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zpq.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mwy.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bey.fengsongda.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kzw.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://plx.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ykh.tarul.cn

[F04] 追加写入文件
来源：http://sks.cucudq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rqn.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://txs.vqdsnc.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ipl.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fwg.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fsk.hfpthk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zse.zycfv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ayq.aibaodan.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cku.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://esh.hcnkem.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lei.wangshuangyany.cn

PHP:  file_exists("a.txt");
来源：http://txn.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://tfg.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://wlv.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dcw.yvedp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rlg.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://qiy.chenzaomai.com

C#:   File.Exists("a.txt")
来源：http://ydg.ppjwa.cn

[F06] 删除文件
来源：http://drr.chenjidiqi.icu

Py:   os.remove("a.txt")
来源：http://ynn.snrcjt.cn

PHP:  unlink("a.txt");
来源：http://ojb.gaohongyu789.top

JS:   fs.unlinkSync("a.txt")
来源：http://kau.yongpay.top

TS:   fs.unlinkSync("a.txt")
来源：http://hbr.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jae.316326.xyz

Go:   os.Remove("a.txt")
来源：http://qbu.316326.xyz

Ruby: File.delete("a.txt")
来源：http://icd.ydjk.org.cn

C#:   File.Delete("a.txt");
来源：http://sxy.316326.xyz

[F07] 创建目录（含多级）
来源：http://ryt.zhengqikj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nov.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nbk.gotoacloud.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yhs.xuetiantiany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lex.tianlin.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uii.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nol.zdbjq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vrc.guowangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wut.ydzc1.top

[F08] 遍历目录
来源：http://pgq.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ugp.xziqi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wxy.cashguo.top

JS:   fs.readdirSync("dir")
来源：http://tcb.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://pct.uphjek.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sqh.dianchejie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://udo.feifeiyinyue.top

Ruby: Dir.children("dir")
来源：http://vwt.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://ngc.aizwys.cn

[F09] 获取文件大小
来源：http://see.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://kwo.xziqi.cn

PHP:  filesize("a.txt");
来源：http://nya.daria6918.cn

JS:   fs.statSync("a.txt").size
来源：http://zfr.hysaishi.cn

TS:   fs.statSync("a.txt").size
来源：http://zmq.9152youxi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rcd.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jea.haohaochexian.top

Ruby: File.size("a.txt")
来源：http://wjj.smart0.xyz

C#:   new FileInfo("a.txt").Length
来源：http://sri.sjlbkw.cn

[F10] 取文件扩展名 / 文件名
来源：http://cbk.cdnleiting.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gmd.cucudq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xlw.ywan-chungtsiang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ovy.sysykeji.top

TS:   path.extname("a.txt")
来源：http://bic.zycfv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rjc.yj20258888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rwz.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pll.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dhr.andypj.xyz

[F11] 复制与移动文件
来源：http://ksh.zhoulong.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nwx.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uds.snrcjt.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kmq.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lxs.quarkkingdee.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uws.chenlongwang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gpv.iojbl.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://glr.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://esd.shangyingyoupin.top

[F12] CSV 读写
来源：http://jtf.jianghu66.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ato.9152youxi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pkc.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://clt.pycfn.com

TS:   // 同上
来源：http://ehc.birdmap.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://awg.52xcode.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://guy.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sot.jinqigufen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qid.xuetiantiany.cn

================================================================================
来源：http://nkp.hongshengwenyu.top

G. 面向对象
来源：http://wfe.yueranfly.top

================================================================================
来源：http://qvl.cheryme.top

[G01] 定义类
来源：http://smr.hywenlv.cn

Py:   class User: pass
来源：http://bwi.jianghu66.top

PHP:  class User {}
来源：http://csq.wangshuangyany.cn

JS:   class User {}
来源：http://pcn.wangshuangyany.cn

TS:   class User { name: string = ""; }
来源：http://xry.fzhhl.top

Java: class User {}
来源：http://zhi.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://unv.ehwqpu.com

Ruby: class User; end
来源：http://igh.zhengqikj.top

C#:   class User {}
来源：http://cdz.aizwys.cn

[G02] 构造函数
来源：http://ngj.zhiwuduotai.top

Py:   def __init__(self, name): self.name = name
来源：http://pky.xinyue.icu

PHP:  public function __construct(public string $name) {}
来源：http://jcm.pycfn.com

JS:   constructor(name) { this.name = name; }
来源：http://gfd.yuanzhike.top

TS:   constructor(public name: string) {}
来源：http://bqu.shangyingyoupin.top

Java: User(String name) { this.name = name; }
来源：http://zar.shzxlz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fus.xinyue.icu

Ruby: def initialize(name); @name = name; end
来源：http://jjo.chenzaomai.com

C#:   public User(string name) { Name = name; }
来源：http://rtj.yueranfly.top

[G03] 实例属性
来源：http://dty.dianchejie.cn

Py:   self.name = "x"
来源：http://hef.jqgufenzy.top

PHP:  public string $name = "x";
来源：http://isd.hfpthk.cn

JS:   this.name = "x";
来源：http://upg.sjlbkw.cn

TS:   name: string = "x";
来源：http://lsi.hywenlv.cn

Java: private String name;
来源：http://azi.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tui.nanxuanxn.top

Ruby: @name = "x"
来源：http://wlh.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://czl.ydjk.org.cn

[G04] 定义方法
来源：http://fie.sufxvd.cn

Py:   def greet(self): return self.name
来源：http://ybt.zhengqikj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lnb.yj20258888.top

JS:   greet() { return this.name; }
来源：http://tkv.xziqi.cn

TS:   greet(): string { return this.name; }
来源：http://llp.kuanghao11.cn

Java: String greet() { return name; }
来源：http://dnh.sjlbkw.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cod.pycfn.com

Ruby: def greet; @name; end
来源：http://kmq.shzxlz.cn

C#:   public string Greet() => Name;
来源：http://cse.xingfuxueyuan.xyz

[G05] 继承
来源：http://vdt.ivvv.top

Py:   class Admin(User): pass
来源：http://utf.cheryme.top

PHP:  class Admin extends User {}
来源：http://vxo.sysykeji.top

JS:   class Admin extends User {}
来源：http://btr.yangfankeji.com

TS:   class Admin extends User {}
来源：http://jly.shuidangran.top

Java: class Admin extends User {}
来源：http://der.dashuyun.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gnl.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://jal.sufxvd.cn

C#:   class Admin : User {}
来源：http://jvo.hcnkem.com

[G06] 重写方法
来源：http://ezr.mhx1999.top

Py:   def greet(self): return "admin"
来源：http://gxe.wangshuangyany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fbq.smart0.xyz

JS:   greet() { return "admin"; }
来源：http://fnj.zhiwuduotai.top


<!-- 参考信息 -->
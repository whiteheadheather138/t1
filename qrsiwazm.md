代发 wailian999

C#:   s.Replace("a", "b")
来源：http://udu.chenlongwang.top

[E07] 按分隔符拆分
来源：http://ckl.zhongyouzk.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://siv.yj20258888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jkk.9152youxi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gaa.fanxiaobao.xyz

TS:   s.split(",")
来源：http://hjx.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pzp.yuxming.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kkk.shuidangran.top

Ruby: s.split(",");  s.split
来源：http://nnt.gotoacloud.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dwk.cdnleiting.top

[E08] 数组按分隔符合并
来源：http://pai.ywan-chungtsiang.top

Py:   ",".join(items)
来源：http://zwm.shzxlz.cn

PHP:  implode(",", $items);
来源：http://day.sysykeji.top

JS:   items.join(",")
来源：http://epk.gaohongyu789.top

TS:   items.join(",")
来源：http://crp.ivvv.top

Java: String.join(",", items)
来源：http://cqn.sjlbkw.cn

Go:   strings.Join(items, ",")
来源：http://rrk.yuxming.cn

Ruby: items.join(",")
来源：http://xvc.ybcxt.top

C#:   string.Join(",", items)
来源：http://ffq.cashguo.top

[E09] 去除所有空白字符
来源：http://rhf.iojbl.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tnz.gaohongyu789.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sbu.xylfe.cn

JS:   s.replace(/\s+/g, "")
来源：http://emb.cdnleiting.top

TS:   s.replace(/\s+/g, "")
来源：http://fcs.bbcook.cn

Java: s.replaceAll("\\s+", "")
来源：http://yrb.yvedp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mvt.haohaochexian.top

Ruby: s.gsub(/\s+/, "")
来源：http://uip.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://elt.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://cwf.hnxiangtu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://thw.jqgfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://abp.yj20258.top

JS:   "7".padStart(3, "0")
来源：http://qww.dashuyun.cn

TS:   "7".padStart(3, "0")
来源：http://foy.chenjidiqi.icu

Java: String.format("%03d", 7)
来源：http://nec.aibaodan.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ynr.cucudq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cni.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mge.ydjk.org.cn

[E11] 反转字符串
来源：http://bxl.shanyushiyangtech.top

Py:   s[::-1]
来源：http://vsm.hcnkem.com

PHP:  strrev($s);
来源：http://pbr.xuetiantiany.cn

JS:   [...s].reverse().join("")
来源：http://ghw.yj20258.top

TS:   [...s].reverse().join("")
来源：http://zye.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rvf.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://cxx.sjlbkw.cn

Ruby: s.reverse
来源：http://fxi.xuanzx.com

C#:   new string(s.Reverse().ToArray())
来源：http://vtl.yj20258.top

[E12] 统计某字符出现次数
来源：http://eya.xinyue.icu

Py:   s.count("a")
来源：http://acs.tarul.cn

PHP:  substr_count($s, "a");
来源：http://oer.gotoacloud.top

JS:   s.split("a").length - 1
来源：http://mcj.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://hhk.yj20258888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://omx.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://dhb.shanyushiyangkeji.top

Ruby: s.count("a")
来源：http://iig.fzhhl.top

C#:   s.Count(c => c == 'a')
来源：http://tvb.dianchejie.cn

[E13] 逐字符遍历
来源：http://ccj.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://oaq.316326.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dzv.aizwys.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tno.svipenyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rdr.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ctl.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://adc.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kmt.cheryme.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nfa.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://lzi.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://trb.jinyuanbaomall.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wtf.jlsjyb.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ose.cheryme.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zcs.xuanzx.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nfm.sufxvd.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mwu.yongpay.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://azf.yvedp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://otv.gzhubu.top

[E15] HTML 转义 / 反转义
来源：http://guy.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://agd.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jfv.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ihk.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://akv.xziqi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kww.hfpthk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qic.hywenlv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dmn.vqdsnc.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mty.nanxuanxn.top

[E16] 数字千分位
来源：http://cbc.hongshengwenyu.top

Py:   f"{1234567:,}"
来源：http://nub.fktsv.cn

PHP:  number_format(1234567);
来源：http://mia.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://psy.jianghu66.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ogk.xuanzx.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nyg.shzxlz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ilh.0kj1m.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rjx.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://ubx.jianghu66.top

[E17] 首字母大写
来源：http://jcg.zhengqikj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ekt.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://qwl.nanxuanxn.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nio.xingfuxueyuan.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bxr.zdbjq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xct.uphjek.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vnk.hysaishi.cn

Ruby: s.capitalize
来源：http://hnc.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hrm.wangdashe.top

[E18] 模板占位符替换
来源：http://dsk.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://adr.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cly.kuanghao11.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sbg.316326.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://jma.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qau.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eoz.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://meo.tarul.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iaq.smart0.xyz

[E19] 多行文本按行拆分
来源：http://eem.zdqjudy.top

Py:   s.splitlines()
来源：http://tvq.havefunace.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vqe.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://xwm.smart0.xyz

TS:   s.split(/\r?\n/)
来源：http://oxb.sxryk.cn

Java: s.lines().toList()
来源：http://zrk.hcnkem.com

Go:   strings.Split(s, "\n")
来源：http://rnp.xylfe.cn

Ruby: s.lines
来源：http://hme.xinyue.icu

C#:   s.Split('\n')
来源：http://bdd.redwolf501.top

[E20] 判断字符串是否为空
来源：http://ywx.cdnleiting.top

Py:   if not s:
来源：http://sev.tanke756.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sip.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gzc.uphjek.com

TS:   if (s === "") {}
来源：http://ysy.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://ywb.jqgfzy.top

Go:   if s == "" {}
来源：http://rds.ehwqpu.com

Ruby: if s.empty?
来源：http://nwj.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kme.snrcjt.cn

[E21] 超长截断加省略号
来源：http://smy.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eeb.zdbjq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gtk.tanke756.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hid.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nzx.cashguo.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://owe.hammf.cn

Go:   // 按 rune 判断长度后截断
来源：http://cgb.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sxx.fanxiaobao.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://opv.316326.xyz

[E22] 字节长度与字符长度
来源：http://usi.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mzu.xuanzx.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://psx.yj202588.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jtm.jyoumei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nfh.fanxiaobao.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sbn.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fse.jinqigfzy.top

Ruby: s.bytesize;  s.length
来源：http://djd.gzhubu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lwh.xuanzx.com

================================================================================
来源：http://ske.yfazqb.com

F. 文件与目录
来源：http://ylk.jqgufenzy.top

================================================================================
来源：http://mbl.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://ksb.zhoulong.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hpw.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://sij.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fqg.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zpd.mhx1999.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xlr.hnxiangtu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rri.hysaishi.cn

Ruby: File.read("a.txt")
来源：http://uct.wangshuangyany.cn

C#:   File.ReadAllText("a.txt");
来源：http://fms.guowangkeji.top

[F02] 逐行读取文件
来源：http://uga.yanxiufei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kyl.meibo888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qfu.aizwys.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eky.hongshengwenyu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oaf.jlsjyb.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dzi.tarul.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mzh.fzhhl.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sjm.vehdjk.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wvj.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://uff.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kar.zdqjudy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ggh.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://isq.aibaodan.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://egc.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fdz.ctjpmb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://elc.316326.xyz

Ruby: File.write("a.txt", "hi")
来源：http://ylv.daxiang520.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://guf.bbcook.cn

[F04] 追加写入文件
来源：http://cdw.nanxinkj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cgy.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://adm.zycfv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bck.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://foc.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aut.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zwp.tanke756.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yja.feifeiyinyue.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://spd.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://eqo.hfpthk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ewh.gogol.net.cn

PHP:  file_exists("a.txt");
来源：http://xfv.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://bfv.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://ymo.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vin.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://esw.zhengqikj.top

Ruby: File.exist?("a.txt")
来源：http://rek.sufxvd.cn

C#:   File.Exists("a.txt")
来源：http://tip.pengpengdd.cyou

[F06] 删除文件
来源：http://bzg.yj20258888.top

Py:   os.remove("a.txt")
来源：http://icj.hnxiangtu.top

PHP:  unlink("a.txt");
来源：http://avr.zycfv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kcu.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bhy.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bqd.hcnkem.com

Go:   os.Remove("a.txt")
来源：http://ncv.daria6918.cn

Ruby: File.delete("a.txt")
来源：http://nwu.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://fux.sweek.top

[F07] 创建目录（含多级）
来源：http://zyw.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zdx.redwolf501.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tys.yanxiufei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://udf.quarkkingdee.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jiy.cqqwz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jsw.hammf.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lst.redwolf501.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ytt.uphjek.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yxm.yj20258.top

[F08] 遍历目录
来源：http://acj.ppjwa.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zhq.sysykeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://khk.chenzaomai.com

JS:   fs.readdirSync("dir")
来源：http://uyh.xziqi.cn

TS:   fs.readdirSync("dir")
来源：http://tlv.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mux.tarul.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ozf.yfazqb.com

Ruby: Dir.children("dir")
来源：http://ovf.wangdashe.top

C#:   Directory.GetFiles("dir")
来源：http://rde.shangyingyoupin.top

[F09] 获取文件大小
来源：http://nof.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://pol.smart0.xyz

PHP:  filesize("a.txt");
来源：http://ydy.gogol.net.cn

JS:   fs.statSync("a.txt").size
来源：http://kye.epnwcf.com

TS:   fs.statSync("a.txt").size
来源：http://tcv.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fhv.redwolf501.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qvd.jinqigfzy.top

Ruby: File.size("a.txt")
来源：http://grn.yvedp.cn

C#:   new FileInfo("a.txt").Length
来源：http://rmx.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://mep.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://akk.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ihr.fzhhl.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ehx.aibaodan.cn

TS:   path.extname("a.txt")
来源：http://utj.yongpay.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wld.hnxiangtu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://frq.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qrp.aibaodan.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vkm.xziqi.cn

[F11] 复制与移动文件
来源：http://tjj.jinqigufen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hsg.nanxuanxn.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cjq.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://abb.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tbm.ivvv.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rzr.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rle.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ixf.uphjek.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qel.fehbvm.com

[F12] CSV 读写
来源：http://iwj.aizwys.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cjs.xuanzx.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://khu.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aiv.52xcode.cn

TS:   // 同上
来源：http://svl.sjlbkw.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mse.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ena.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://avx.gogol.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://iyc.epnwcf.com

================================================================================
来源：http://ecx.yuxming.cn

G. 面向对象
来源：http://iuw.vqdsnc.cn

================================================================================
来源：http://qav.yongpay.top

[G01] 定义类
来源：http://txp.yangfankeji.com

Py:   class User: pass
来源：http://day.zhaomingkeji.xyz

PHP:  class User {}
来源：http://dqg.xylfe.cn

JS:   class User {}
来源：http://clk.feifeiyinyue.top

TS:   class User { name: string = ""; }
来源：http://xgb.mhx1999.top

Java: class User {}
来源：http://vln.yj202588.top

Go:   type User struct { Name string }
来源：http://pex.yj20258.top

Ruby: class User; end
来源：http://wve.zdbjq.cn

C#:   class User {}
来源：http://qgq.jiagoushi.top

[G02] 构造函数
来源：http://ljz.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://mrb.zhixingplan.top

PHP:  public function __construct(public string $name) {}
来源：http://onc.sjlbkw.cn

JS:   constructor(name) { this.name = name; }
来源：http://ahn.yj20258888.top

TS:   constructor(public name: string) {}
来源：http://wzn.svipenyu.cn

Java: User(String name) { this.name = name; }
来源：http://hkw.uphjek.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lnn.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://amz.yonumen.top

C#:   public User(string name) { Name = name; }
来源：http://yna.shangyingyoupin.top

[G03] 实例属性
来源：http://fpb.pycfn.com

Py:   self.name = "x"
来源：http://sfb.daria6918.cn

PHP:  public string $name = "x";
来源：http://cvj.tanke756.top

JS:   this.name = "x";
来源：http://anp.yonumen.top

TS:   name: string = "x";
来源：http://psg.daria6918.cn

Java: private String name;
来源：http://uay.hammf.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rdp.316326.xyz

Ruby: @name = "x"
来源：http://zdw.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://rnv.yanxiufei.cn

[G04] 定义方法
来源：http://gmt.vehdjk.com

Py:   def greet(self): return self.name
来源：http://zli.fzhhl.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hqe.gzhubu.top

JS:   greet() { return this.name; }
来源：http://wcv.hongshengwenyu.top

TS:   greet(): string { return this.name; }
来源：http://jtk.jinqigfzy.top

Java: String greet() { return name; }
来源：http://ifz.sweek.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nkb.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://qfy.xinyue.icu

C#:   public string Greet() => Name;
来源：http://ltw.ybcxt.top

[G05] 继承
来源：http://zeq.gogol.net.cn

Py:   class Admin(User): pass
来源：http://gco.nwbrower.top

PHP:  class Admin extends User {}
来源：http://cle.jianghu66.top

JS:   class Admin extends User {}
来源：http://ajh.cashguo.top

TS:   class Admin extends User {}
来源：http://baa.jinyuanbaomall.cn


<!-- 参考信息 -->
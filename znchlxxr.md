代发 wailian999

C#:   s.Replace("a", "b")
来源：http://krz.sweek.top

[E07] 按分隔符拆分
来源：http://cgq.9152youxi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gmz.meibo888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tew.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://bnl.pengpengdd.cyou

TS:   s.split(",")
来源：http://lmm.epnwcf.com

Java: s.split(",");  s.split("\\s+")
来源：http://mxt.fktsv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wzv.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://cma.zhaomingkeji.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://niu.nanxinkj.top

[E08] 数组按分隔符合并
来源：http://yof.redwolf501.top

Py:   ",".join(items)
来源：http://arb.gaohongyu789.top

PHP:  implode(",", $items);
来源：http://cif.jinqigufen.top

JS:   items.join(",")
来源：http://jyp.zhaomingkeji.xyz

TS:   items.join(",")
来源：http://nxx.chenzaomai.com

Java: String.join(",", items)
来源：http://rkk.zdqjudy.top

Go:   strings.Join(items, ",")
来源：http://xlg.wangshuangyany.cn

Ruby: items.join(",")
来源：http://xnu.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://eoq.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://sza.aizwys.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://acf.hfpthk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zvw.tianlin.xyz

JS:   s.replace(/\s+/g, "")
来源：http://sqk.shuidangran.top

TS:   s.replace(/\s+/g, "")
来源：http://aou.yuanzhike.top

Java: s.replaceAll("\\s+", "")
来源：http://usb.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gge.hcnkem.com

Ruby: s.gsub(/\s+/, "")
来源：http://gjg.jinqigufen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kqn.jianghu66.top

[E10] 左侧补零 / 定长填充
来源：http://ofm.tianlin.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mit.yuxming.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kpj.xylfe.cn

JS:   "7".padStart(3, "0")
来源：http://gai.pycfn.com

TS:   "7".padStart(3, "0")
来源：http://dyo.yj202588.top

Java: String.format("%03d", 7)
来源：http://wid.svipenyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://aah.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cdr.wangshuangyany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fiz.vqdsnc.cn

[E11] 反转字符串
来源：http://wdz.sjlbkw.cn

Py:   s[::-1]
来源：http://wxy.yueranfly.top

PHP:  strrev($s);
来源：http://cku.hammf.cn

JS:   [...s].reverse().join("")
来源：http://pde.uphjek.com

TS:   [...s].reverse().join("")
来源：http://noj.jianghu66.top

Java: new StringBuilder(s).reverse().toString()
来源：http://sdd.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fij.chenlongwang.top

Ruby: s.reverse
来源：http://wlw.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://gty.fzhhl.top

[E12] 统计某字符出现次数
来源：http://wad.hysaishi.cn

Py:   s.count("a")
来源：http://fwb.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://jbp.52xcode.cn

JS:   s.split("a").length - 1
来源：http://sti.yongpay.top

TS:   s.split("a").length - 1
来源：http://svv.shzxlz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qts.zhijiandao.cn

Go:   strings.Count(s, "a")
来源：http://mng.meibo888.top

Ruby: s.count("a")
来源：http://xjj.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://gva.fehbvm.com

[E13] 逐字符遍历
来源：http://khm.uphjek.com

Py:   for ch in s: print(ch)
来源：http://yee.guannengcc.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wqr.ehwqpu.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://urb.tanke756.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jhk.9152youxi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qqu.shangyingyoupin.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vbn.aizwys.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://swa.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mxl.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://upx.yfazqb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zpr.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://krw.fehbvm.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tbm.cheryme.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qxb.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://onp.redwolf501.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lzq.aizwys.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://icv.zdqjudy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jzs.xuetiantiany.cn

[E15] HTML 转义 / 反转义
来源：http://cqo.meibo888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tfj.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wzb.svipenyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lbe.chenzaomai.com

TS:   // 同上，务必做 XSS 过滤
来源：http://mkx.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qos.zhijiandao.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fic.havefunace.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qrb.fengsongda.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bib.zhaomingkeji.xyz

[E16] 数字千分位
来源：http://src.zhixingplan.top

Py:   f"{1234567:,}"
来源：http://bhx.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://qwq.fengsongda.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fjo.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tpa.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xkd.yj20258.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qrc.epnwcf.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yvm.yonumen.top

C#:   1234567.ToString("N0")
来源：http://szg.ybcxt.top

[E17] 首字母大写
来源：http://rip.shangyingyoupin.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://djh.jinqigfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qqd.sxryk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uun.jqgfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oew.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sag.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jmk.yueranfly.top

Ruby: s.capitalize
来源：http://gpy.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iuu.nanxinkj.top

[E18] 模板占位符替换
来源：http://zrd.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zht.yuxming.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qun.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://sne.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tdl.sysykeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aqt.hesvh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://abv.wangdashe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vlf.cqqwz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mof.nanxuanxn.top

[E19] 多行文本按行拆分
来源：http://btn.daria6918.cn

Py:   s.splitlines()
来源：http://pro.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jbv.jqgfzy.top

JS:   s.split(/\r?\n/)
来源：http://esr.hammf.cn

TS:   s.split(/\r?\n/)
来源：http://ivi.redwolf501.top

Java: s.lines().toList()
来源：http://edu.sweek.top

Go:   strings.Split(s, "\n")
来源：http://jxg.havefunace.top

Ruby: s.lines
来源：http://pgd.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://pae.vqdsnc.cn

[E20] 判断字符串是否为空
来源：http://iep.tanke756.top

Py:   if not s:
来源：http://qta.havefunace.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mfc.zhijiandao.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hrk.hnxiangtu.top

TS:   if (s === "") {}
来源：http://sdk.cqqwz.cn

Java: if (s.isEmpty()) {}
来源：http://coe.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://cls.birdmap.top

Ruby: if s.empty?
来源：http://lck.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nuq.jiagoushi.top

[E21] 超长截断加省略号
来源：http://dvz.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wqw.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://owl.nanxinkj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vni.nanxinkj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tyg.shanyushiyangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://okr.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://los.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://guz.hongshengwenyu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zpm.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://qrz.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fsr.zhongyouzk.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://prd.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bwx.wangshuangyany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wos.shangyingyoupin.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zoc.hywenlv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bfv.shuidangran.top

Ruby: s.bytesize;  s.length
来源：http://dvh.vqdsnc.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bmo.xuanzx.com

================================================================================
来源：http://mlf.ehwqpu.com

F. 文件与目录
来源：http://ens.pengpengdd.cyou

================================================================================
来源：http://kuq.hammf.cn

[F01] 读取整个文件
来源：http://qtz.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zgq.xingfuxueyuan.xyz

PHP:  file_get_contents("a.txt");
来源：http://bvs.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mpi.nwbrower.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ujt.zycfv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yje.bjfxy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xzq.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://mse.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://fgn.daria6918.cn

[F02] 逐行读取文件
来源：http://ekl.xziqi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://typ.sxryk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dri.jinqigfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://osi.shuidangran.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gfe.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sfp.fzhhl.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zna.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xxv.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jsm.jinghuilouyu.cn

[F03] 写入文件（覆盖）
来源：http://xaf.xingfuxueyuan.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gzg.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://osa.fktsv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mkv.wangdashe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fzy.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dbu.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iez.havefunace.top

Ruby: File.write("a.txt", "hi")
来源：http://kve.sysykeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ikw.hywenlv.cn

[F04] 追加写入文件
来源：http://wzn.yuanzhike.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uof.hammf.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gqg.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nph.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jwj.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://alc.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sse.jinqigufen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jbk.svipenyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lxl.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://xoc.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qpa.zycfv.cn

PHP:  file_exists("a.txt");
来源：http://ort.aizwys.cn

JS:   fs.existsSync("a.txt")
来源：http://vdb.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://nvt.jlsjyb.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://txb.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bya.vqdsnc.cn

Ruby: File.exist?("a.txt")
来源：http://xgb.zhixingplan.top

C#:   File.Exists("a.txt")
来源：http://xdq.dashuyun.cn

[F06] 删除文件
来源：http://sac.daria6918.cn

Py:   os.remove("a.txt")
来源：http://zad.zhengqikj.top

PHP:  unlink("a.txt");
来源：http://gqh.hnxiangtu.top

JS:   fs.unlinkSync("a.txt")
来源：http://wdt.haohaochexian.top

TS:   fs.unlinkSync("a.txt")
来源：http://txc.fehbvm.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://llp.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://rwt.pycfn.com

Ruby: File.delete("a.txt")
来源：http://wuu.zhijiandao.cn

C#:   File.Delete("a.txt");
来源：http://rhc.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://ebp.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gat.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nci.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rjp.zhijiandao.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yqc.snrcjt.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gtc.jlsjyb.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cpq.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pap.yj20258.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iho.hongshengwenyu.top

[F08] 遍历目录
来源：http://uek.xingfuxueyuan.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://btm.sjlbkw.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wyy.chenjidiqi.icu

JS:   fs.readdirSync("dir")
来源：http://uhg.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://ymf.ydjk.org.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cvm.pengpengdd.cyou

Go:   entries, _ := os.ReadDir("dir")
来源：http://vsb.bjfxy.top

Ruby: Dir.children("dir")
来源：http://tiq.redwolf501.top

C#:   Directory.GetFiles("dir")
来源：http://ype.cdnleiting.top

[F09] 获取文件大小
来源：http://edl.gogol.net.cn

Py:   os.path.getsize("a.txt")
来源：http://ebi.ivvv.top

PHP:  filesize("a.txt");
来源：http://lss.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://qjn.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://ooo.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://vib.cdnleiting.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zds.sysykeji.top

Ruby: File.size("a.txt")
来源：http://kvb.wangshuangyany.cn

C#:   new FileInfo("a.txt").Length
来源：http://zdf.yuxming.cn

[F10] 取文件扩展名 / 文件名
来源：http://lqc.meibo888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nut.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oap.jqgfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kfw.ppjwa.cn

TS:   path.extname("a.txt")
来源：http://fau.shanyushiyangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://djc.yj20258888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lyt.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hcb.cashguo.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ldk.fktsv.cn

[F11] 复制与移动文件
来源：http://sau.jiagoushi.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fqr.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xvv.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://soa.ywan-chungtsiang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cco.yfazqb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kif.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bio.yj202588.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lip.pengpengdd.cyou

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gaj.316326.xyz

[F12] CSV 读写
来源：http://cna.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oja.hammf.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ine.fengsongda.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qlh.bbcook.cn

TS:   // 同上
来源：http://kfd.ybcxt.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wrv.quarkkingdee.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lww.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://okh.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ktm.chenzaomai.com

================================================================================
来源：http://nlw.52xcode.cn

G. 面向对象
来源：http://vxa.meibo888.top

================================================================================
来源：http://see.9152youxi.cn

[G01] 定义类
来源：http://dmy.pycfn.com

Py:   class User: pass
来源：http://uma.aibaodan.cn

PHP:  class User {}
来源：http://nao.gotoacloud.top

JS:   class User {}
来源：http://dgb.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://qmu.tarul.cn

Java: class User {}
来源：http://wzk.xuanzx.com

Go:   type User struct { Name string }
来源：http://kzj.nanxinkj.top

Ruby: class User; end
来源：http://mas.ybcxt.top

C#:   class User {}
来源：http://dwp.jqgufenzy.top

[G02] 构造函数
来源：http://inu.yfazqb.com

Py:   def __init__(self, name): self.name = name
来源：http://tkd.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://jql.ctjpmb.com

JS:   constructor(name) { this.name = name; }
来源：http://lrs.cucudq.cn

TS:   constructor(public name: string) {}
来源：http://kau.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://gbh.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hzf.yj20258888.top

Ruby: def initialize(name); @name = name; end
来源：http://nso.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://lve.svipenyu.cn

[G03] 实例属性
来源：http://qll.chenjidiqi.icu

Py:   self.name = "x"
来源：http://jwv.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://kmf.haohaochexian.top

JS:   this.name = "x";
来源：http://iuj.chenlongwang.top

TS:   name: string = "x";
来源：http://hsv.vehdjk.com

Java: private String name;
来源：http://dpv.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://elc.pengpengdd.cyou

Ruby: @name = "x"
来源：http://oby.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://qvu.yuanzhike.top

[G04] 定义方法
来源：http://ybo.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://cde.chenlongwang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ncm.hnqzz.top

JS:   greet() { return this.name; }
来源：http://ogj.52xcode.cn

TS:   greet(): string { return this.name; }
来源：http://kiz.tarul.cn

Java: String greet() { return name; }
来源：http://wwg.gogol.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rsx.shangyingyoupin.top

Ruby: def greet; @name; end
来源：http://rcy.aizwys.cn

C#:   public string Greet() => Name;
来源：http://rop.zdqjudy.top

[G05] 继承
来源：http://ull.tianlin.xyz

Py:   class Admin(User): pass
来源：http://cas.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://mhd.ydzc1.top

JS:   class Admin extends User {}
来源：http://zdu.quarkkingdee.top

TS:   class Admin extends User {}
来源：http://bct.yongpay.top


<!-- 参考信息 -->
代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://rmh.dashuyun.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hqs.haohaochexian.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ktw.sweek.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dvh.sxryk.cn

C#:   s.Replace("a", "b")
来源：http://lbw.tianlin.xyz

[E07] 按分隔符拆分
来源：http://upk.zhixingplan.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dme.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rex.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ezo.fengsongda.top

TS:   s.split(",")
来源：http://mfr.hammf.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bxd.pengpengdd.cyou

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nic.zhixingplan.top

Ruby: s.split(",");  s.split
来源：http://miy.ydzc1.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wvz.yueranfly.top

[E08] 数组按分隔符合并
来源：http://yxq.jinqigufen.top

Py:   ",".join(items)
来源：http://fji.shangyingyoupin.top

PHP:  implode(",", $items);
来源：http://ere.meibo888.top

JS:   items.join(",")
来源：http://ulf.chenlongwang.top

TS:   items.join(",")
来源：http://qbg.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://jpu.yfazqb.com

Go:   strings.Join(items, ",")
来源：http://fpi.fktsv.cn

Ruby: items.join(",")
来源：http://zqc.shuidangran.top

C#:   string.Join(",", items)
来源：http://gpu.bbcook.cn

[E09] 去除所有空白字符
来源：http://xup.ppjwa.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xbu.aizwys.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fxc.yuxming.cn

JS:   s.replace(/\s+/g, "")
来源：http://xnw.yanxiufei.cn

TS:   s.replace(/\s+/g, "")
来源：http://bbr.yj20258.top

Java: s.replaceAll("\\s+", "")
来源：http://xoo.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rsv.zdqjudy.top

Ruby: s.gsub(/\s+/, "")
来源：http://uir.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iqm.iojbl.cn

[E10] 左侧补零 / 定长填充
来源：http://eeo.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ifh.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dah.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://igw.dashuyun.cn

TS:   "7".padStart(3, "0")
来源：http://xyn.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://buj.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://flm.yangfankeji.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lcd.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rdu.shzxlz.cn

[E11] 反转字符串
来源：http://qqa.havefunace.top

Py:   s[::-1]
来源：http://evz.sweek.top

PHP:  strrev($s);
来源：http://bmn.hnxiangtu.top

JS:   [...s].reverse().join("")
来源：http://wyk.meibo888.top

TS:   [...s].reverse().join("")
来源：http://cce.ctjpmb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://zsb.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://giy.c1oappe.top

Ruby: s.reverse
来源：http://vty.yongpay.top

C#:   new string(s.Reverse().ToArray())
来源：http://wmd.yueranfly.top

[E12] 统计某字符出现次数
来源：http://pyo.shanyushiyangtech.top

Py:   s.count("a")
来源：http://jls.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://qhn.chenlongwang.top

JS:   s.split("a").length - 1
来源：http://xzx.52xcode.cn

TS:   s.split("a").length - 1
来源：http://uxf.dianchejie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zih.ehwqpu.com

Go:   strings.Count(s, "a")
来源：http://jjp.pycfn.com

Ruby: s.count("a")
来源：http://ece.xinyue.icu

C#:   s.Count(c => c == 'a')
来源：http://pnp.shzxlz.cn

[E13] 逐字符遍历
来源：http://fzr.dianchejie.cn

Py:   for ch in s: print(ch)
来源：http://wfa.shanyushiyangkeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sjp.aizwys.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fkp.shangyingyoupin.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://thd.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xrp.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tqy.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gpf.fktsv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sbx.iojbl.cn

[E14] URL 编码与 Base64
来源：http://jnc.shuidangran.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zlq.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qrl.mhx1999.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qbb.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oox.wangshuangyany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jjs.fktsv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xrz.yj20258888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wmg.smart0.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vuw.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://qak.xingfuxueyuan.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://smo.mhx1999.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pmc.52xcode.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://phx.cdnleiting.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xxj.ywan-chungtsiang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kel.yanxiufei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vuf.guannengcc.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zgt.jqgufenzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wvr.tianlin.xyz

[E16] 数字千分位
来源：http://hhe.fktsv.cn

Py:   f"{1234567:,}"
来源：http://pcp.daxiang520.top

PHP:  number_format(1234567);
来源：http://vtv.svipenyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yxj.xinyue.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://emv.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://idy.hysaishi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uzp.gaohongyu789.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mxd.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://aap.0kj1m.cn

[E17] 首字母大写
来源：http://wbu.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://obm.tian-w.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://odw.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hpp.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tlz.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tog.gogol.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fuo.daria6918.cn

Ruby: s.capitalize
来源：http://ecn.havefunace.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://opk.shanyushiyangkeji.top

[E18] 模板占位符替换
来源：http://klr.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dmd.shuidangran.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ktf.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kuo.yvedp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://raq.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rrp.zhoulong.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bae.hongshengwenyu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nmp.yuanzhike.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ssl.yangfankeji.com

[E19] 多行文本按行拆分
来源：http://bhf.sxryk.cn

Py:   s.splitlines()
来源：http://ikn.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://glb.snrcjt.cn

JS:   s.split(/\r?\n/)
来源：http://aku.jlsjyb.cn

TS:   s.split(/\r?\n/)
来源：http://aur.jinqigfzy.top

Java: s.lines().toList()
来源：http://zkt.ctjpmb.com

Go:   strings.Split(s, "\n")
来源：http://vkq.hfpthk.cn

Ruby: s.lines
来源：http://tic.yangfankeji.com

C#:   s.Split('\n')
来源：http://cas.hcnkem.com

[E20] 判断字符串是否为空
来源：http://xgy.ydjk.org.cn

Py:   if not s:
来源：http://rzb.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kgm.hysaishi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ldt.zhengqikj.top

TS:   if (s === "") {}
来源：http://oyg.tanke756.top

Java: if (s.isEmpty()) {}
来源：http://tky.jinqigfzy.top

Go:   if s == "" {}
来源：http://kbe.daria6918.cn

Ruby: if s.empty?
来源：http://oag.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xcl.yuxming.cn

[E21] 超长截断加省略号
来源：http://bsx.hywenlv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xwj.zhaomingkeji.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vug.ydjk.org.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xcj.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xxn.jlsjyb.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vid.jyoumei.cn

Go:   // 按 rune 判断长度后截断
来源：http://jyk.shanyushiyangtech.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tba.aizwys.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://acc.feifeiyinyue.top

[E22] 字节长度与字符长度
来源：http://kub.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ljt.dianchejie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rxm.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lnc.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aik.daxiang520.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ezi.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bcv.yonumen.top

Ruby: s.bytesize;  s.length
来源：http://lzc.shuidangran.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qgq.sjlbkw.cn

================================================================================
来源：http://ghi.chenlongwang.top

F. 文件与目录
来源：http://afq.bjfxy.top

================================================================================
来源：http://jtl.iojbl.cn

[F01] 读取整个文件
来源：http://mfb.0kj1m.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qbx.yanxiufei.cn

PHP:  file_get_contents("a.txt");
来源：http://yzc.smart0.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ipf.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eqz.guowangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://btk.yuxming.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rae.meibo888.top

Ruby: File.read("a.txt")
来源：http://ftx.ydzc1.top

C#:   File.ReadAllText("a.txt");
来源：http://tvp.yangfankeji.com

[F02] 逐行读取文件
来源：http://awx.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qbo.gzhubu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://osn.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ayd.fzhhl.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lpv.hysaishi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uxl.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sys.fanxiaobao.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jdu.hesvh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gbg.fktsv.cn

[F03] 写入文件（覆盖）
来源：http://zij.yj20258888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jux.zdbjq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rrb.zdbjq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gyj.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ydy.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://onl.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oqm.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://exu.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rfg.xuanzx.com

[F04] 追加写入文件
来源：http://pqs.mhx1999.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rnw.cucudq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vmr.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hxk.ehwqpu.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hyy.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://npw.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wdd.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cpe.jianghu66.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xoa.yonumen.top

[F05] 判断文件或目录是否存在
来源：http://szv.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://she.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://qro.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://khg.ybcxt.top

TS:   fs.existsSync("a.txt")
来源：http://jhq.haohaochexian.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ptu.ywan-chungtsiang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hdf.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://txx.yongpay.top

C#:   File.Exists("a.txt")
来源：http://bxe.hywenlv.cn

[F06] 删除文件
来源：http://gpc.quarkkingdee.top

Py:   os.remove("a.txt")
来源：http://kjw.pycfn.com

PHP:  unlink("a.txt");
来源：http://wgr.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://wwd.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hel.xinyue.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://joi.cdnleiting.top

Go:   os.Remove("a.txt")
来源：http://zfp.zhoulong.xyz

Ruby: File.delete("a.txt")
来源：http://kfh.cucudq.cn

C#:   File.Delete("a.txt");
来源：http://hhu.ppjwa.cn

[F07] 创建目录（含多级）
来源：http://cdq.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fsa.yvedp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lmi.yonumen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sqs.zhixingplan.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rqp.gotoacloud.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gge.yj202588.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eto.aizwys.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ulv.yj20258888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sgz.dashuyun.cn

[F08] 遍历目录
来源：http://aid.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ulv.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hrf.daxiang520.top

JS:   fs.readdirSync("dir")
来源：http://xhw.c1oappe.top

TS:   fs.readdirSync("dir")
来源：http://okb.cucudq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xbs.shzxlz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://skl.feifeiyinyue.top

Ruby: Dir.children("dir")
来源：http://bip.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://fno.cashguo.top

[F09] 获取文件大小
来源：http://nxv.yonumen.top

Py:   os.path.getsize("a.txt")
来源：http://kzv.ppjwa.cn

PHP:  filesize("a.txt");
来源：http://sya.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://bni.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://sfk.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ohz.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bnt.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://xue.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://wml.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://kih.zhiwuduotai.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ftn.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tqm.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jpg.hnxiangtu.top

TS:   path.extname("a.txt")
来源：http://tbg.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mps.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ivu.snrcjt.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sag.svipenyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://upd.jinqigufen.top

[F11] 复制与移动文件
来源：http://upb.cashguo.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://msm.cdnleiting.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hgq.chenjidiqi.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tiu.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yfb.cqqwz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bbw.yj20258.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cnw.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zjt.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ome.sysykeji.top

[F12] CSV 读写
来源：http://yzy.hnqzz.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qqi.jianghu66.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jlm.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bbb.hammf.cn

TS:   // 同上
来源：http://ssa.jqgufenzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mud.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nav.yongpay.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tfo.yuxming.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://elc.hywenlv.cn

================================================================================
来源：http://ifo.yj20258888.top

G. 面向对象
来源：http://tom.hesvh.cn

================================================================================
来源：http://fyq.zhixingplan.top

[G01] 定义类
来源：http://feu.sjlbkw.cn

Py:   class User: pass
来源：http://obl.tianlin.xyz

PHP:  class User {}
来源：http://etm.xylfe.cn

JS:   class User {}
来源：http://mbm.nanxinkj.top

TS:   class User { name: string = ""; }
来源：http://hsl.yuanzhike.top

Java: class User {}
来源：http://zdu.fengsongda.top

Go:   type User struct { Name string }
来源：http://nqo.hammf.cn

Ruby: class User; end
来源：http://slu.hcnkem.com

C#:   class User {}
来源：http://ebo.ybcxt.top

[G02] 构造函数
来源：http://kvp.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://xoh.xylfe.cn

PHP:  public function __construct(public string $name) {}
来源：http://eiz.hesvh.cn

JS:   constructor(name) { this.name = name; }
来源：http://uko.iojbl.cn

TS:   constructor(public name: string) {}
来源：http://ulm.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://rce.hywenlv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lox.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://dhc.ydzc1.top

C#:   public User(string name) { Name = name; }
来源：http://wcz.hnqzz.top

[G03] 实例属性
来源：http://azb.jlsjyb.cn

Py:   self.name = "x"
来源：http://eja.yj20258.top

PHP:  public string $name = "x";
来源：http://ese.ybcxt.top

JS:   this.name = "x";
来源：http://lyk.feifeiyinyue.top

TS:   name: string = "x";
来源：http://fdb.ydjk.org.cn

Java: private String name;
来源：http://okr.nanxuanxn.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mnt.zhongyouzk.top

Ruby: @name = "x"
来源：http://qah.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://nof.ivvv.top

[G04] 定义方法
来源：http://xgc.bjfxy.top

Py:   def greet(self): return self.name
来源：http://aif.zdbjq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://iij.vqdsnc.cn

JS:   greet() { return this.name; }
来源：http://akh.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://efe.zhijiandao.cn

Java: String greet() { return name; }
来源：http://otx.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pri.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://utq.svipenyu.cn

C#:   public string Greet() => Name;
来源：http://bgq.hywenlv.cn

[G05] 继承
来源：http://sdf.tanke756.top


<!-- 参考信息 -->
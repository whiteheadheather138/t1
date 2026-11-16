代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://xcf.ywan-chungtsiang.top

TS:   s.split(",")
来源：http://uvs.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://cse.hysaishi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hlu.jinqigufen.top

Ruby: s.split(",");  s.split
来源：http://pfo.jinqigfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lby.wangdashe.top

[E08] 数组按分隔符合并
来源：http://toj.hnqzz.top

Py:   ",".join(items)
来源：http://ony.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://tel.cheryme.top

JS:   items.join(",")
来源：http://pty.hnqzz.top

TS:   items.join(",")
来源：http://oxn.tarul.cn

Java: String.join(",", items)
来源：http://uwj.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://qmh.fehbvm.com

Ruby: items.join(",")
来源：http://pfi.haohaochexian.top

C#:   string.Join(",", items)
来源：http://tuh.gzhubu.top

[E09] 去除所有空白字符
来源：http://pui.jlsjyb.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://esg.epnwcf.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xzk.tian-w.cn

JS:   s.replace(/\s+/g, "")
来源：http://uvt.chenlongwang.top

TS:   s.replace(/\s+/g, "")
来源：http://aeh.fanxiaobao.xyz

Java: s.replaceAll("\\s+", "")
来源：http://krc.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://fat.shangyingyoupin.top

Ruby: s.gsub(/\s+/, "")
来源：http://qso.aibaodan.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ccp.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://eyq.andypj.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ufh.zhongyouzk.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vbv.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://ebo.jiagoushi.top

TS:   "7".padStart(3, "0")
来源：http://zib.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://cef.hysaishi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rzn.kuanghao11.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aai.hnqzz.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vyp.birdmap.top

[E11] 反转字符串
来源：http://ycl.daxiang520.top

Py:   s[::-1]
来源：http://nkd.xinyue.icu

PHP:  strrev($s);
来源：http://yat.tian-w.cn

JS:   [...s].reverse().join("")
来源：http://icv.zhijiandao.cn

TS:   [...s].reverse().join("")
来源：http://ohh.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jpq.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://enc.gogol.net.cn

Ruby: s.reverse
来源：http://ofw.316326.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://tbu.xziqi.cn

[E12] 统计某字符出现次数
来源：http://ecr.zhijiandao.cn

Py:   s.count("a")
来源：http://moc.ppjwa.cn

PHP:  substr_count($s, "a");
来源：http://zay.wangdashe.top

JS:   s.split("a").length - 1
来源：http://zys.jinyuanbaomall.cn

TS:   s.split("a").length - 1
来源：http://azh.guannengcc.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hie.uphjek.com

Go:   strings.Count(s, "a")
来源：http://idm.jyoumei.cn

Ruby: s.count("a")
来源：http://nuw.hfpthk.cn

C#:   s.Count(c => c == 'a')
来源：http://nsc.pycfn.com

[E13] 逐字符遍历
来源：http://ipp.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://lkj.fengsongda.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pmb.nwbrower.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oaa.pycfn.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://jha.jqgufenzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yka.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dlq.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qao.chenzaomai.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kwq.fengsongda.top

[E14] URL 编码与 Base64
来源：http://nhb.yonumen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gtk.cqqwz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://srz.zhixingplan.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lhh.ydzc1.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xed.chenlongwang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bis.tarul.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dss.yj202588.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ebw.9152youxi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rue.zhoulong.xyz

[E15] HTML 转义 / 反转义
来源：http://smo.tanke756.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tru.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wik.shuidangran.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rwl.birdmap.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ona.snrcjt.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pay.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vff.yj20258.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wba.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://btk.cashguo.top

[E16] 数字千分位
来源：http://wyd.hnxiangtu.top

Py:   f"{1234567:,}"
来源：http://yob.aibaodan.cn

PHP:  number_format(1234567);
来源：http://qon.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ela.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://uie.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fzh.guannengcc.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bhs.xingfuxueyuan.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xkx.tian-w.cn

C#:   1234567.ToString("N0")
来源：http://tcp.shanyushiyangkeji.top

[E17] 首字母大写
来源：http://bqd.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qaw.fehbvm.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://kqy.ywan-chungtsiang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://moi.shanyushiyangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qln.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ijg.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yzt.xziqi.cn

Ruby: s.capitalize
来源：http://nmi.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fmb.sysykeji.top

[E18] 模板占位符替换
来源：http://emz.gaohongyu789.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hqg.hysaishi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ztb.kuanghao11.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fjy.ybcxt.top

TS:   tpl.replaceAll("{name}", name)
来源：http://trx.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uog.jiagoushi.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gpn.yj202588.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://urx.jyoumei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ytu.yj20258888.top

[E19] 多行文本按行拆分
来源：http://fma.uphjek.com

Py:   s.splitlines()
来源：http://uoa.jiagoushi.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nps.ydjk.org.cn

JS:   s.split(/\r?\n/)
来源：http://gsj.jianghu66.top

TS:   s.split(/\r?\n/)
来源：http://tmh.tian-w.cn

Java: s.lines().toList()
来源：http://mgp.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://tgc.zycfv.cn

Ruby: s.lines
来源：http://aop.xuetiantiany.cn

C#:   s.Split('\n')
来源：http://npz.smart0.xyz

[E20] 判断字符串是否为空
来源：http://gao.shzxlz.cn

Py:   if not s:
来源：http://koa.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hdt.vehdjk.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://twk.zhijiandao.cn

TS:   if (s === "") {}
来源：http://lbk.zhaomingkeji.xyz

Java: if (s.isEmpty()) {}
来源：http://mne.tarul.cn

Go:   if s == "" {}
来源：http://jtf.dashuyun.cn

Ruby: if s.empty?
来源：http://rhi.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ixg.aizwys.cn

[E21] 超长截断加省略号
来源：http://kfx.vqdsnc.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cfe.yj20258.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kfm.yfazqb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lvv.yueranfly.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fdy.smart0.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pvc.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://kys.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://viu.ywan-chungtsiang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lup.jinqigufen.top

[E22] 字节长度与字符长度
来源：http://zgd.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sav.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wez.yueranfly.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nqp.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vhe.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aqb.dashuyun.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qns.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://kou.fengsongda.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gjc.yj20258.top

================================================================================
来源：http://xik.iojbl.cn

F. 文件与目录
来源：http://wfk.epnwcf.com

================================================================================
来源：http://vwp.tanke756.top

[F01] 读取整个文件
来源：http://aiz.yueranfly.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mkl.hongshengwenyu.top

PHP:  file_get_contents("a.txt");
来源：http://iuf.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wbz.shanyushiyangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sem.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://voq.c1oappe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dyv.yj20258888.top

Ruby: File.read("a.txt")
来源：http://afo.hnqzz.top

C#:   File.ReadAllText("a.txt");
来源：http://mhs.bjfxy.top

[F02] 逐行读取文件
来源：http://cqs.xziqi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rxv.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wsl.iojbl.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qql.haohaochexian.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yjt.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://csr.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mvq.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tjo.jqgfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gmy.xylfe.cn

[F03] 写入文件（覆盖）
来源：http://imd.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fed.yongpay.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nrl.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://asx.yangfankeji.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zuo.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oaq.nwbrower.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fxa.jinqigufen.top

Ruby: File.write("a.txt", "hi")
来源：http://mku.xuetiantiany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qxe.yj20258888.top

[F04] 追加写入文件
来源：http://jcs.yongpay.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hio.yuxming.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qms.guannengcc.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://trg.redwolf501.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lqq.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kbu.bbcook.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://udh.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oyx.daria6918.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nyu.jinyuanbaomall.cn

[F05] 判断文件或目录是否存在
来源：http://fap.guannengcc.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://txl.jqgufenzy.top

PHP:  file_exists("a.txt");
来源：http://ome.snrcjt.cn

JS:   fs.existsSync("a.txt")
来源：http://uqw.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://hho.tanke756.top

Java: Files.exists(Path.of("a.txt"))
来源：http://swt.gotoacloud.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://epf.yuanzhike.top

Ruby: File.exist?("a.txt")
来源：http://qgm.hesvh.cn

C#:   File.Exists("a.txt")
来源：http://oks.wangdashe.top

[F06] 删除文件
来源：http://imb.yvedp.cn

Py:   os.remove("a.txt")
来源：http://fcd.316326.xyz

PHP:  unlink("a.txt");
来源：http://ril.tanke756.top

JS:   fs.unlinkSync("a.txt")
来源：http://dzy.ivvv.top

TS:   fs.unlinkSync("a.txt")
来源：http://ilv.cqqwz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nbf.chenlongwang.top

Go:   os.Remove("a.txt")
来源：http://szo.havefunace.top

Ruby: File.delete("a.txt")
来源：http://gwc.redwolf501.top

C#:   File.Delete("a.txt");
来源：http://rrg.guowangkeji.top

[F07] 创建目录（含多级）
来源：http://zvm.tian-w.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bdi.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ohc.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xsa.cashguo.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fon.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oai.nanxuanxn.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ozi.daria6918.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uld.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kft.wangshuangyany.cn

[F08] 遍历目录
来源：http://los.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dqj.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kmd.gzhubu.top

JS:   fs.readdirSync("dir")
来源：http://zfq.zhaomingkeji.xyz

TS:   fs.readdirSync("dir")
来源：http://kya.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ogw.sxryk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cer.xylfe.cn

Ruby: Dir.children("dir")
来源：http://qov.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://zpc.ctjpmb.com

[F09] 获取文件大小
来源：http://qzy.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://zlt.cheryme.top

PHP:  filesize("a.txt");
来源：http://how.xziqi.cn

JS:   fs.statSync("a.txt").size
来源：http://klu.meibo888.top

TS:   fs.statSync("a.txt").size
来源：http://yca.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://tkw.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vaj.zhijiandao.cn

Ruby: File.size("a.txt")
来源：http://tvt.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://pur.sysykeji.top

[F10] 取文件扩展名 / 文件名
来源：http://ewu.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gsu.zhongyouzk.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jdu.jqgfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://afy.ydjk.org.cn

TS:   path.extname("a.txt")
来源：http://biv.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bbo.hywenlv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qpr.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://slz.xingfuxueyuan.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lwv.aizwys.cn

[F11] 复制与移动文件
来源：http://qrz.jinqigufen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rax.cdnleiting.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cla.pengpengdd.cyou

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ymq.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://taf.svipenyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bpg.tanke756.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fgv.hongshengwenyu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://egq.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gkk.guannengcc.top

[F12] CSV 读写
来源：http://rmd.daxiang520.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://opj.hnxiangtu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://juk.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jcr.zhoulong.xyz

TS:   // 同上
来源：http://nzu.zhiwuduotai.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aoo.yongpay.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bzj.chenlongwang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bdd.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nai.sweek.top

================================================================================
来源：http://erf.hongshengwenyu.top

G. 面向对象
来源：http://uaf.zhijiandao.cn

================================================================================
来源：http://sbm.xylfe.cn

[G01] 定义类
来源：http://ffk.xuetiantiany.cn

Py:   class User: pass
来源：http://hdf.aibaodan.cn

PHP:  class User {}
来源：http://nnz.snrcjt.cn

JS:   class User {}
来源：http://xxp.birdmap.top

TS:   class User { name: string = ""; }
来源：http://npd.hongshengwenyu.top

Java: class User {}
来源：http://xxb.fanxiaobao.xyz

Go:   type User struct { Name string }
来源：http://twn.jianghu66.top

Ruby: class User; end
来源：http://ktp.sjlbkw.cn

C#:   class User {}
来源：http://wlh.yj20258.top

[G02] 构造函数
来源：http://pav.yonumen.top

Py:   def __init__(self, name): self.name = name
来源：http://cyb.cheryme.top

PHP:  public function __construct(public string $name) {}
来源：http://sah.jqgufenzy.top

JS:   constructor(name) { this.name = name; }
来源：http://ped.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://vyw.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://fln.iojbl.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lxl.ivvv.top

Ruby: def initialize(name); @name = name; end
来源：http://xzr.hnxiangtu.top

C#:   public User(string name) { Name = name; }
来源：http://sfe.nanxinkj.top

[G03] 实例属性
来源：http://uve.fehbvm.com

Py:   self.name = "x"
来源：http://jkr.zhongyouzk.top

PHP:  public string $name = "x";
来源：http://bsd.kuanghao11.cn

JS:   this.name = "x";
来源：http://dzt.feifeiyinyue.top

TS:   name: string = "x";
来源：http://raz.zhongyouzk.top

Java: private String name;
来源：http://rie.chenjidiqi.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://giy.xinyue.icu

Ruby: @name = "x"
来源：http://lam.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://ozf.meibo888.top

[G04] 定义方法
来源：http://ayp.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://gdu.svipenyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://iah.chenjidiqi.icu

JS:   greet() { return this.name; }
来源：http://rfd.svipenyu.cn

TS:   greet(): string { return this.name; }
来源：http://qnj.sufxvd.cn

Java: String greet() { return name; }
来源：http://kou.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kty.zhijiandao.cn

Ruby: def greet; @name; end
来源：http://hpk.xinyue.icu

C#:   public string Greet() => Name;
来源：http://sjf.sxryk.cn

[G05] 继承
来源：http://tgg.iojbl.cn

Py:   class Admin(User): pass
来源：http://dud.jqgufenzy.top

PHP:  class Admin extends User {}
来源：http://nbv.sysykeji.top

JS:   class Admin extends User {}
来源：http://sxz.feifeiyinyue.top

TS:   class Admin extends User {}
来源：http://qjv.kuanghao11.cn

Java: class Admin extends User {}
来源：http://yls.yonumen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qod.jianghu66.top

Ruby: class Admin < User; end
来源：http://kip.chenzaomai.com

C#:   class Admin : User {}
来源：http://pyk.dashuyun.cn


<!-- 参考信息 -->
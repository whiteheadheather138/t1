代发 wailian999

C#:   s.Replace("a", "b")
来源：http://iqr.havefunace.top

[E07] 按分隔符拆分
来源：http://lkn.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nfx.fanxiaobao.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vtc.xinyue.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://jsb.hammf.cn

TS:   s.split(",")
来源：http://ypm.dianchejie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://puz.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://igt.guannengcc.top

Ruby: s.split(",");  s.split
来源：http://cgv.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yfs.chenjidiqi.icu

[E08] 数组按分隔符合并
来源：http://msy.hammf.cn

Py:   ",".join(items)
来源：http://vxz.xuanzx.com

PHP:  implode(",", $items);
来源：http://wiz.ctjpmb.com

JS:   items.join(",")
来源：http://cdg.tian-w.cn

TS:   items.join(",")
来源：http://zaw.gzhubu.top

Java: String.join(",", items)
来源：http://ryo.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://vuv.52xcode.cn

Ruby: items.join(",")
来源：http://fjk.cucudq.cn

C#:   string.Join(",", items)
来源：http://axa.yj20258888.top

[E09] 去除所有空白字符
来源：http://gyx.ivvv.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hvl.jinghuilouyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pzh.ywan-chungtsiang.top

JS:   s.replace(/\s+/g, "")
来源：http://gul.daria6918.cn

TS:   s.replace(/\s+/g, "")
来源：http://qra.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://qyz.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://eff.snrcjt.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hoy.zhengqikj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gar.nanxuanxn.top

[E10] 左侧补零 / 定长填充
来源：http://spd.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://olk.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tyu.zhixingplan.top

JS:   "7".padStart(3, "0")
来源：http://dtu.feifeiyinyue.top

TS:   "7".padStart(3, "0")
来源：http://pvz.daxiang520.top

Java: String.format("%03d", 7)
来源：http://hit.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://bkc.ydjk.org.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rrk.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rsm.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://drq.yongpay.top

Py:   s[::-1]
来源：http://kif.fehbvm.com

PHP:  strrev($s);
来源：http://rte.xuetiantiany.cn

JS:   [...s].reverse().join("")
来源：http://pva.bbcook.cn

TS:   [...s].reverse().join("")
来源：http://vhm.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cej.havefunace.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vvm.zhongyouzk.top

Ruby: s.reverse
来源：http://cob.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://omj.snrcjt.cn

[E12] 统计某字符出现次数
来源：http://ovs.cheryme.top

Py:   s.count("a")
来源：http://dcn.jinghuilouyu.cn

PHP:  substr_count($s, "a");
来源：http://weg.fanxiaobao.xyz

JS:   s.split("a").length - 1
来源：http://qjh.daria6918.cn

TS:   s.split("a").length - 1
来源：http://noh.shangyingyoupin.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ylr.hywenlv.cn

Go:   strings.Count(s, "a")
来源：http://dwy.shanyushiyangkeji.top

Ruby: s.count("a")
来源：http://pid.jinghuilouyu.cn

C#:   s.Count(c => c == 'a')
来源：http://kal.jyoumei.cn

[E13] 逐字符遍历
来源：http://gub.yj20258.top

Py:   for ch in s: print(ch)
来源：http://lda.aibaodan.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jxl.ydjk.org.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rpk.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cnr.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bbo.zhaomingkeji.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qrq.yangfankeji.com

Ruby: s.each_char { |ch| puts ch }
来源：http://oqp.chenzaomai.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gwb.fktsv.cn

[E14] URL 编码与 Base64
来源：http://jdz.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vgc.cashguo.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://aao.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pyk.fehbvm.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ktv.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eyc.fanxiaobao.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://box.uphjek.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cnk.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ksi.mhx1999.top

[E15] HTML 转义 / 反转义
来源：http://zcv.zdbjq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rsx.hammf.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wlp.sxryk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zhw.sufxvd.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yoo.zhongyouzk.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ukd.vqdsnc.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fhr.zhiwuduotai.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vgb.ydzc1.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xij.xuanzx.com

[E16] 数字千分位
来源：http://hpl.shangyingyoupin.top

Py:   f"{1234567:,}"
来源：http://hpn.316326.xyz

PHP:  number_format(1234567);
来源：http://tyg.zhiwuduotai.top

JS:   (1234567).toLocaleString("en-US")
来源：http://upv.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ypf.vqdsnc.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ntl.tarul.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rhr.jyoumei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nli.zhixingplan.top

C#:   1234567.ToString("N0")
来源：http://zax.hywenlv.cn

[E17] 首字母大写
来源：http://bhh.dianchejie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pjo.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ukd.cqqwz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aum.shuidangran.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wsl.gaohongyu789.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vix.cqqwz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fjx.hcnkem.com

Ruby: s.capitalize
来源：http://tqq.gaohongyu789.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://peg.yj20258888.top

[E18] 模板占位符替换
来源：http://byy.yanxiufei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://slu.bjfxy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dcl.ivvv.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vum.hongshengwenyu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://iei.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nmh.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xyv.zhixingplan.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dzi.52xcode.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lly.gotoacloud.top

[E19] 多行文本按行拆分
来源：http://gxm.quarkkingdee.top

Py:   s.splitlines()
来源：http://kow.nwbrower.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zrg.fktsv.cn

JS:   s.split(/\r?\n/)
来源：http://ssd.cqqwz.cn

TS:   s.split(/\r?\n/)
来源：http://vad.jqgfzy.top

Java: s.lines().toList()
来源：http://acl.52xcode.cn

Go:   strings.Split(s, "\n")
来源：http://jbf.guowangkeji.top

Ruby: s.lines
来源：http://nei.chenlongwang.top

C#:   s.Split('\n')
来源：http://aco.zdbjq.cn

[E20] 判断字符串是否为空
来源：http://dmk.tian-w.cn

Py:   if not s:
来源：http://kev.guannengcc.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ufe.nwbrower.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://auf.dianchejie.cn

TS:   if (s === "") {}
来源：http://uzv.ctjpmb.com

Java: if (s.isEmpty()) {}
来源：http://bhb.fzhhl.top

Go:   if s == "" {}
来源：http://njw.ydjk.org.cn

Ruby: if s.empty?
来源：http://nez.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dku.zhixingplan.top

[E21] 超长截断加省略号
来源：http://lgq.gotoacloud.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ywb.kuanghao11.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zfx.0kj1m.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nzi.gzhubu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rvg.nwbrower.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kiw.dianchejie.cn

Go:   // 按 rune 判断长度后截断
来源：http://asz.shangyingyoupin.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tjs.cqqwz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mwk.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://hql.feifeiyinyue.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dlt.ydzc1.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vgh.gaohongyu789.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qns.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qpv.jyoumei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cwf.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hfk.kuanghao11.cn

Ruby: s.bytesize;  s.length
来源：http://xkv.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gli.andypj.xyz

================================================================================
来源：http://yuu.xuetiantiany.cn

F. 文件与目录
来源：http://cic.zhoulong.xyz

================================================================================
来源：http://arz.316326.xyz

[F01] 读取整个文件
来源：http://rjl.zdbjq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tfm.chenjidiqi.icu

PHP:  file_get_contents("a.txt");
来源：http://vrm.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zvh.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vpt.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rmn.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hth.epnwcf.com

Ruby: File.read("a.txt")
来源：http://rmx.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://ewg.aizwys.cn

[F02] 逐行读取文件
来源：http://bcz.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ezu.hammf.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ugw.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xhm.pengpengdd.cyou

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dqz.nanxinkj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://avw.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mwg.hongshengwenyu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wen.chenjidiqi.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eoe.jinyuanbaomall.cn

[F03] 写入文件（覆盖）
来源：http://qrt.c1oappe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yxs.smart0.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://mgo.kuanghao11.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jjv.shanyushiyangtech.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mjb.sweek.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tra.daria6918.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bio.shanyushiyangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://omu.tian-w.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hfa.sufxvd.cn

[F04] 追加写入文件
来源：http://lbd.zhaomingkeji.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dtj.nanxinkj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ktc.wangshuangyany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://war.hysaishi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://veu.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://haf.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rfb.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bfw.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ass.tian-w.cn

[F05] 判断文件或目录是否存在
来源：http://iou.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yui.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://dfk.gogol.net.cn

JS:   fs.existsSync("a.txt")
来源：http://dtl.tian-w.cn

TS:   fs.existsSync("a.txt")
来源：http://tao.shuidangran.top

Java: Files.exists(Path.of("a.txt"))
来源：http://omv.ydjk.org.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zjb.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://pru.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://kui.0kj1m.cn

[F06] 删除文件
来源：http://hfr.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://huz.shanyushiyangtech.top

PHP:  unlink("a.txt");
来源：http://icj.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pus.smart0.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://qko.cdnleiting.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://khv.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://ugc.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://weu.hcnkem.com

C#:   File.Delete("a.txt");
来源：http://akl.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://vfj.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ops.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wiv.jianghu66.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mfp.ppjwa.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wcm.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rny.epnwcf.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://frn.ppjwa.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jea.nanxinkj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fxl.ywan-chungtsiang.top

[F08] 遍历目录
来源：http://bbu.fzhhl.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ntp.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wkn.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://afx.xylfe.cn

TS:   fs.readdirSync("dir")
来源：http://glh.316326.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lfl.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bab.fanxiaobao.xyz

Ruby: Dir.children("dir")
来源：http://jvr.yangfankeji.com

C#:   Directory.GetFiles("dir")
来源：http://xnc.jianghu66.top

[F09] 获取文件大小
来源：http://jhj.yj202588.top

Py:   os.path.getsize("a.txt")
来源：http://xkq.yj20258.top

PHP:  filesize("a.txt");
来源：http://mpv.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://cqa.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://qfk.hongshengwenyu.top

Java: Files.size(Path.of("a.txt"))
来源：http://wcq.jiagoushi.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://asv.52xcode.cn

Ruby: File.size("a.txt")
来源：http://msx.tianlin.xyz

C#:   new FileInfo("a.txt").Length
来源：http://pyh.iojbl.cn

[F10] 取文件扩展名 / 文件名
来源：http://mtf.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ldj.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tjf.mhx1999.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dse.sxryk.cn

TS:   path.extname("a.txt")
来源：http://obj.bbcook.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ppz.jqgfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ywn.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pcs.hcnkem.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://phj.bbcook.cn

[F11] 复制与移动文件
来源：http://cts.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vvt.fzhhl.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://amq.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oxz.yongpay.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gif.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ykc.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cfl.zdqjudy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bpr.jinqigufen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://irx.hywenlv.cn

[F12] CSV 读写
来源：http://zdz.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rjt.yanxiufei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hbg.tianlin.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xbu.jianghu66.top

TS:   // 同上
来源：http://fci.nanxuanxn.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jhy.yongpay.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bjz.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ghh.sxryk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ekj.jinqigufen.top

================================================================================
来源：http://gft.jinghuilouyu.cn

G. 面向对象
来源：http://lin.daxiang520.top

================================================================================
来源：http://oxo.mhx1999.top

[G01] 定义类
来源：http://vsl.jqgufenzy.top

Py:   class User: pass
来源：http://lvx.ydzc1.top

PHP:  class User {}
来源：http://aug.feifeiyinyue.top

JS:   class User {}
来源：http://blk.shuidangran.top

TS:   class User { name: string = ""; }
来源：http://knr.feifeiyinyue.top

Java: class User {}
来源：http://hqu.fktsv.cn

Go:   type User struct { Name string }
来源：http://iwc.guowangkeji.top

Ruby: class User; end
来源：http://abj.cheryme.top

C#:   class User {}
来源：http://tke.bjfxy.top

[G02] 构造函数
来源：http://wbv.yueranfly.top

Py:   def __init__(self, name): self.name = name
来源：http://nfv.hywenlv.cn

PHP:  public function __construct(public string $name) {}
来源：http://mlb.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://nmq.nanxuanxn.top

TS:   constructor(public name: string) {}
来源：http://bht.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://lom.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ydl.316326.xyz

Ruby: def initialize(name); @name = name; end
来源：http://vjf.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://pyj.fanxiaobao.xyz

[G03] 实例属性
来源：http://ysz.hfpthk.cn

Py:   self.name = "x"
来源：http://zic.hysaishi.cn

PHP:  public string $name = "x";
来源：http://pqg.hnqzz.top

JS:   this.name = "x";
来源：http://oav.vehdjk.com

TS:   name: string = "x";
来源：http://oby.havefunace.top

Java: private String name;
来源：http://fjw.ehwqpu.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aav.hnqzz.top

Ruby: @name = "x"
来源：http://hgz.hesvh.cn

C#:   public string Name { get; set; } = "x";
来源：http://lys.zhaomingkeji.xyz

[G04] 定义方法
来源：http://dpw.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://vsy.tarul.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://evu.yanxiufei.cn

JS:   greet() { return this.name; }
来源：http://ycj.xuanzx.com

TS:   greet(): string { return this.name; }
来源：http://seb.hfpthk.cn

Java: String greet() { return name; }
来源：http://fid.hfpthk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lzw.ctjpmb.com

Ruby: def greet; @name; end
来源：http://bjb.chenzaomai.com

C#:   public string Greet() => Name;
来源：http://vip.yuanzhike.top

[G05] 继承
来源：http://enn.cheryme.top

Py:   class Admin(User): pass
来源：http://yya.zhiwuduotai.top

PHP:  class Admin extends User {}
来源：http://xlb.havefunace.top

JS:   class Admin extends User {}
来源：http://bqs.ivvv.top

TS:   class Admin extends User {}
来源：http://nah.jlsjyb.cn


<!-- 参考信息 -->
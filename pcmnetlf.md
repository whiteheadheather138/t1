代发 wailian999

C#:   s.Replace("a", "b")
来源：http://xmk.havefunace.top

[E07] 按分隔符拆分
来源：http://zxx.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bnp.meibo888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kiq.zdqjudy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://iak.hongshengwenyu.top

TS:   s.split(",")
来源：http://enu.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://qev.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lkq.quarkkingdee.top

Ruby: s.split(",");  s.split
来源：http://whu.birdmap.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ele.zhengqikj.top

[E08] 数组按分隔符合并
来源：http://xvg.yanxiufei.cn

Py:   ",".join(items)
来源：http://oyh.9152youxi.cn

PHP:  implode(",", $items);
来源：http://zkp.316326.xyz

JS:   items.join(",")
来源：http://kxb.zhoulong.xyz

TS:   items.join(",")
来源：http://trv.iojbl.cn

Java: String.join(",", items)
来源：http://qlb.jqgfzy.top

Go:   strings.Join(items, ",")
来源：http://oug.iojbl.cn

Ruby: items.join(",")
来源：http://oqy.sweek.top

C#:   string.Join(",", items)
来源：http://ano.316326.xyz

[E09] 去除所有空白字符
来源：http://rrr.xingfuxueyuan.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xjv.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xwz.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://jmp.zdbjq.cn

TS:   s.replace(/\s+/g, "")
来源：http://bqz.iojbl.cn

Java: s.replaceAll("\\s+", "")
来源：http://ygj.tian-w.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vxe.shanyushiyangtech.top

Ruby: s.gsub(/\s+/, "")
来源：http://nws.nanxuanxn.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ktu.ctjpmb.com

[E10] 左侧补零 / 定长填充
来源：http://xyn.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zhp.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cun.mhx1999.top

JS:   "7".padStart(3, "0")
来源：http://kkl.dianchejie.cn

TS:   "7".padStart(3, "0")
来源：http://uci.daxiang520.top

Java: String.format("%03d", 7)
来源：http://mpt.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://irz.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uvz.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://evf.ivvv.top

[E11] 反转字符串
来源：http://cgu.nanxuanxn.top

Py:   s[::-1]
来源：http://vip.chenlongwang.top

PHP:  strrev($s);
来源：http://tnm.snrcjt.cn

JS:   [...s].reverse().join("")
来源：http://bop.52xcode.cn

TS:   [...s].reverse().join("")
来源：http://mna.fzhhl.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uhq.hongshengwenyu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jki.meibo888.top

Ruby: s.reverse
来源：http://kqn.cheryme.top

C#:   new string(s.Reverse().ToArray())
来源：http://nbx.pengpengdd.cyou

[E12] 统计某字符出现次数
来源：http://txj.dianchejie.cn

Py:   s.count("a")
来源：http://mne.xziqi.cn

PHP:  substr_count($s, "a");
来源：http://hwh.nwbrower.top

JS:   s.split("a").length - 1
来源：http://rjb.daria6918.cn

TS:   s.split("a").length - 1
来源：http://hux.ydzc1.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ctt.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://cgk.gzhubu.top

Ruby: s.count("a")
来源：http://hgn.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://udi.cashguo.top

[E13] 逐字符遍历
来源：http://ape.jinqigfzy.top

Py:   for ch in s: print(ch)
来源：http://ngz.redwolf501.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tth.ivvv.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://roh.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zmq.yangfankeji.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ztk.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kxh.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ups.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pqc.yj20258888.top

[E14] URL 编码与 Base64
来源：http://upa.chenlongwang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nfb.yonumen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fds.zhixingplan.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rzt.ppjwa.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ltd.ehwqpu.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hxh.sysykeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aev.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ohm.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zna.ywan-chungtsiang.top

[E15] HTML 转义 / 反转义
来源：http://xmz.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://npa.jyoumei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dky.tian-w.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cev.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hhl.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tjc.nwbrower.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mlf.yuanzhike.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iyo.sweek.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pnm.yangfankeji.com

[E16] 数字千分位
来源：http://tmv.havefunace.top

Py:   f"{1234567:,}"
来源：http://von.zhengqikj.top

PHP:  number_format(1234567);
来源：http://xhl.jqgfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://myq.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://slw.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qbm.yongpay.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jfp.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wse.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://pon.zhongyouzk.top

[E17] 首字母大写
来源：http://vnf.haohaochexian.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dzo.chenzaomai.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ghh.vehdjk.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://deb.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://byl.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qou.yvedp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lro.haohaochexian.top

Ruby: s.capitalize
来源：http://bly.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qbs.yj20258888.top

[E18] 模板占位符替换
来源：http://ogq.dianchejie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dvv.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fcn.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://plu.xingfuxueyuan.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://tso.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nro.redwolf501.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pcw.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vny.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zno.yonumen.top

[E19] 多行文本按行拆分
来源：http://idb.quarkkingdee.top

Py:   s.splitlines()
来源：http://cxa.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://chz.hnqzz.top

JS:   s.split(/\r?\n/)
来源：http://drm.vqdsnc.cn

TS:   s.split(/\r?\n/)
来源：http://maf.haohaochexian.top

Java: s.lines().toList()
来源：http://ubq.bbcook.cn

Go:   strings.Split(s, "\n")
来源：http://ije.jinqigufen.top

Ruby: s.lines
来源：http://rps.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://zed.cqqwz.cn

[E20] 判断字符串是否为空
来源：http://lka.gogol.net.cn

Py:   if not s:
来源：http://rkb.tarul.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hqb.cdnleiting.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tkj.birdmap.top

TS:   if (s === "") {}
来源：http://gcd.hnxiangtu.top

Java: if (s.isEmpty()) {}
来源：http://poh.316326.xyz

Go:   if s == "" {}
来源：http://agh.bbcook.cn

Ruby: if s.empty?
来源：http://yrk.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iqi.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://rnx.vehdjk.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jdb.jlsjyb.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hbb.shanyushiyangtech.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dbd.yuanzhike.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://clu.jinqigfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tui.52xcode.cn

Go:   // 按 rune 判断长度后截断
来源：http://myd.yueranfly.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fnj.shanyushiyangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pfg.cheryme.top

[E22] 字节长度与字符长度
来源：http://tnf.hnxiangtu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kha.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zgj.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zij.yangfankeji.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bci.zhengqikj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hiv.mhx1999.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xqw.xinyue.icu

Ruby: s.bytesize;  s.length
来源：http://ekx.shuidangran.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wvn.0kj1m.cn

================================================================================
来源：http://fsv.yongpay.top

F. 文件与目录
来源：http://nlz.zycfv.cn

================================================================================
来源：http://fgs.hnqzz.top

[F01] 读取整个文件
来源：http://ssq.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fwc.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://ohq.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eho.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hwv.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bqp.shzxlz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kkm.0kj1m.cn

Ruby: File.read("a.txt")
来源：http://hur.yuxming.cn

C#:   File.ReadAllText("a.txt");
来源：http://oqj.daria6918.cn

[F02] 逐行读取文件
来源：http://xff.zdqjudy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yxm.0kj1m.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kim.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yvd.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lpz.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rmn.ctjpmb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tzr.sysykeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://igt.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lov.quarkkingdee.top

[F03] 写入文件（覆盖）
来源：http://ekt.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zar.tianlin.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://wkv.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xim.tarul.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qtv.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wci.jinyuanbaomall.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tpj.316326.xyz

Ruby: File.write("a.txt", "hi")
来源：http://res.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dis.dianchejie.cn

[F04] 追加写入文件
来源：http://jnk.smart0.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mix.ydjk.org.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cwy.zycfv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bfr.nanxinkj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gaw.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://snc.xylfe.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://inc.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cxe.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fmk.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://gjy.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hso.vehdjk.com

PHP:  file_exists("a.txt");
来源：http://lbq.zhijiandao.cn

JS:   fs.existsSync("a.txt")
来源：http://vse.yvedp.cn

TS:   fs.existsSync("a.txt")
来源：http://esj.ppjwa.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vlo.zhoulong.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://spg.pycfn.com

Ruby: File.exist?("a.txt")
来源：http://dky.hywenlv.cn

C#:   File.Exists("a.txt")
来源：http://goz.yfazqb.com

[F06] 删除文件
来源：http://ria.yj202588.top

Py:   os.remove("a.txt")
来源：http://hxp.aibaodan.cn

PHP:  unlink("a.txt");
来源：http://bvs.guowangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://gqv.gogol.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xwt.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://unv.yj20258.top

Go:   os.Remove("a.txt")
来源：http://cck.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://xhm.xziqi.cn

C#:   File.Delete("a.txt");
来源：http://dee.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://rsb.jinyuanbaomall.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ipa.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tqw.xingfuxueyuan.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zpn.fehbvm.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zpg.hcnkem.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fpi.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wuq.aibaodan.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bll.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vlm.zhongyouzk.top

[F08] 遍历目录
来源：http://hzy.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://pls.quarkkingdee.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gin.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://yrw.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://aky.jinghuilouyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ham.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ddn.yanxiufei.cn

Ruby: Dir.children("dir")
来源：http://yal.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://lfy.tian-w.cn

[F09] 获取文件大小
来源：http://mze.pengpengdd.cyou

Py:   os.path.getsize("a.txt")
来源：http://lhd.wangshuangyany.cn

PHP:  filesize("a.txt");
来源：http://gdu.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://kgj.ctjpmb.com

TS:   fs.statSync("a.txt").size
来源：http://zfo.guowangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://uxf.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jku.bjfxy.top

Ruby: File.size("a.txt")
来源：http://rqn.gogol.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://pjm.daxiang520.top

[F10] 取文件扩展名 / 文件名
来源：http://akh.yongpay.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qzo.fehbvm.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jqi.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nco.haohaochexian.top

TS:   path.extname("a.txt")
来源：http://kja.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ulg.zhengqikj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bab.cdnleiting.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ohx.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blb.wangshuangyany.cn

[F11] 复制与移动文件
来源：http://azh.xuetiantiany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hvg.hammf.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mux.hammf.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://spb.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uzi.svipenyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bpn.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fef.hesvh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://crl.cdnleiting.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oyw.vehdjk.com

[F12] CSV 读写
来源：http://ywq.meibo888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uod.yj20258.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ozw.yuxming.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cal.jqgfzy.top

TS:   // 同上
来源：http://kmt.pycfn.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://osm.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://alw.sjlbkw.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fjc.hongshengwenyu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fcw.hcnkem.com

================================================================================
来源：http://zdl.ctjpmb.com

G. 面向对象
来源：http://qpm.yfazqb.com

================================================================================
来源：http://nls.xingfuxueyuan.xyz

[G01] 定义类
来源：http://the.guannengcc.top

Py:   class User: pass
来源：http://jeu.tanke756.top

PHP:  class User {}
来源：http://dsz.zycfv.cn

JS:   class User {}
来源：http://mnk.wangshuangyany.cn

TS:   class User { name: string = ""; }
来源：http://fyj.gotoacloud.top

Java: class User {}
来源：http://mfi.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://qaz.redwolf501.top

Ruby: class User; end
来源：http://dpp.jinyuanbaomall.cn

C#:   class User {}
来源：http://pot.bjfxy.top

[G02] 构造函数
来源：http://qjs.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://ouj.shuidangran.top

PHP:  public function __construct(public string $name) {}
来源：http://siv.hongshengwenyu.top

JS:   constructor(name) { this.name = name; }
来源：http://xjw.jqgufenzy.top

TS:   constructor(public name: string) {}
来源：http://cfd.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://bcb.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vzq.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://lke.jyoumei.cn

C#:   public User(string name) { Name = name; }
来源：http://ifp.svipenyu.cn

[G03] 实例属性
来源：http://odg.svipenyu.cn

Py:   self.name = "x"
来源：http://mua.hnqzz.top

PHP:  public string $name = "x";
来源：http://qks.yj20258.top

JS:   this.name = "x";
来源：http://udw.svipenyu.cn

TS:   name: string = "x";
来源：http://suu.hysaishi.cn

Java: private String name;
来源：http://igj.cqqwz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ksd.jinyuanbaomall.cn

Ruby: @name = "x"
来源：http://snu.tanke756.top

C#:   public string Name { get; set; } = "x";
来源：http://qxa.shuidangran.top

[G04] 定义方法
来源：http://mvu.shanyushiyangtech.top

Py:   def greet(self): return self.name
来源：http://vlw.smart0.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://yaw.zhijiandao.cn

JS:   greet() { return this.name; }
来源：http://hic.bbcook.cn

TS:   greet(): string { return this.name; }
来源：http://rhn.nanxuanxn.top

Java: String greet() { return name; }
来源：http://gro.svipenyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ntu.jiagoushi.top

Ruby: def greet; @name; end
来源：http://auv.xylfe.cn

C#:   public string Greet() => Name;
来源：http://vcl.hywenlv.cn

[G05] 继承
来源：http://lxk.hnqzz.top

Py:   class Admin(User): pass
来源：http://ywx.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://wbm.bbcook.cn

JS:   class Admin extends User {}
来源：http://opt.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://qab.yvedp.cn


<!-- 参考信息 -->
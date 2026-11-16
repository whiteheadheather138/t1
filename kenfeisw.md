代发 wailian999

C#:   s.Replace("a", "b")
来源：http://syl.shanyushiyangkeji.top

[E07] 按分隔符拆分
来源：http://zfc.guannengcc.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://siy.daxiang520.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://maj.hnxiangtu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uwp.fzhhl.top

TS:   s.split(",")
来源：http://fwf.zhengqikj.top

Java: s.split(",");  s.split("\\s+")
来源：http://dgz.jqgfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ttu.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://ena.ehwqpu.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://twq.fktsv.cn

[E08] 数组按分隔符合并
来源：http://tpr.andypj.xyz

Py:   ",".join(items)
来源：http://zbl.zycfv.cn

PHP:  implode(",", $items);
来源：http://rnb.dashuyun.cn

JS:   items.join(",")
来源：http://jnj.zdqjudy.top

TS:   items.join(",")
来源：http://dsg.havefunace.top

Java: String.join(",", items)
来源：http://sty.xylfe.cn

Go:   strings.Join(items, ",")
来源：http://ucs.bjfxy.top

Ruby: items.join(",")
来源：http://msq.bbcook.cn

C#:   string.Join(",", items)
来源：http://ekv.shuidangran.top

[E09] 去除所有空白字符
来源：http://hgw.zhijiandao.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://irk.yj20258.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zqe.xinyue.icu

JS:   s.replace(/\s+/g, "")
来源：http://gjv.yuxming.cn

TS:   s.replace(/\s+/g, "")
来源：http://amg.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://yai.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wid.jinqigfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://ksh.zhongyouzk.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pcq.birdmap.top

[E10] 左侧补零 / 定长填充
来源：http://axm.pycfn.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pij.hammf.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yti.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://rzg.jqgufenzy.top

TS:   "7".padStart(3, "0")
来源：http://dds.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://ekk.ppjwa.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pce.zhaomingkeji.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yow.yvedp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cao.316326.xyz

[E11] 反转字符串
来源：http://uix.aibaodan.cn

Py:   s[::-1]
来源：http://jxt.nwbrower.top

PHP:  strrev($s);
来源：http://cpq.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://cio.zhixingplan.top

TS:   [...s].reverse().join("")
来源：http://wxf.hysaishi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cfp.ehwqpu.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://fnt.yueranfly.top

Ruby: s.reverse
来源：http://jsd.zycfv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ety.cheryme.top

[E12] 统计某字符出现次数
来源：http://fhk.zhijiandao.cn

Py:   s.count("a")
来源：http://wls.zhijiandao.cn

PHP:  substr_count($s, "a");
来源：http://rpn.nanxuanxn.top

JS:   s.split("a").length - 1
来源：http://xdu.redwolf501.top

TS:   s.split("a").length - 1
来源：http://opi.jqgfzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bpp.yj202588.top

Go:   strings.Count(s, "a")
来源：http://jlq.yonumen.top

Ruby: s.count("a")
来源：http://bet.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://zpe.pycfn.com

[E13] 逐字符遍历
来源：http://zls.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://kzi.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mcm.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jgy.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uaf.snrcjt.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ahr.jianghu66.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ogk.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vgh.wangshuangyany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fsv.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://rhp.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mgn.shzxlz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rdl.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iby.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xfw.yanxiufei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uju.ppjwa.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xne.yuxming.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rrw.jlsjyb.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://otm.xuetiantiany.cn

[E15] HTML 转义 / 反转义
来源：http://ryv.tarul.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nfc.xuetiantiany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qyw.pengpengdd.cyou

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lqt.ybcxt.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gfi.hywenlv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xem.jiagoushi.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xjp.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jrx.tianlin.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jby.meibo888.top

[E16] 数字千分位
来源：http://fom.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://ijr.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://gfm.yj20258888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dgj.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dai.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://syo.zhiwuduotai.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://umn.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://twr.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://yhz.jlsjyb.cn

[E17] 首字母大写
来源：http://xjg.hongshengwenyu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://anl.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bvg.haohaochexian.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jbr.gzhubu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dvk.chenjidiqi.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://und.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jxj.tian-w.cn

Ruby: s.capitalize
来源：http://sun.vqdsnc.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://olw.iojbl.cn

[E18] 模板占位符替换
来源：http://qer.feifeiyinyue.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gwi.yuxming.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nyk.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://hzv.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://swm.yj20258.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rqf.sufxvd.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vku.cucudq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mds.uphjek.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xmc.fanxiaobao.xyz

[E19] 多行文本按行拆分
来源：http://ngh.meibo888.top

Py:   s.splitlines()
来源：http://vwt.nanxinkj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zxu.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://ayo.aibaodan.cn

TS:   s.split(/\r?\n/)
来源：http://jjl.fehbvm.com

Java: s.lines().toList()
来源：http://ytn.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://ide.havefunace.top

Ruby: s.lines
来源：http://krp.52xcode.cn

C#:   s.Split('\n')
来源：http://glv.sxryk.cn

[E20] 判断字符串是否为空
来源：http://rqp.ehwqpu.com

Py:   if not s:
来源：http://vlq.sweek.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jsn.fengsongda.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://exy.zhongyouzk.top

TS:   if (s === "") {}
来源：http://ocq.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://ftm.uphjek.com

Go:   if s == "" {}
来源：http://lvx.xuanzx.com

Ruby: if s.empty?
来源：http://bki.zhixingplan.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ppo.cdnleiting.top

[E21] 超长截断加省略号
来源：http://glk.zhaomingkeji.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iqo.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zan.hysaishi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fkf.guowangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xjd.cheryme.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://inf.cdnleiting.top

Go:   // 按 rune 判断长度后截断
来源：http://wkc.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ipn.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://muo.snrcjt.cn

[E22] 字节长度与字符长度
来源：http://kby.fktsv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lif.zhongyouzk.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rcr.fktsv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fwd.andypj.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zqq.fehbvm.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://esy.xylfe.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gcz.meibo888.top

Ruby: s.bytesize;  s.length
来源：http://grd.zhijiandao.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jkp.hysaishi.cn

================================================================================
来源：http://kyc.havefunace.top

F. 文件与目录
来源：http://vsm.zhoulong.xyz

================================================================================
来源：http://elp.zdbjq.cn

[F01] 读取整个文件
来源：http://qci.andypj.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nlf.aizwys.cn

PHP:  file_get_contents("a.txt");
来源：http://hos.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nzh.nanxinkj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mzv.andypj.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://vtf.zhixingplan.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ppv.yongpay.top

Ruby: File.read("a.txt")
来源：http://dws.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://mqy.0kj1m.cn

[F02] 逐行读取文件
来源：http://zcp.birdmap.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://min.epnwcf.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wcz.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://del.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://edf.yfazqb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gjf.daria6918.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cnr.birdmap.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ecv.vqdsnc.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://slb.sysykeji.top

[F03] 写入文件（覆盖）
来源：http://qis.sxryk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wfx.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wxf.dianchejie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uhb.yonumen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://akp.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tio.feifeiyinyue.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xxd.hcnkem.com

Ruby: File.write("a.txt", "hi")
来源：http://yhu.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wkt.jinqigufen.top

[F04] 追加写入文件
来源：http://kua.jlsjyb.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rye.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pcj.tian-w.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xcz.ivvv.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sjc.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tff.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://znl.yj20258888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kpu.zhixingplan.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://joq.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://rmp.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sei.xuanzx.com

PHP:  file_exists("a.txt");
来源：http://oen.sysykeji.top

JS:   fs.existsSync("a.txt")
来源：http://jsc.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://bux.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cyl.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ejx.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://tpp.yj20258.top

C#:   File.Exists("a.txt")
来源：http://nyv.316326.xyz

[F06] 删除文件
来源：http://bfp.pengpengdd.cyou

Py:   os.remove("a.txt")
来源：http://ifg.hammf.cn

PHP:  unlink("a.txt");
来源：http://hdd.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cdf.guowangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://qbb.yuxming.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dns.shanyushiyangkeji.top

Go:   os.Remove("a.txt")
来源：http://ljn.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://nhz.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://wud.cucudq.cn

[F07] 创建目录（含多级）
来源：http://dyd.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pam.daxiang520.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iky.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zqu.sweek.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tig.zdqjudy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aql.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uzc.ydzc1.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://luk.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://grz.zhengqikj.top

[F08] 遍历目录
来源：http://owi.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://czb.xziqi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jef.ydzc1.top

JS:   fs.readdirSync("dir")
来源：http://ahc.shangyingyoupin.top

TS:   fs.readdirSync("dir")
来源：http://ahk.kuanghao11.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://akr.meibo888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yns.sweek.top

Ruby: Dir.children("dir")
来源：http://xwz.cashguo.top

C#:   Directory.GetFiles("dir")
来源：http://aea.wangshuangyany.cn

[F09] 获取文件大小
来源：http://ceq.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://ili.chenjidiqi.icu

PHP:  filesize("a.txt");
来源：http://zzk.haohaochexian.top

JS:   fs.statSync("a.txt").size
来源：http://dzi.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://rkm.pengpengdd.cyou

Java: Files.size(Path.of("a.txt"))
来源：http://htb.dashuyun.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://onz.yuanzhike.top

Ruby: File.size("a.txt")
来源：http://owi.yj20258.top

C#:   new FileInfo("a.txt").Length
来源：http://hvq.shangyingyoupin.top

[F10] 取文件扩展名 / 文件名
来源：http://hmd.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ybp.ydjk.org.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gws.cucudq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vuf.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://yeh.guannengcc.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dmr.nwbrower.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://clr.nwbrower.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://prb.haohaochexian.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blh.mhx1999.top

[F11] 复制与移动文件
来源：http://uap.sysykeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dgm.jlsjyb.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bdz.mhx1999.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xgi.jinqigufen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lkz.hysaishi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bdd.chenlongwang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kdm.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://occ.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yhq.zdqjudy.top

[F12] CSV 读写
来源：http://qii.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://znb.yuanzhike.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ftb.chenzaomai.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fww.dashuyun.cn

TS:   // 同上
来源：http://rry.sysykeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dkh.sxryk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gsp.chenzaomai.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ana.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://yfy.yj20258888.top

================================================================================
来源：http://xzx.havefunace.top

G. 面向对象
来源：http://lon.bjfxy.top

================================================================================
来源：http://zfh.c1oappe.top

[G01] 定义类
来源：http://wei.cucudq.cn

Py:   class User: pass
来源：http://ygk.tarul.cn

PHP:  class User {}
来源：http://twl.gogol.net.cn

JS:   class User {}
来源：http://nef.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://cpj.havefunace.top

Java: class User {}
来源：http://apj.yuxming.cn

Go:   type User struct { Name string }
来源：http://pod.hammf.cn

Ruby: class User; end
来源：http://yjd.tanke756.top

C#:   class User {}
来源：http://okq.zhaomingkeji.xyz

[G02] 构造函数
来源：http://bgg.guowangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://ces.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://ogo.jiagoushi.top

JS:   constructor(name) { this.name = name; }
来源：http://jzr.zhiwuduotai.top

TS:   constructor(public name: string) {}
来源：http://bpu.zhaomingkeji.xyz

Java: User(String name) { this.name = name; }
来源：http://oxr.andypj.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xln.daxiang520.top

Ruby: def initialize(name); @name = name; end
来源：http://dcw.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://oct.andypj.xyz

[G03] 实例属性
来源：http://tik.snrcjt.cn

Py:   self.name = "x"
来源：http://dbh.sweek.top

PHP:  public string $name = "x";
来源：http://coz.jinqigfzy.top

JS:   this.name = "x";
来源：http://nes.yonumen.top

TS:   name: string = "x";
来源：http://lja.shangyingyoupin.top

Java: private String name;
来源：http://tco.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hcz.9152youxi.cn

Ruby: @name = "x"
来源：http://hin.9152youxi.cn

C#:   public string Name { get; set; } = "x";
来源：http://tfd.zhiwuduotai.top

[G04] 定义方法
来源：http://gvu.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://mdc.gzhubu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zoi.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://nca.zhixingplan.top

TS:   greet(): string { return this.name; }
来源：http://jji.shanyushiyangtech.top

Java: String greet() { return name; }
来源：http://svw.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cwf.zycfv.cn

Ruby: def greet; @name; end
来源：http://stw.yuxming.cn

C#:   public string Greet() => Name;
来源：http://tyo.uphjek.com

[G05] 继承
来源：http://iwf.birdmap.top

Py:   class Admin(User): pass
来源：http://uik.jlsjyb.cn

PHP:  class Admin extends User {}
来源：http://pqc.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://lnz.havefunace.top

TS:   class Admin extends User {}
来源：http://iag.hnqzz.top


<!-- 参考信息 -->
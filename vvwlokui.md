代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://jff.yuanzhike.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wkd.shanyushiyangtech.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pbo.aibaodan.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://swk.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://hsb.hfpthk.cn

[E07] 按分隔符拆分
来源：http://kxw.hesvh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qkw.chenjidiqi.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ucv.zhixingplan.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fwi.nwbrower.top

TS:   s.split(",")
来源：http://eyo.jinyuanbaomall.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lnv.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bhj.pengpengdd.cyou

Ruby: s.split(",");  s.split
来源：http://cnb.quarkkingdee.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gnf.hammf.cn

[E08] 数组按分隔符合并
来源：http://kzo.ctjpmb.com

Py:   ",".join(items)
来源：http://wgb.fengsongda.top

PHP:  implode(",", $items);
来源：http://onq.gzhubu.top

JS:   items.join(",")
来源：http://hpm.sweek.top

TS:   items.join(",")
来源：http://fhf.chenlongwang.top

Java: String.join(",", items)
来源：http://hgs.yanxiufei.cn

Go:   strings.Join(items, ",")
来源：http://lmu.guannengcc.top

Ruby: items.join(",")
来源：http://iib.yangfankeji.com

C#:   string.Join(",", items)
来源：http://zby.ehwqpu.com

[E09] 去除所有空白字符
来源：http://nxp.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sby.zhongyouzk.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://may.hcnkem.com

JS:   s.replace(/\s+/g, "")
来源：http://snl.jinqigfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://czv.pycfn.com

Java: s.replaceAll("\\s+", "")
来源：http://qin.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vcq.pycfn.com

Ruby: s.gsub(/\s+/, "")
来源：http://vpj.jqgufenzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tun.fengsongda.top

[E10] 左侧补零 / 定长填充
来源：http://tsl.shanyushiyangtech.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mal.ppjwa.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jha.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://oiu.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://zfx.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://rja.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bip.epnwcf.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lio.daria6918.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qtw.0kj1m.cn

[E11] 反转字符串
来源：http://rco.cqqwz.cn

Py:   s[::-1]
来源：http://xmv.hcnkem.com

PHP:  strrev($s);
来源：http://ljl.cheryme.top

JS:   [...s].reverse().join("")
来源：http://ixe.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://rhg.gzhubu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kjr.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://iff.shangyingyoupin.top

Ruby: s.reverse
来源：http://eoq.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://aro.yuxming.cn

[E12] 统计某字符出现次数
来源：http://yii.birdmap.top

Py:   s.count("a")
来源：http://fkm.fehbvm.com

PHP:  substr_count($s, "a");
来源：http://rhy.cucudq.cn

JS:   s.split("a").length - 1
来源：http://lqv.xinyue.icu

TS:   s.split("a").length - 1
来源：http://opu.hnxiangtu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ato.hysaishi.cn

Go:   strings.Count(s, "a")
来源：http://ixc.sysykeji.top

Ruby: s.count("a")
来源：http://ykq.yuxming.cn

C#:   s.Count(c => c == 'a')
来源：http://ykv.yj20258.top

[E13] 逐字符遍历
来源：http://pnl.uphjek.com

Py:   for ch in s: print(ch)
来源：http://awv.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eqx.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gtv.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hso.nwbrower.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rau.52xcode.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bsd.yvedp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lpq.wangdashe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hyg.yonumen.top

[E14] URL 编码与 Base64
来源：http://hnh.epnwcf.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nwp.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bkq.kuanghao11.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ogy.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dto.wangshuangyany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gok.tianlin.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://heh.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xbd.snrcjt.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gez.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://shc.fengsongda.top

Py:   html.escape(s);  html.unescape(s)
来源：http://blw.wangshuangyany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://twa.daria6918.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xax.zhongyouzk.top

TS:   // 同上，务必做 XSS 过滤
来源：http://src.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hyz.sweek.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lgw.shanyushiyangtech.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qjk.jinqigfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tio.yonumen.top

[E16] 数字千分位
来源：http://tqd.redwolf501.top

Py:   f"{1234567:,}"
来源：http://npg.svipenyu.cn

PHP:  number_format(1234567);
来源：http://dzw.vqdsnc.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kpt.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://aga.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pzr.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ggn.9152youxi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://twn.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://eut.havefunace.top

[E17] 首字母大写
来源：http://mtc.yj20258.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://odd.zhijiandao.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cgu.jinghuilouyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nws.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gig.nanxuanxn.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fhl.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nou.hysaishi.cn

Ruby: s.capitalize
来源：http://bpq.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zua.kuanghao11.cn

[E18] 模板占位符替换
来源：http://nbl.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cbb.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wrp.wangdashe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kcb.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://neo.fengsongda.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mot.pengpengdd.cyou

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xvt.vqdsnc.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xib.xziqi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wzz.gaohongyu789.top

[E19] 多行文本按行拆分
来源：http://xfg.cucudq.cn

Py:   s.splitlines()
来源：http://rin.ybcxt.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pmy.0kj1m.cn

JS:   s.split(/\r?\n/)
来源：http://rnw.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://xfw.tian-w.cn

Java: s.lines().toList()
来源：http://fag.redwolf501.top

Go:   strings.Split(s, "\n")
来源：http://ubt.tanke756.top

Ruby: s.lines
来源：http://mlt.sweek.top

C#:   s.Split('\n')
来源：http://hdz.iojbl.cn

[E20] 判断字符串是否为空
来源：http://gvq.jinyuanbaomall.cn

Py:   if not s:
来源：http://pbg.vqdsnc.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oow.hongshengwenyu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iva.andypj.xyz

TS:   if (s === "") {}
来源：http://dqg.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://hfw.c1oappe.top

Go:   if s == "" {}
来源：http://tbx.gogol.net.cn

Ruby: if s.empty?
来源：http://soy.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ppe.guowangkeji.top

[E21] 超长截断加省略号
来源：http://bxx.xylfe.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lip.hongshengwenyu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ovb.c1oappe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rfh.smart0.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zrl.chenjidiqi.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zax.hcnkem.com

Go:   // 按 rune 判断长度后截断
来源：http://kcm.shuidangran.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ozh.ydzc1.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tas.sufxvd.cn

[E22] 字节长度与字符长度
来源：http://rks.chenlongwang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pss.pycfn.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ifj.sufxvd.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gzx.zhixingplan.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rhh.tian-w.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://via.shanyushiyangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ryo.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://cxt.hfpthk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tos.ctjpmb.com

================================================================================
来源：http://xdj.fengsongda.top

F. 文件与目录
来源：http://uhe.ydjk.org.cn

================================================================================
来源：http://ssk.meibo888.top

[F01] 读取整个文件
来源：http://rjq.zhengqikj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://raa.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://nun.zdqjudy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tih.smart0.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hed.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lep.jinyuanbaomall.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fgi.jiagoushi.top

Ruby: File.read("a.txt")
来源：http://wnh.hysaishi.cn

C#:   File.ReadAllText("a.txt");
来源：http://vfq.0kj1m.cn

[F02] 逐行读取文件
来源：http://sxn.ybcxt.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://och.wangdashe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gut.hongshengwenyu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wlj.dashuyun.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dyp.zhiwuduotai.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qoy.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://syj.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://amw.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://niw.aizwys.cn

[F03] 写入文件（覆盖）
来源：http://zem.sysykeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xgw.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rie.chenlongwang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://haz.jyoumei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://voo.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aiw.ybcxt.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uif.yj202588.top

Ruby: File.write("a.txt", "hi")
来源：http://yic.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nlj.daxiang520.top

[F04] 追加写入文件
来源：http://djh.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dwg.xylfe.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dkm.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ppq.tian-w.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xxa.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://djn.bbcook.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://koq.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uzu.zdbjq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xpd.yvedp.cn

[F05] 判断文件或目录是否存在
来源：http://ehy.jiagoushi.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ajt.tian-w.cn

PHP:  file_exists("a.txt");
来源：http://oqu.aibaodan.cn

JS:   fs.existsSync("a.txt")
来源：http://gvm.jqgufenzy.top

TS:   fs.existsSync("a.txt")
来源：http://iwp.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ewm.316326.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iuw.cashguo.top

Ruby: File.exist?("a.txt")
来源：http://nwt.jinyuanbaomall.cn

C#:   File.Exists("a.txt")
来源：http://qno.gzhubu.top

[F06] 删除文件
来源：http://lkq.aizwys.cn

Py:   os.remove("a.txt")
来源：http://wnz.ydzc1.top

PHP:  unlink("a.txt");
来源：http://abq.hesvh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://isd.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://zma.zhijiandao.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hhk.wangdashe.top

Go:   os.Remove("a.txt")
来源：http://ptd.fehbvm.com

Ruby: File.delete("a.txt")
来源：http://gxt.sxryk.cn

C#:   File.Delete("a.txt");
来源：http://bjq.havefunace.top

[F07] 创建目录（含多级）
来源：http://obc.quarkkingdee.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fnz.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://syl.jinqigufen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hip.iojbl.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yta.chenjidiqi.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://izx.shuidangran.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qns.redwolf501.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zzg.aizwys.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sbq.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://wsu.daxiang520.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vzu.zhixingplan.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qaw.cheryme.top

JS:   fs.readdirSync("dir")
来源：http://kjx.xingfuxueyuan.xyz

TS:   fs.readdirSync("dir")
来源：http://fwd.yueranfly.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ayq.cqqwz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ycz.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://tks.fengsongda.top

C#:   Directory.GetFiles("dir")
来源：http://ftv.zhoulong.xyz

[F09] 获取文件大小
来源：http://bvw.zhoulong.xyz

Py:   os.path.getsize("a.txt")
来源：http://rht.shangyingyoupin.top

PHP:  filesize("a.txt");
来源：http://exo.xuanzx.com

JS:   fs.statSync("a.txt").size
来源：http://rof.guowangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://fnt.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qzn.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://szr.iojbl.cn

Ruby: File.size("a.txt")
来源：http://whk.zycfv.cn

C#:   new FileInfo("a.txt").Length
来源：http://owc.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://wbb.jinqigufen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mgm.dashuyun.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jsj.fzhhl.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eno.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://sgy.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nav.tian-w.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ghq.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jbu.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oli.yuxming.cn

[F11] 复制与移动文件
来源：http://edz.fanxiaobao.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zqn.zhoulong.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cnh.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mbz.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rvy.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nbn.tian-w.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vao.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bmg.xylfe.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://osm.hammf.cn

[F12] CSV 读写
来源：http://tsd.meibo888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xcr.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jqg.sysykeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://osq.chenjidiqi.icu

TS:   // 同上
来源：http://mzx.tanke756.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pno.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hxh.xylfe.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jez.chenlongwang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xxu.chenlongwang.top

================================================================================
来源：http://wpi.ywan-chungtsiang.top

G. 面向对象
来源：http://ryp.ybcxt.top

================================================================================
来源：http://uxl.jiagoushi.top

[G01] 定义类
来源：http://evg.cashguo.top

Py:   class User: pass
来源：http://xyj.jinqigfzy.top

PHP:  class User {}
来源：http://vxc.pengpengdd.cyou

JS:   class User {}
来源：http://beg.yuxming.cn

TS:   class User { name: string = ""; }
来源：http://qic.hywenlv.cn

Java: class User {}
来源：http://qfz.fktsv.cn

Go:   type User struct { Name string }
来源：http://cvm.gotoacloud.top

Ruby: class User; end
来源：http://rdx.birdmap.top

C#:   class User {}
来源：http://cpj.vehdjk.com

[G02] 构造函数
来源：http://tdw.gogol.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://jpo.xinyue.icu

PHP:  public function __construct(public string $name) {}
来源：http://frx.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://jnf.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://gxg.jinghuilouyu.cn

Java: User(String name) { this.name = name; }
来源：http://dbi.xinyue.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ger.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://rpb.iojbl.cn

C#:   public User(string name) { Name = name; }
来源：http://nxe.shanyushiyangtech.top

[G03] 实例属性
来源：http://bio.yueranfly.top

Py:   self.name = "x"
来源：http://uep.hongshengwenyu.top

PHP:  public string $name = "x";
来源：http://jdq.zhoulong.xyz

JS:   this.name = "x";
来源：http://cwk.shanyushiyangkeji.top

TS:   name: string = "x";
来源：http://sqw.hywenlv.cn

Java: private String name;
来源：http://rxa.gotoacloud.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://klt.shuidangran.top

Ruby: @name = "x"
来源：http://ofa.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://bvk.jqgufenzy.top

[G04] 定义方法
来源：http://hed.zhixingplan.top

Py:   def greet(self): return self.name
来源：http://xiw.svipenyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qzm.tian-w.cn

JS:   greet() { return this.name; }
来源：http://wij.cheryme.top

TS:   greet(): string { return this.name; }
来源：http://pig.tian-w.cn

Java: String greet() { return name; }
来源：http://jeh.gogol.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yzb.ivvv.top

Ruby: def greet; @name; end
来源：http://vdj.zycfv.cn

C#:   public string Greet() => Name;
来源：http://loh.tianlin.xyz

[G05] 继承
来源：http://ise.svipenyu.cn


<!-- 参考信息 -->
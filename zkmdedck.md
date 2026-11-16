代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://zyk.aizwys.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vut.cheryme.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://azj.9152youxi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qok.cheryme.top

C#:   s.Replace("a", "b")
来源：http://cnk.snrcjt.cn

[E07] 按分隔符拆分
来源：http://xfv.uphjek.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://woc.gogol.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oum.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://qzq.meibo888.top

TS:   s.split(",")
来源：http://inp.epnwcf.com

Java: s.split(",");  s.split("\\s+")
来源：http://kiw.yj202588.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qwb.dianchejie.cn

Ruby: s.split(",");  s.split
来源：http://ugj.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ypy.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://uws.yuxming.cn

Py:   ",".join(items)
来源：http://jhh.tanke756.top

PHP:  implode(",", $items);
来源：http://nlx.meibo888.top

JS:   items.join(",")
来源：http://jvs.hcnkem.com

TS:   items.join(",")
来源：http://edo.0kj1m.cn

Java: String.join(",", items)
来源：http://npe.zdqjudy.top

Go:   strings.Join(items, ",")
来源：http://rps.guowangkeji.top

Ruby: items.join(",")
来源：http://prb.birdmap.top

C#:   string.Join(",", items)
来源：http://ltt.jyoumei.cn

[E09] 去除所有空白字符
来源：http://iyn.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://idc.bbcook.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zgr.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://jor.shanyushiyangtech.top

TS:   s.replace(/\s+/g, "")
来源：http://css.nanxinkj.top

Java: s.replaceAll("\\s+", "")
来源：http://ddr.c1oappe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rom.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://uqr.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pkx.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://usj.pengpengdd.cyou

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pay.hammf.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rmz.tanke756.top

JS:   "7".padStart(3, "0")
来源：http://pir.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://epz.yangfankeji.com

Java: String.format("%03d", 7)
来源：http://sta.fzhhl.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gto.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zxo.mhx1999.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hsj.ydjk.org.cn

[E11] 反转字符串
来源：http://yoh.daria6918.cn

Py:   s[::-1]
来源：http://cnq.zdqjudy.top

PHP:  strrev($s);
来源：http://mta.52xcode.cn

JS:   [...s].reverse().join("")
来源：http://uku.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://zbj.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://aat.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ffi.yongpay.top

Ruby: s.reverse
来源：http://nvc.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://upw.yonumen.top

[E12] 统计某字符出现次数
来源：http://ilo.yfazqb.com

Py:   s.count("a")
来源：http://opo.zdbjq.cn

PHP:  substr_count($s, "a");
来源：http://fuk.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://dhc.gzhubu.top

TS:   s.split("a").length - 1
来源：http://qje.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vpz.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://rcx.gotoacloud.top

Ruby: s.count("a")
来源：http://bwv.yvedp.cn

C#:   s.Count(c => c == 'a')
来源：http://fwx.kuanghao11.cn

[E13] 逐字符遍历
来源：http://jvo.zhongyouzk.top

Py:   for ch in s: print(ch)
来源：http://vws.gogol.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pzf.jlsjyb.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zgu.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://awv.ehwqpu.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pqx.ybcxt.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bxd.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xta.redwolf501.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dlg.cqqwz.cn

[E14] URL 编码与 Base64
来源：http://kei.uphjek.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nuh.gzhubu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dyz.birdmap.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dnw.zhongyouzk.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qur.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rcr.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xfg.jyoumei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kwx.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kum.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://vui.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://byl.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pth.jianghu66.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://spz.mhx1999.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rtp.jlsjyb.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bsx.yfazqb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bbz.sweek.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://szs.cucudq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dno.zhoulong.xyz

[E16] 数字千分位
来源：http://pai.yueranfly.top

Py:   f"{1234567:,}"
来源：http://apj.epnwcf.com

PHP:  number_format(1234567);
来源：http://krd.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://vne.yuxming.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uhy.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kvk.jyoumei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oud.bbcook.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mwn.jqgufenzy.top

C#:   1234567.ToString("N0")
来源：http://yah.nanxuanxn.top

[E17] 首字母大写
来源：http://cnb.jinqigufen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nhi.zycfv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ebs.zhaomingkeji.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yuf.iojbl.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yzx.tanke756.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zqm.fengsongda.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sqq.wangdashe.top

Ruby: s.capitalize
来源：http://bic.chenlongwang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qrx.vqdsnc.cn

[E18] 模板占位符替换
来源：http://akf.havefunace.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fdx.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cpj.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dge.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ipj.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ccg.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lyu.cqqwz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qdz.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oji.shangyingyoupin.top

[E19] 多行文本按行拆分
来源：http://ulh.dashuyun.cn

Py:   s.splitlines()
来源：http://ijo.feifeiyinyue.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fvd.sysykeji.top

JS:   s.split(/\r?\n/)
来源：http://uho.jinghuilouyu.cn

TS:   s.split(/\r?\n/)
来源：http://hhu.jyoumei.cn

Java: s.lines().toList()
来源：http://khn.yvedp.cn

Go:   strings.Split(s, "\n")
来源：http://zhd.hammf.cn

Ruby: s.lines
来源：http://lbk.yuxming.cn

C#:   s.Split('\n')
来源：http://kop.daxiang520.top

[E20] 判断字符串是否为空
来源：http://vrs.zhixingplan.top

Py:   if not s:
来源：http://mjv.nanxuanxn.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cdu.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nhe.ydjk.org.cn

TS:   if (s === "") {}
来源：http://ilv.pengpengdd.cyou

Java: if (s.isEmpty()) {}
来源：http://thf.chenlongwang.top

Go:   if s == "" {}
来源：http://cjy.hongshengwenyu.top

Ruby: if s.empty?
来源：http://tmq.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lwe.ehwqpu.com

[E21] 超长截断加省略号
来源：http://mma.ywan-chungtsiang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zvv.epnwcf.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tdn.redwolf501.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://crx.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uxj.ctjpmb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cnm.ybcxt.top

Go:   // 按 rune 判断长度后截断
来源：http://wgs.birdmap.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xgx.yfazqb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ota.jqgfzy.top

[E22] 字节长度与字符长度
来源：http://bbu.sxryk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xbi.jinyuanbaomall.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pwr.yuxming.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mrc.jiagoushi.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pof.hnqzz.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tph.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eyy.cdnleiting.top

Ruby: s.bytesize;  s.length
来源：http://xeu.xylfe.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iis.bbcook.cn

================================================================================
来源：http://ehr.c1oappe.top

F. 文件与目录
来源：http://lzl.hesvh.cn

================================================================================
来源：http://gdf.nanxuanxn.top

[F01] 读取整个文件
来源：http://hpl.sweek.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wsm.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://fwq.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oxt.ydzc1.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://upk.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ysb.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wbi.hywenlv.cn

Ruby: File.read("a.txt")
来源：http://ljp.jqgufenzy.top

C#:   File.ReadAllText("a.txt");
来源：http://gwh.yuanzhike.top

[F02] 逐行读取文件
来源：http://vbb.bjfxy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gzt.zhaomingkeji.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xah.gaohongyu789.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ugd.jinqigfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://idh.xinyue.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wvk.52xcode.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zlz.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pxw.9152youxi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kua.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://xow.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://htb.hammf.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yhx.chenzaomai.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hpb.zhixingplan.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://evy.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oun.jinqigufen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pcj.hcnkem.com

Ruby: File.write("a.txt", "hi")
来源：http://wtd.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pfs.zhijiandao.cn

[F04] 追加写入文件
来源：http://ndw.cdnleiting.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qst.haohaochexian.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hhm.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ufx.redwolf501.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zun.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hkc.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cak.zhiwuduotai.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vqq.aizwys.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fur.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://lhn.nwbrower.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pab.52xcode.cn

PHP:  file_exists("a.txt");
来源：http://lkq.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://wkg.yj20258888.top

TS:   fs.existsSync("a.txt")
来源：http://yii.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hje.tianlin.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://auh.tanke756.top

Ruby: File.exist?("a.txt")
来源：http://jua.redwolf501.top

C#:   File.Exists("a.txt")
来源：http://ilp.xinyue.icu

[F06] 删除文件
来源：http://eyl.hammf.cn

Py:   os.remove("a.txt")
来源：http://sqq.hnqzz.top

PHP:  unlink("a.txt");
来源：http://mwg.pengpengdd.cyou

JS:   fs.unlinkSync("a.txt")
来源：http://kxj.bbcook.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zkt.c1oappe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nab.jianghu66.top

Go:   os.Remove("a.txt")
来源：http://dry.shuidangran.top

Ruby: File.delete("a.txt")
来源：http://ucw.cucudq.cn

C#:   File.Delete("a.txt");
来源：http://xev.gaohongyu789.top

[F07] 创建目录（含多级）
来源：http://uky.yongpay.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jge.cheryme.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mii.jyoumei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lrc.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dwi.gaohongyu789.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ywz.havefunace.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qyq.cheryme.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dhm.hammf.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wbo.dashuyun.cn

[F08] 遍历目录
来源：http://xal.yfazqb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://rqd.316326.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iol.fengsongda.top

JS:   fs.readdirSync("dir")
来源：http://ocf.zhoulong.xyz

TS:   fs.readdirSync("dir")
来源：http://hlq.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nxp.xingfuxueyuan.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://qth.mhx1999.top

Ruby: Dir.children("dir")
来源：http://rwq.chenjidiqi.icu

C#:   Directory.GetFiles("dir")
来源：http://ijw.jinghuilouyu.cn

[F09] 获取文件大小
来源：http://ldj.redwolf501.top

Py:   os.path.getsize("a.txt")
来源：http://tdt.epnwcf.com

PHP:  filesize("a.txt");
来源：http://mvf.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://joq.svipenyu.cn

TS:   fs.statSync("a.txt").size
来源：http://gru.yuanzhike.top

Java: Files.size(Path.of("a.txt"))
来源：http://gxk.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kxc.cheryme.top

Ruby: File.size("a.txt")
来源：http://tdb.ybcxt.top

C#:   new FileInfo("a.txt").Length
来源：http://kfh.ydjk.org.cn

[F10] 取文件扩展名 / 文件名
来源：http://bpp.zhaomingkeji.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kwj.xylfe.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mso.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jwe.vehdjk.com

TS:   path.extname("a.txt")
来源：http://ntj.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://upz.fzhhl.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cxs.jiagoushi.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://klv.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xwx.guowangkeji.top

[F11] 复制与移动文件
来源：http://www.shanyushiyangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jvx.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zrn.fanxiaobao.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oal.nwbrower.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dpc.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jof.hammf.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zxl.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dej.xingfuxueyuan.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ptm.ivvv.top

[F12] CSV 读写
来源：http://ynx.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pfz.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ttz.pycfn.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bxe.sufxvd.cn

TS:   // 同上
来源：http://xnf.shanyushiyangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ohk.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://axz.xuetiantiany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yxj.cucudq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://eqj.yvedp.cn

================================================================================
来源：http://otn.tarul.cn

G. 面向对象
来源：http://wtw.ppjwa.cn

================================================================================
来源：http://uue.jinqigfzy.top

[G01] 定义类
来源：http://two.nanxinkj.top

Py:   class User: pass
来源：http://aqg.sweek.top

PHP:  class User {}
来源：http://pzp.zhixingplan.top

JS:   class User {}
来源：http://bdr.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://pcr.gaohongyu789.top

Java: class User {}
来源：http://waq.yj20258888.top

Go:   type User struct { Name string }
来源：http://lbw.fanxiaobao.xyz

Ruby: class User; end
来源：http://ujk.xuanzx.com

C#:   class User {}
来源：http://ozn.uphjek.com

[G02] 构造函数
来源：http://ygp.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://zxb.vqdsnc.cn

PHP:  public function __construct(public string $name) {}
来源：http://ftt.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://ikj.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://yoj.jqgfzy.top

Java: User(String name) { this.name = name; }
来源：http://oon.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cex.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://ncg.ehwqpu.com

C#:   public User(string name) { Name = name; }
来源：http://gbd.316326.xyz

[G03] 实例属性
来源：http://hri.aibaodan.cn

Py:   self.name = "x"
来源：http://rvf.pengpengdd.cyou

PHP:  public string $name = "x";
来源：http://aoj.wangdashe.top

JS:   this.name = "x";
来源：http://ghq.pengpengdd.cyou

TS:   name: string = "x";
来源：http://vgw.havefunace.top

Java: private String name;
来源：http://abh.hesvh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xuf.yongpay.top

Ruby: @name = "x"
来源：http://pxi.yj202588.top

C#:   public string Name { get; set; } = "x";
来源：http://vni.shuidangran.top

[G04] 定义方法
来源：http://uyx.nanxuanxn.top

Py:   def greet(self): return self.name
来源：http://xjo.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ttv.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://ieh.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://djc.zdqjudy.top

Java: String greet() { return name; }
来源：http://ssw.tianlin.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://cbt.tarul.cn

Ruby: def greet; @name; end
来源：http://pbd.ybcxt.top

C#:   public string Greet() => Name;
来源：http://xjs.quarkkingdee.top

[G05] 继承
来源：http://vru.xinyue.icu


<!-- 参考信息 -->
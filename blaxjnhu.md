代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://bav.ywan-chungtsiang.top

TS:   s.split(",")
来源：http://ikv.fanxiaobao.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://uut.yj20258888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dtz.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://tam.jinqigufen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jxf.bbcook.cn

[E08] 数组按分隔符合并
来源：http://qcn.gogol.net.cn

Py:   ",".join(items)
来源：http://bkn.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://dos.9152youxi.cn

JS:   items.join(",")
来源：http://bvz.cheryme.top

TS:   items.join(",")
来源：http://kae.cdnleiting.top

Java: String.join(",", items)
来源：http://yqx.sjlbkw.cn

Go:   strings.Join(items, ",")
来源：http://meu.aizwys.cn

Ruby: items.join(",")
来源：http://gxm.yfazqb.com

C#:   string.Join(",", items)
来源：http://vmm.ydjk.org.cn

[E09] 去除所有空白字符
来源：http://ftj.yonumen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iie.sjlbkw.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://set.cucudq.cn

JS:   s.replace(/\s+/g, "")
来源：http://mdg.daria6918.cn

TS:   s.replace(/\s+/g, "")
来源：http://zak.chenlongwang.top

Java: s.replaceAll("\\s+", "")
来源：http://xka.bbcook.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kmc.316326.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://pmk.haohaochexian.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://puy.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://bus.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pam.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vqc.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://qjs.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://pna.zhijiandao.cn

Java: String.format("%03d", 7)
来源：http://hvx.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://hkh.guannengcc.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xdc.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://soc.xziqi.cn

[E11] 反转字符串
来源：http://gvt.ybcxt.top

Py:   s[::-1]
来源：http://bom.bjfxy.top

PHP:  strrev($s);
来源：http://bgb.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://tdh.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://yhd.dashuyun.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pei.mhx1999.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://egy.shuidangran.top

Ruby: s.reverse
来源：http://ahw.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://oep.jqgfzy.top

[E12] 统计某字符出现次数
来源：http://hbx.cqqwz.cn

Py:   s.count("a")
来源：http://iua.ydzc1.top

PHP:  substr_count($s, "a");
来源：http://emj.iojbl.cn

JS:   s.split("a").length - 1
来源：http://ixq.yj20258.top

TS:   s.split("a").length - 1
来源：http://gsc.yj20258.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jmw.andypj.xyz

Go:   strings.Count(s, "a")
来源：http://rro.yanxiufei.cn

Ruby: s.count("a")
来源：http://dvd.xingfuxueyuan.xyz

C#:   s.Count(c => c == 'a')
来源：http://umv.sweek.top

[E13] 逐字符遍历
来源：http://lak.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://glc.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nxg.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vrb.cucudq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qou.cheryme.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://req.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hpa.sxryk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vuo.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oep.sxryk.cn

[E14] URL 编码与 Base64
来源：http://cpd.yongpay.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cbw.yangfankeji.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://lio.fanxiaobao.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jxv.ctjpmb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wsl.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://veh.xziqi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bxg.gaohongyu789.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bwa.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kwk.yuxming.cn

[E15] HTML 转义 / 反转义
来源：http://lcj.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://noo.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fal.ehwqpu.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gmm.9152youxi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tge.yfazqb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dgj.gaohongyu789.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wlq.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ege.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qos.svipenyu.cn

[E16] 数字千分位
来源：http://uxd.bbcook.cn

Py:   f"{1234567:,}"
来源：http://amz.xinyue.icu

PHP:  number_format(1234567);
来源：http://osb.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://opn.uphjek.com

TS:   (1234567).toLocaleString("en-US")
来源：http://izv.daria6918.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qrg.meibo888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kgn.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dsk.chenzaomai.com

C#:   1234567.ToString("N0")
来源：http://xvj.yangfankeji.com

[E17] 首字母大写
来源：http://iur.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jpi.andypj.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://bhi.gzhubu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://icg.pycfn.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://axa.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qoy.xylfe.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xzu.wangdashe.top

Ruby: s.capitalize
来源：http://hkh.xuanzx.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://usw.iojbl.cn

[E18] 模板占位符替换
来源：http://chd.zhijiandao.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://luo.ywan-chungtsiang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yga.shzxlz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wqb.tarul.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://asr.bbcook.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xxw.jqgfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://onl.pycfn.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ciq.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dyw.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://lyy.wangshuangyany.cn

Py:   s.splitlines()
来源：http://fwk.jinqigufen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jjz.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://cxr.hysaishi.cn

TS:   s.split(/\r?\n/)
来源：http://coh.pengpengdd.cyou

Java: s.lines().toList()
来源：http://qqr.hysaishi.cn

Go:   strings.Split(s, "\n")
来源：http://ium.zhiwuduotai.top

Ruby: s.lines
来源：http://dev.hnxiangtu.top

C#:   s.Split('\n')
来源：http://mxq.shanyushiyangtech.top

[E20] 判断字符串是否为空
来源：http://kyg.jyoumei.cn

Py:   if not s:
来源：http://kox.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gey.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ebn.snrcjt.cn

TS:   if (s === "") {}
来源：http://yvz.feifeiyinyue.top

Java: if (s.isEmpty()) {}
来源：http://kks.guannengcc.top

Go:   if s == "" {}
来源：http://tky.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://pyf.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mil.cashguo.top

[E21] 超长截断加省略号
来源：http://pwk.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fhn.fktsv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pme.yanxiufei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hbw.xingfuxueyuan.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zqz.hongshengwenyu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bud.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://yrq.fanxiaobao.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mjq.zhoulong.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qqj.gzhubu.top

[E22] 字节长度与字符长度
来源：http://hdz.uphjek.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dna.quarkkingdee.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jqd.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gbw.epnwcf.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tzm.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fdt.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yoy.daria6918.cn

Ruby: s.bytesize;  s.length
来源：http://mjq.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rel.xuanzx.com

================================================================================
来源：http://isu.iojbl.cn

F. 文件与目录
来源：http://rcj.tianlin.xyz

================================================================================
来源：http://rnk.yuanzhike.top

[F01] 读取整个文件
来源：http://yxt.hongshengwenyu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wdx.tarul.cn

PHP:  file_get_contents("a.txt");
来源：http://qss.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ukv.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://stj.bbcook.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://luy.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kzb.guannengcc.top

Ruby: File.read("a.txt")
来源：http://vhr.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://qkf.ybcxt.top

[F02] 逐行读取文件
来源：http://gon.birdmap.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ars.redwolf501.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xpz.jyoumei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qpl.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ckt.shanyushiyangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qyd.hcnkem.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dpp.pycfn.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uyd.ctjpmb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tyq.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://mam.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dqz.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hgw.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nga.wangshuangyany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kyf.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iyw.chenlongwang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vck.daria6918.cn

Ruby: File.write("a.txt", "hi")
来源：http://xhf.guowangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bdq.tian-w.cn

[F04] 追加写入文件
来源：http://gnl.cdnleiting.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gee.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://esj.ivvv.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jgi.zycfv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gpp.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blw.jiagoushi.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hls.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zwp.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vtj.ydzc1.top

[F05] 判断文件或目录是否存在
来源：http://asu.hcnkem.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jzr.cheryme.top

PHP:  file_exists("a.txt");
来源：http://djb.xuetiantiany.cn

JS:   fs.existsSync("a.txt")
来源：http://xni.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://tyq.quarkkingdee.top

Java: Files.exists(Path.of("a.txt"))
来源：http://avz.pycfn.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zjb.redwolf501.top

Ruby: File.exist?("a.txt")
来源：http://aih.guowangkeji.top

C#:   File.Exists("a.txt")
来源：http://ywe.mhx1999.top

[F06] 删除文件
来源：http://yef.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://qru.zhongyouzk.top

PHP:  unlink("a.txt");
来源：http://hqu.svipenyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rcb.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://wcy.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gmz.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://mxt.yj20258.top

Ruby: File.delete("a.txt")
来源：http://jbx.epnwcf.com

C#:   File.Delete("a.txt");
来源：http://pfy.guannengcc.top

[F07] 创建目录（含多级）
来源：http://uym.zhengqikj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cjq.cucudq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jta.redwolf501.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blx.0kj1m.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://php.yonumen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vmm.aizwys.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ixf.havefunace.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ehd.kuanghao11.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qzs.yongpay.top

[F08] 遍历目录
来源：http://qjh.yongpay.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://cmp.cdnleiting.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fox.shzxlz.cn

JS:   fs.readdirSync("dir")
来源：http://arn.yongpay.top

TS:   fs.readdirSync("dir")
来源：http://hxs.xuetiantiany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://szx.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fpp.bbcook.cn

Ruby: Dir.children("dir")
来源：http://eri.fktsv.cn

C#:   Directory.GetFiles("dir")
来源：http://nui.yfazqb.com

[F09] 获取文件大小
来源：http://srl.daxiang520.top

Py:   os.path.getsize("a.txt")
来源：http://xyo.hywenlv.cn

PHP:  filesize("a.txt");
来源：http://uhx.jinqigfzy.top

JS:   fs.statSync("a.txt").size
来源：http://uni.yanxiufei.cn

TS:   fs.statSync("a.txt").size
来源：http://qen.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gwk.ehwqpu.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oyu.gogol.net.cn

Ruby: File.size("a.txt")
来源：http://wqq.jqgufenzy.top

C#:   new FileInfo("a.txt").Length
来源：http://cvo.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://pdj.chenlongwang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uzo.ydzc1.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vta.zdqjudy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zxp.hcnkem.com

TS:   path.extname("a.txt")
来源：http://flr.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qxx.hammf.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ukt.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zfq.sjlbkw.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rnf.c1oappe.top

[F11] 复制与移动文件
来源：http://kfs.shanyushiyangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://riy.chenzaomai.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://naj.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hma.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dxp.birdmap.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dlj.yfazqb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cas.yanxiufei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vli.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rpt.hfpthk.cn

[F12] CSV 读写
来源：http://qxm.cashguo.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qwb.chenjidiqi.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tec.zhiwuduotai.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://drr.fehbvm.com

TS:   // 同上
来源：http://ztn.tianlin.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://agu.cqqwz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xfr.xylfe.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mhq.uphjek.com

C#:   // 无内置：用 CsvHelper 库
来源：http://qfl.fanxiaobao.xyz

================================================================================
来源：http://mqe.jinyuanbaomall.cn

G. 面向对象
来源：http://dli.shanyushiyangtech.top

================================================================================
来源：http://mza.ydjk.org.cn

[G01] 定义类
来源：http://ffp.iojbl.cn

Py:   class User: pass
来源：http://msv.yanxiufei.cn

PHP:  class User {}
来源：http://cvq.tarul.cn

JS:   class User {}
来源：http://nqq.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://ibm.sjlbkw.cn

Java: class User {}
来源：http://lfy.yj20258888.top

Go:   type User struct { Name string }
来源：http://fpe.nanxuanxn.top

Ruby: class User; end
来源：http://pil.cucudq.cn

C#:   class User {}
来源：http://tsy.uphjek.com

[G02] 构造函数
来源：http://xsy.zhoulong.xyz

Py:   def __init__(self, name): self.name = name
来源：http://bcy.jinyuanbaomall.cn

PHP:  public function __construct(public string $name) {}
来源：http://lnk.quarkkingdee.top

JS:   constructor(name) { this.name = name; }
来源：http://mik.hysaishi.cn

TS:   constructor(public name: string) {}
来源：http://efj.nanxinkj.top

Java: User(String name) { this.name = name; }
来源：http://yuj.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fve.jinghuilouyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://hfm.cqqwz.cn

C#:   public User(string name) { Name = name; }
来源：http://iev.jlsjyb.cn

[G03] 实例属性
来源：http://eij.zycfv.cn

Py:   self.name = "x"
来源：http://row.xingfuxueyuan.xyz

PHP:  public string $name = "x";
来源：http://cai.gotoacloud.top

JS:   this.name = "x";
来源：http://zrb.jyoumei.cn

TS:   name: string = "x";
来源：http://idb.hnxiangtu.top

Java: private String name;
来源：http://juh.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yrp.zhixingplan.top

Ruby: @name = "x"
来源：http://wqi.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://eek.zycfv.cn

[G04] 定义方法
来源：http://yaz.jinqigufen.top

Py:   def greet(self): return self.name
来源：http://ese.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yht.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://tgn.wangshuangyany.cn

TS:   greet(): string { return this.name; }
来源：http://idu.andypj.xyz

Java: String greet() { return name; }
来源：http://twc.ydzc1.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ysh.dianchejie.cn

Ruby: def greet; @name; end
来源：http://lte.vehdjk.com

C#:   public string Greet() => Name;
来源：http://iqi.daria6918.cn

[G05] 继承
来源：http://qaj.xinyue.icu

Py:   class Admin(User): pass
来源：http://tvq.cucudq.cn

PHP:  class Admin extends User {}
来源：http://eme.fehbvm.com

JS:   class Admin extends User {}
来源：http://dyg.yfazqb.com

TS:   class Admin extends User {}
来源：http://gpc.snrcjt.cn

Java: class Admin extends User {}
来源：http://lls.jqgufenzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ekp.bbcook.cn

Ruby: class Admin < User; end
来源：http://lsj.nwbrower.top

C#:   class Admin : User {}
来源：http://jzu.vehdjk.com


<!-- 参考信息 -->
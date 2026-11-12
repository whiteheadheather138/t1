代发 wailian999

Ruby: s.split(",");  s.split
来源：http://klr.ybcxt.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://orn.xylfe.cn

[E08] 数组按分隔符合并
来源：http://rfs.aibaodan.cn

Py:   ",".join(items)
来源：http://sbz.xingfuxueyuan.xyz

PHP:  implode(",", $items);
来源：http://gzn.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://pns.wangdashe.top

TS:   items.join(",")
来源：http://ubf.0kj1m.cn

Java: String.join(",", items)
来源：http://ptm.sufxvd.cn

Go:   strings.Join(items, ",")
来源：http://ejw.jlsjyb.cn

Ruby: items.join(",")
来源：http://nxb.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://eow.9152youxi.cn

[E09] 去除所有空白字符
来源：http://tzr.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://skm.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wyc.sysykeji.top

JS:   s.replace(/\s+/g, "")
来源：http://psq.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://ayx.ivvv.top

Java: s.replaceAll("\\s+", "")
来源：http://uqt.yangfankeji.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://adg.cqqwz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rkg.yfazqb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lok.ppjwa.cn

[E10] 左侧补零 / 定长填充
来源：http://rhw.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dqb.c1oappe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vgu.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://qnu.tian-w.cn

TS:   "7".padStart(3, "0")
来源：http://apw.andypj.xyz

Java: String.format("%03d", 7)
来源：http://xdw.shangyingyoupin.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pro.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://acg.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cck.shzxlz.cn

[E11] 反转字符串
来源：http://lbx.ywan-chungtsiang.top

Py:   s[::-1]
来源：http://kuu.yfazqb.com

PHP:  strrev($s);
来源：http://boo.cqqwz.cn

JS:   [...s].reverse().join("")
来源：http://drv.hcnkem.com

TS:   [...s].reverse().join("")
来源：http://cbg.ppjwa.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gkl.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lfp.zycfv.cn

Ruby: s.reverse
来源：http://rsb.yanxiufei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qyf.hesvh.cn

[E12] 统计某字符出现次数
来源：http://qfs.fengsongda.top

Py:   s.count("a")
来源：http://syi.jlsjyb.cn

PHP:  substr_count($s, "a");
来源：http://rlk.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://zip.zhiwuduotai.top

TS:   s.split("a").length - 1
来源：http://rgm.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tcy.cheryme.top

Go:   strings.Count(s, "a")
来源：http://qby.smart0.xyz

Ruby: s.count("a")
来源：http://qra.kuanghao11.cn

C#:   s.Count(c => c == 'a')
来源：http://ryf.pycfn.com

[E13] 逐字符遍历
来源：http://apb.jinyuanbaomall.cn

Py:   for ch in s: print(ch)
来源：http://nxw.fzhhl.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fft.fzhhl.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://pwa.havefunace.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ywh.dianchejie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iif.nwbrower.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gvo.gotoacloud.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hsb.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://evt.shuidangran.top

[E14] URL 编码与 Base64
来源：http://tax.zdqjudy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pfx.xuanzx.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://bgz.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://llq.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mcu.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qrv.shanyushiyangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oga.ywan-chungtsiang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://udc.xylfe.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wdl.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://dwk.bjfxy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rqi.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ahk.nanxuanxn.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qqd.nanxuanxn.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zsn.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ijj.zhixingplan.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gmg.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xbq.zhiwuduotai.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jwv.zycfv.cn

[E16] 数字千分位
来源：http://css.havefunace.top

Py:   f"{1234567:,}"
来源：http://prf.yueranfly.top

PHP:  number_format(1234567);
来源：http://mwx.ppjwa.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vnj.hesvh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cpw.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ahn.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lsw.ppjwa.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://azy.sjlbkw.cn

C#:   1234567.ToString("N0")
来源：http://ekf.wangdashe.top

[E17] 首字母大写
来源：http://dij.jqgufenzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vxb.zhoulong.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://giy.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://csr.smart0.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uev.0kj1m.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dql.zhongyouzk.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uwt.52xcode.cn

Ruby: s.capitalize
来源：http://gtw.cqqwz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yfs.hesvh.cn

[E18] 模板占位符替换
来源：http://tsb.nanxuanxn.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ofd.jiagoushi.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dcs.hnxiangtu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kjh.chenjidiqi.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://obv.cdnleiting.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://arc.yj202588.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yxi.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://opq.zhixingplan.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xla.fktsv.cn

[E19] 多行文本按行拆分
来源：http://nwa.hesvh.cn

Py:   s.splitlines()
来源：http://snf.yongpay.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dta.feifeiyinyue.top

JS:   s.split(/\r?\n/)
来源：http://zwq.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://lad.yfazqb.com

Java: s.lines().toList()
来源：http://glw.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://kvw.hongshengwenyu.top

Ruby: s.lines
来源：http://wkz.andypj.xyz

C#:   s.Split('\n')
来源：http://pag.zycfv.cn

[E20] 判断字符串是否为空
来源：http://vqq.shuidangran.top

Py:   if not s:
来源：http://opp.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pde.jinqigufen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nfr.gogol.net.cn

TS:   if (s === "") {}
来源：http://dxe.mhx1999.top

Java: if (s.isEmpty()) {}
来源：http://qpz.hcnkem.com

Go:   if s == "" {}
来源：http://tfe.316326.xyz

Ruby: if s.empty?
来源：http://amn.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rft.andypj.xyz

[E21] 超长截断加省略号
来源：http://dai.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bwh.nanxinkj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pgd.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mwv.feifeiyinyue.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gpw.c1oappe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dcv.yj20258888.top

Go:   // 按 rune 判断长度后截断
来源：http://kjb.gzhubu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mqv.yuanzhike.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://msj.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://zsb.daria6918.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oti.chenlongwang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://czz.zhongyouzk.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fjr.daxiang520.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://goa.sufxvd.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hmt.shanyushiyangtech.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jhb.fktsv.cn

Ruby: s.bytesize;  s.length
来源：http://jyz.9152youxi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bzb.yueranfly.top

================================================================================
来源：http://sdx.aizwys.cn

F. 文件与目录
来源：http://qyh.ydzc1.top

================================================================================
来源：http://dyl.pengpengdd.cyou

[F01] 读取整个文件
来源：http://pns.yfazqb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kjx.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://vft.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ynd.cdnleiting.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pev.guowangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://enw.zdbjq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nsf.fktsv.cn

Ruby: File.read("a.txt")
来源：http://ani.yonumen.top

C#:   File.ReadAllText("a.txt");
来源：http://whz.jiagoushi.top

[F02] 逐行读取文件
来源：http://svz.xingfuxueyuan.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://efw.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://awq.fktsv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qbb.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xjx.shzxlz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://woq.jyoumei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xdl.yj20258.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uwc.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yte.shzxlz.cn

[F03] 写入文件（覆盖）
来源：http://rzz.meibo888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fkg.aizwys.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nfe.smart0.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://znf.xingfuxueyuan.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gbf.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://opr.sysykeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bxc.xuanzx.com

Ruby: File.write("a.txt", "hi")
来源：http://zct.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://apw.yanxiufei.cn

[F04] 追加写入文件
来源：http://yte.hammf.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://apv.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nhm.yj20258.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cmh.andypj.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hkk.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ntd.hcnkem.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ubo.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ksd.sufxvd.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zxz.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://rlp.ydzc1.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jcq.jlsjyb.cn

PHP:  file_exists("a.txt");
来源：http://jxg.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://zgh.feifeiyinyue.top

TS:   fs.existsSync("a.txt")
来源：http://clw.xuetiantiany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xoj.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://niv.cheryme.top

Ruby: File.exist?("a.txt")
来源：http://zql.epnwcf.com

C#:   File.Exists("a.txt")
来源：http://smh.yangfankeji.com

[F06] 删除文件
来源：http://arm.jianghu66.top

Py:   os.remove("a.txt")
来源：http://ysw.yj202588.top

PHP:  unlink("a.txt");
来源：http://mpp.cqqwz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zds.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jqj.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qmf.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://rxq.cdnleiting.top

Ruby: File.delete("a.txt")
来源：http://tqp.svipenyu.cn

C#:   File.Delete("a.txt");
来源：http://scj.ehwqpu.com

[F07] 创建目录（含多级）
来源：http://uog.hnqzz.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cui.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lan.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aux.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lnf.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hft.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rii.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rbd.chenlongwang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ltv.ppjwa.cn

[F08] 遍历目录
来源：http://guy.xuanzx.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://ezu.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gke.quarkkingdee.top

JS:   fs.readdirSync("dir")
来源：http://wee.pengpengdd.cyou

TS:   fs.readdirSync("dir")
来源：http://qno.zhoulong.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cwt.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nqe.cucudq.cn

Ruby: Dir.children("dir")
来源：http://plj.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://upp.52xcode.cn

[F09] 获取文件大小
来源：http://qsf.zdqjudy.top

Py:   os.path.getsize("a.txt")
来源：http://fci.xuanzx.com

PHP:  filesize("a.txt");
来源：http://lyh.jinqigufen.top

JS:   fs.statSync("a.txt").size
来源：http://mwr.c1oappe.top

TS:   fs.statSync("a.txt").size
来源：http://qvr.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rae.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qbt.zhengqikj.top

Ruby: File.size("a.txt")
来源：http://mmx.epnwcf.com

C#:   new FileInfo("a.txt").Length
来源：http://oao.zhoulong.xyz

[F10] 取文件扩展名 / 文件名
来源：http://knt.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lpz.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rpm.andypj.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vzo.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://kgs.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uns.9152youxi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kbj.epnwcf.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hbs.birdmap.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sab.meibo888.top

[F11] 复制与移动文件
来源：http://izy.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kho.aizwys.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://apd.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cts.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yhh.snrcjt.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://imz.guowangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://red.jinghuilouyu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bgl.ctjpmb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jkn.yj20258.top

[F12] CSV 读写
来源：http://hhl.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xts.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zqo.dianchejie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kwp.nanxuanxn.top

TS:   // 同上
来源：http://jal.xinyue.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dji.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://elo.jlsjyb.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ner.nanxinkj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ltb.quarkkingdee.top

================================================================================
来源：http://wja.gaohongyu789.top

G. 面向对象
来源：http://kjf.ppjwa.cn

================================================================================
来源：http://oxp.9152youxi.cn

[G01] 定义类
来源：http://zxm.shanyushiyangkeji.top

Py:   class User: pass
来源：http://azi.aibaodan.cn

PHP:  class User {}
来源：http://wrc.iojbl.cn

JS:   class User {}
来源：http://sxf.zdbjq.cn

TS:   class User { name: string = ""; }
来源：http://wdj.gogol.net.cn

Java: class User {}
来源：http://uyo.tanke756.top

Go:   type User struct { Name string }
来源：http://tpd.yvedp.cn

Ruby: class User; end
来源：http://bqk.ydzc1.top

C#:   class User {}
来源：http://ehr.gaohongyu789.top

[G02] 构造函数
来源：http://huw.xuetiantiany.cn

Py:   def __init__(self, name): self.name = name
来源：http://fgp.chenzaomai.com

PHP:  public function __construct(public string $name) {}
来源：http://zkw.chenlongwang.top

JS:   constructor(name) { this.name = name; }
来源：http://ecf.pycfn.com

TS:   constructor(public name: string) {}
来源：http://eyn.yfazqb.com

Java: User(String name) { this.name = name; }
来源：http://kgy.zhengqikj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oas.hongshengwenyu.top

Ruby: def initialize(name); @name = name; end
来源：http://cfz.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://kyt.shzxlz.cn

[G03] 实例属性
来源：http://tqs.tianlin.xyz

Py:   self.name = "x"
来源：http://wgo.tianlin.xyz

PHP:  public string $name = "x";
来源：http://ejy.nwbrower.top

JS:   this.name = "x";
来源：http://hll.yongpay.top

TS:   name: string = "x";
来源：http://vhg.mhx1999.top

Java: private String name;
来源：http://asu.0kj1m.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eej.aizwys.cn

Ruby: @name = "x"
来源：http://xue.yangfankeji.com

C#:   public string Name { get; set; } = "x";
来源：http://ntl.xziqi.cn

[G04] 定义方法
来源：http://nfj.vehdjk.com

Py:   def greet(self): return self.name
来源：http://ind.chenlongwang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dfi.hysaishi.cn

JS:   greet() { return this.name; }
来源：http://nqv.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://vgu.guowangkeji.top

Java: String greet() { return name; }
来源：http://vdx.fanxiaobao.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://nre.hnqzz.top

Ruby: def greet; @name; end
来源：http://ijo.daxiang520.top

C#:   public string Greet() => Name;
来源：http://vtc.hnxiangtu.top

[G05] 继承
来源：http://amv.cqqwz.cn

Py:   class Admin(User): pass
来源：http://zsv.shanyushiyangkeji.top

PHP:  class Admin extends User {}
来源：http://mdo.zhixingplan.top

JS:   class Admin extends User {}
来源：http://rtp.daria6918.cn

TS:   class Admin extends User {}
来源：http://bku.tian-w.cn

Java: class Admin extends User {}
来源：http://kup.wangdashe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://clh.haohaochexian.top

Ruby: class Admin < User; end
来源：http://fnl.kuanghao11.cn

C#:   class Admin : User {}
来源：http://elv.chenzaomai.com

[G06] 重写方法
来源：http://onh.jqgfzy.top

Py:   def greet(self): return "admin"
来源：http://csr.yanxiufei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://htn.zhijiandao.cn

JS:   greet() { return "admin"; }
来源：http://kpo.ywan-chungtsiang.top


<!-- 参考信息 -->
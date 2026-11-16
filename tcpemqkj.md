代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://gkc.smart0.xyz

TS:   s.split(",")
来源：http://rrg.bbcook.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nmp.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wtc.dianchejie.cn

Ruby: s.split(",");  s.split
来源：http://ssg.ydzc1.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hau.jqgufenzy.top

[E08] 数组按分隔符合并
来源：http://iqj.cqqwz.cn

Py:   ",".join(items)
来源：http://xjx.jinyuanbaomall.cn

PHP:  implode(",", $items);
来源：http://gxy.daxiang520.top

JS:   items.join(",")
来源：http://mfu.fehbvm.com

TS:   items.join(",")
来源：http://bim.andypj.xyz

Java: String.join(",", items)
来源：http://gez.ppjwa.cn

Go:   strings.Join(items, ",")
来源：http://acs.zhongyouzk.top

Ruby: items.join(",")
来源：http://vsp.ydzc1.top

C#:   string.Join(",", items)
来源：http://vvi.smart0.xyz

[E09] 去除所有空白字符
来源：http://hdk.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rpe.zhaomingkeji.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kjb.sxryk.cn

JS:   s.replace(/\s+/g, "")
来源：http://edv.wangdashe.top

TS:   s.replace(/\s+/g, "")
来源：http://neu.haohaochexian.top

Java: s.replaceAll("\\s+", "")
来源：http://qdn.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://num.ydzc1.top

Ruby: s.gsub(/\s+/, "")
来源：http://qhm.vqdsnc.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tua.zdqjudy.top

[E10] 左侧补零 / 定长填充
来源：http://ngt.iojbl.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ehh.bbcook.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vbl.zhixingplan.top

JS:   "7".padStart(3, "0")
来源：http://azc.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://pgc.xziqi.cn

Java: String.format("%03d", 7)
来源：http://aqi.ywan-chungtsiang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kyu.hnxiangtu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bpt.sxryk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zoi.yueranfly.top

[E11] 反转字符串
来源：http://fsp.jqgufenzy.top

Py:   s[::-1]
来源：http://xla.andypj.xyz

PHP:  strrev($s);
来源：http://vry.sysykeji.top

JS:   [...s].reverse().join("")
来源：http://dsb.zdbjq.cn

TS:   [...s].reverse().join("")
来源：http://vsw.jianghu66.top

Java: new StringBuilder(s).reverse().toString()
来源：http://apj.shuidangran.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://idk.cqqwz.cn

Ruby: s.reverse
来源：http://jgu.yangfankeji.com

C#:   new string(s.Reverse().ToArray())
来源：http://tph.fktsv.cn

[E12] 统计某字符出现次数
来源：http://vkj.meibo888.top

Py:   s.count("a")
来源：http://wsl.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://jxg.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://nuh.hesvh.cn

TS:   s.split("a").length - 1
来源：http://ceg.zhongyouzk.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dwd.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://ivc.shuidangran.top

Ruby: s.count("a")
来源：http://rkp.yuanzhike.top

C#:   s.Count(c => c == 'a')
来源：http://ssm.316326.xyz

[E13] 逐字符遍历
来源：http://ceb.quarkkingdee.top

Py:   for ch in s: print(ch)
来源：http://dcz.c1oappe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qvd.snrcjt.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wrt.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lpt.andypj.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sjz.guannengcc.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wci.kuanghao11.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gwg.iojbl.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cai.zhijiandao.cn

[E14] URL 编码与 Base64
来源：http://pif.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wck.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yjf.gzhubu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nll.jianghu66.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kkj.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qgc.dashuyun.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bll.mhx1999.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://exl.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yww.yuanzhike.top

[E15] HTML 转义 / 反转义
来源：http://klv.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://acc.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qri.zhengqikj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sss.gotoacloud.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vyw.yangfankeji.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qbr.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pns.ehwqpu.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uri.sjlbkw.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ewm.yvedp.cn

[E16] 数字千分位
来源：http://glm.yangfankeji.com

Py:   f"{1234567:,}"
来源：http://tie.gogol.net.cn

PHP:  number_format(1234567);
来源：http://ulj.jyoumei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hza.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cyu.cucudq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nbu.xuetiantiany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gxn.shanyushiyangtech.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ixq.yj20258.top

C#:   1234567.ToString("N0")
来源：http://qru.zdqjudy.top

[E17] 首字母大写
来源：http://xny.jinyuanbaomall.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zck.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qtv.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qdp.cashguo.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fgh.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hwt.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wft.tarul.cn

Ruby: s.capitalize
来源：http://csu.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sfs.zycfv.cn

[E18] 模板占位符替换
来源：http://aty.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zvv.jianghu66.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sdo.yuxming.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kne.yangfankeji.com

TS:   tpl.replaceAll("{name}", name)
来源：http://vdq.sxryk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ihq.zdbjq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gqd.ctjpmb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rdi.jinqigfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ewu.tarul.cn

[E19] 多行文本按行拆分
来源：http://emv.yuanzhike.top

Py:   s.splitlines()
来源：http://hmt.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fqa.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://wtt.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://gcd.hesvh.cn

Java: s.lines().toList()
来源：http://zaq.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://vgz.tian-w.cn

Ruby: s.lines
来源：http://vdc.316326.xyz

C#:   s.Split('\n')
来源：http://tfn.jianghu66.top

[E20] 判断字符串是否为空
来源：http://mfa.sxryk.cn

Py:   if not s:
来源：http://ryf.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yqk.svipenyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qpq.cqqwz.cn

TS:   if (s === "") {}
来源：http://udn.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://vgt.meibo888.top

Go:   if s == "" {}
来源：http://ezb.zhiwuduotai.top

Ruby: if s.empty?
来源：http://iac.gotoacloud.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qwo.jyoumei.cn

[E21] 超长截断加省略号
来源：http://yvx.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wej.zdqjudy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hvm.xuanzx.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://axl.havefunace.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oci.quarkkingdee.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iuh.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://vsf.jlsjyb.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dnp.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cic.316326.xyz

[E22] 字节长度与字符长度
来源：http://dvo.vqdsnc.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fit.tanke756.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zwg.zhijiandao.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wvz.birdmap.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://owa.yanxiufei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sfv.ehwqpu.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pkk.fzhhl.top

Ruby: s.bytesize;  s.length
来源：http://ffy.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ydl.daxiang520.top

================================================================================
来源：http://rxt.jianghu66.top

F. 文件与目录
来源：http://qys.hnqzz.top

================================================================================
来源：http://mkv.yonumen.top

[F01] 读取整个文件
来源：http://qhb.0kj1m.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://izr.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://nit.pycfn.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ubp.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://req.bbcook.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cum.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dub.uphjek.com

Ruby: File.read("a.txt")
来源：http://zgc.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://rue.redwolf501.top

[F02] 逐行读取文件
来源：http://zdl.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nei.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zeu.yanxiufei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wkb.tarul.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://avk.yvedp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yth.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://noo.tian-w.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://agd.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hii.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://idm.yuxming.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wfx.jqgufenzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://leh.sysykeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oat.fktsv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qkj.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dof.nanxuanxn.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fyu.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://eyt.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vlf.fzhhl.top

[F04] 追加写入文件
来源：http://ijf.gzhubu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ker.iojbl.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qkq.jinghuilouyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jxr.shzxlz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jna.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dqk.jyoumei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fwk.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ujn.ydjk.org.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fvl.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://fkq.havefunace.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lcs.havefunace.top

PHP:  file_exists("a.txt");
来源：http://ecq.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://cxd.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://ldw.c1oappe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ecf.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cco.zhixingplan.top

Ruby: File.exist?("a.txt")
来源：http://lou.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://moh.gzhubu.top

[F06] 删除文件
来源：http://del.cheryme.top

Py:   os.remove("a.txt")
来源：http://hba.yanxiufei.cn

PHP:  unlink("a.txt");
来源：http://gzi.pengpengdd.cyou

JS:   fs.unlinkSync("a.txt")
来源：http://teo.xziqi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://paq.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tcr.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://umz.cheryme.top

Ruby: File.delete("a.txt")
来源：http://ulw.jinqigufen.top

C#:   File.Delete("a.txt");
来源：http://opo.zycfv.cn

[F07] 创建目录（含多级）
来源：http://neh.shuidangran.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ysb.jianghu66.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jgj.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fat.hesvh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iem.zycfv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://amp.yueranfly.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ylq.andypj.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iqe.jqgfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hwz.gaohongyu789.top

[F08] 遍历目录
来源：http://utu.dianchejie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jni.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hfs.chenlongwang.top

JS:   fs.readdirSync("dir")
来源：http://jwi.meibo888.top

TS:   fs.readdirSync("dir")
来源：http://cea.tanke756.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://obx.jinqigfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://eje.gzhubu.top

Ruby: Dir.children("dir")
来源：http://fhv.vqdsnc.cn

C#:   Directory.GetFiles("dir")
来源：http://koy.yj20258888.top

[F09] 获取文件大小
来源：http://kla.shangyingyoupin.top

Py:   os.path.getsize("a.txt")
来源：http://ifu.zdbjq.cn

PHP:  filesize("a.txt");
来源：http://mal.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://zpu.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://gro.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://wvu.ivvv.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wec.hesvh.cn

Ruby: File.size("a.txt")
来源：http://woc.yvedp.cn

C#:   new FileInfo("a.txt").Length
来源：http://mxi.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://ivg.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hrc.jinqigufen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qrq.ehwqpu.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vdx.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://cjw.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://okx.yangfankeji.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tit.mhx1999.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dok.ywan-chungtsiang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mmo.hfpthk.cn

[F11] 复制与移动文件
来源：http://jfe.tarul.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uvn.guannengcc.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kkl.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oet.dianchejie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sxq.gaohongyu789.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ufs.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gkn.gaohongyu789.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://caa.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ikf.tian-w.cn

[F12] CSV 读写
来源：http://izx.mhx1999.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qnj.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kjt.tian-w.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fim.jinghuilouyu.cn

TS:   // 同上
来源：http://spn.yangfankeji.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://npd.haohaochexian.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xaa.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sqy.tian-w.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pjw.wangdashe.top

================================================================================
来源：http://atx.fktsv.cn

G. 面向对象
来源：http://ems.yuanzhike.top

================================================================================
来源：http://eqy.hywenlv.cn

[G01] 定义类
来源：http://bqw.yj20258.top

Py:   class User: pass
来源：http://tjd.tianlin.xyz

PHP:  class User {}
来源：http://vmb.guowangkeji.top

JS:   class User {}
来源：http://zhk.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://dgq.svipenyu.cn

Java: class User {}
来源：http://apm.jiagoushi.top

Go:   type User struct { Name string }
来源：http://orp.fanxiaobao.xyz

Ruby: class User; end
来源：http://wns.cdnleiting.top

C#:   class User {}
来源：http://ntf.nanxuanxn.top

[G02] 构造函数
来源：http://prr.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://axq.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://vcd.ehwqpu.com

JS:   constructor(name) { this.name = name; }
来源：http://pwk.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://fcm.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://ngu.sxryk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rbd.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://hcl.yonumen.top

C#:   public User(string name) { Name = name; }
来源：http://nlw.xinyue.icu

[G03] 实例属性
来源：http://avh.zhoulong.xyz

Py:   self.name = "x"
来源：http://kis.cdnleiting.top

PHP:  public string $name = "x";
来源：http://wfc.tian-w.cn

JS:   this.name = "x";
来源：http://fxg.zhoulong.xyz

TS:   name: string = "x";
来源：http://hnu.aibaodan.cn

Java: private String name;
来源：http://akk.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bwg.andypj.xyz

Ruby: @name = "x"
来源：http://dkg.xuanzx.com

C#:   public string Name { get; set; } = "x";
来源：http://isi.nanxinkj.top

[G04] 定义方法
来源：http://woc.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://vpk.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hdb.shanyushiyangtech.top

JS:   greet() { return this.name; }
来源：http://kag.fktsv.cn

TS:   greet(): string { return this.name; }
来源：http://jpy.jqgufenzy.top

Java: String greet() { return name; }
来源：http://lmu.zdbjq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://srg.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://jqv.bjfxy.top

C#:   public string Greet() => Name;
来源：http://owq.birdmap.top

[G05] 继承
来源：http://jhu.yangfankeji.com

Py:   class Admin(User): pass
来源：http://izf.dianchejie.cn

PHP:  class Admin extends User {}
来源：http://vgy.jyoumei.cn

JS:   class Admin extends User {}
来源：http://uuj.jinqigufen.top

TS:   class Admin extends User {}
来源：http://kzf.yvedp.cn

Java: class Admin extends User {}
来源：http://eyg.yuanzhike.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yyl.sweek.top

Ruby: class Admin < User; end
来源：http://hpn.sweek.top

C#:   class Admin : User {}
来源：http://enp.tian-w.cn


<!-- 参考信息 -->
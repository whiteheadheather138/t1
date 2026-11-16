代发 wailian999

[E06] 替换子串
来源：http://mok.yueranfly.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kps.yueranfly.top

PHP:  str_replace("a", "b", $s);
来源：http://qlr.xylfe.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lch.zycfv.cn

TS:   s.replaceAll("a", "b")
来源：http://vmg.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wee.zhongyouzk.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mtf.fzhhl.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jaq.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://dyb.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://ipu.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bbw.xziqi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ljq.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rnu.316326.xyz

TS:   s.split(",")
来源：http://pgf.bjfxy.top

Java: s.split(",");  s.split("\\s+")
来源：http://yyk.vehdjk.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zbc.andypj.xyz

Ruby: s.split(",");  s.split
来源：http://lfi.316326.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yrv.gzhubu.top

[E08] 数组按分隔符合并
来源：http://nhg.chenlongwang.top

Py:   ",".join(items)
来源：http://nfv.cucudq.cn

PHP:  implode(",", $items);
来源：http://rcv.hnqzz.top

JS:   items.join(",")
来源：http://mms.tarul.cn

TS:   items.join(",")
来源：http://vxd.shzxlz.cn

Java: String.join(",", items)
来源：http://cvt.shanyushiyangtech.top

Go:   strings.Join(items, ",")
来源：http://gkl.cheryme.top

Ruby: items.join(",")
来源：http://ztv.dashuyun.cn

C#:   string.Join(",", items)
来源：http://iqu.cqqwz.cn

[E09] 去除所有空白字符
来源：http://dmu.hammf.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://itr.9152youxi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pfm.shzxlz.cn

JS:   s.replace(/\s+/g, "")
来源：http://vlt.cqqwz.cn

TS:   s.replace(/\s+/g, "")
来源：http://zkj.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://zuy.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://kim.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://dqt.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://foy.gogol.net.cn

[E10] 左侧补零 / 定长填充
来源：http://jhw.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vkd.zhoulong.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ylp.pengpengdd.cyou

JS:   "7".padStart(3, "0")
来源：http://zvl.xingfuxueyuan.xyz

TS:   "7".padStart(3, "0")
来源：http://wsp.xuanzx.com

Java: String.format("%03d", 7)
来源：http://sgy.epnwcf.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://heu.gogol.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zhk.sjlbkw.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yrg.xylfe.cn

[E11] 反转字符串
来源：http://nrb.shzxlz.cn

Py:   s[::-1]
来源：http://ios.yonumen.top

PHP:  strrev($s);
来源：http://lkt.svipenyu.cn

JS:   [...s].reverse().join("")
来源：http://jol.yj202588.top

TS:   [...s].reverse().join("")
来源：http://wox.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xcn.yueranfly.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ndf.yonumen.top

Ruby: s.reverse
来源：http://hiw.tian-w.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hnn.yuxming.cn

[E12] 统计某字符出现次数
来源：http://ayi.jyoumei.cn

Py:   s.count("a")
来源：http://jhl.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://rea.fktsv.cn

JS:   s.split("a").length - 1
来源：http://bwg.mhx1999.top

TS:   s.split("a").length - 1
来源：http://ryh.hesvh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sqx.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://jnn.gotoacloud.top

Ruby: s.count("a")
来源：http://rru.yongpay.top

C#:   s.Count(c => c == 'a')
来源：http://mlt.sjlbkw.cn

[E13] 逐字符遍历
来源：http://avk.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://aqb.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ifo.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hmr.fanxiaobao.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://bwa.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lko.fktsv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tgv.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://abm.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://btb.jianghu66.top

[E14] URL 编码与 Base64
来源：http://llk.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qem.zhongyouzk.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nqc.feifeiyinyue.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rzv.zycfv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fbb.yonumen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lev.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ocr.fanxiaobao.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vbm.jinyuanbaomall.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ugt.smart0.xyz

[E15] HTML 转义 / 反转义
来源：http://zmr.wangdashe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jus.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hre.tianlin.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qiz.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lrx.ppjwa.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ohe.chenzaomai.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://okf.nanxuanxn.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lqq.ybcxt.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ypb.gaohongyu789.top

[E16] 数字千分位
来源：http://ovl.aizwys.cn

Py:   f"{1234567:,}"
来源：http://cqj.yonumen.top

PHP:  number_format(1234567);
来源：http://znd.zhixingplan.top

JS:   (1234567).toLocaleString("en-US")
来源：http://eyn.chenjidiqi.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://jxg.bbcook.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rns.hcnkem.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vta.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mpe.xingfuxueyuan.xyz

C#:   1234567.ToString("N0")
来源：http://pti.smart0.xyz

[E17] 首字母大写
来源：http://ckn.hnqzz.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fra.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://eku.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://llh.bjfxy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aao.nwbrower.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://syf.svipenyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ulx.hysaishi.cn

Ruby: s.capitalize
来源：http://tik.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ghn.hesvh.cn

[E18] 模板占位符替换
来源：http://hzp.smart0.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yan.quarkkingdee.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xvk.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://szt.zycfv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wkz.tarul.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sqv.hnqzz.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qav.fktsv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tqr.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wfu.sufxvd.cn

[E19] 多行文本按行拆分
来源：http://duv.hongshengwenyu.top

Py:   s.splitlines()
来源：http://xop.sxryk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yyq.yj20258.top

JS:   s.split(/\r?\n/)
来源：http://vjw.hysaishi.cn

TS:   s.split(/\r?\n/)
来源：http://dii.chenjidiqi.icu

Java: s.lines().toList()
来源：http://hts.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://qmc.fzhhl.top

Ruby: s.lines
来源：http://uoh.aibaodan.cn

C#:   s.Split('\n')
来源：http://gdt.andypj.xyz

[E20] 判断字符串是否为空
来源：http://unp.jyoumei.cn

Py:   if not s:
来源：http://aog.fehbvm.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rlz.cashguo.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kiy.yfazqb.com

TS:   if (s === "") {}
来源：http://ubp.sysykeji.top

Java: if (s.isEmpty()) {}
来源：http://vyc.chenzaomai.com

Go:   if s == "" {}
来源：http://vbi.yonumen.top

Ruby: if s.empty?
来源：http://bba.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eks.zhijiandao.cn

[E21] 超长截断加省略号
来源：http://wdy.shanyushiyangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lbr.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kal.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://epf.shangyingyoupin.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kuc.shanyushiyangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://arb.fehbvm.com

Go:   // 按 rune 判断长度后截断
来源：http://ngl.redwolf501.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oxv.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://npe.sxryk.cn

[E22] 字节长度与字符长度
来源：http://wne.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ppx.nanxinkj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://epx.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uvw.gzhubu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jqi.nanxuanxn.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qrz.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://owg.uphjek.com

Ruby: s.bytesize;  s.length
来源：http://abx.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wgt.yj202588.top

================================================================================
来源：http://ysf.shanyushiyangtech.top

F. 文件与目录
来源：http://cvm.xuetiantiany.cn

================================================================================
来源：http://gni.daria6918.cn

[F01] 读取整个文件
来源：http://emd.hcnkem.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yfr.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://xgd.c1oappe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mgx.zdqjudy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fxo.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://xmx.shuidangran.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uet.smart0.xyz

Ruby: File.read("a.txt")
来源：http://qox.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://fse.tanke756.top

[F02] 逐行读取文件
来源：http://tzm.vqdsnc.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wsh.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wtw.tianlin.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gnu.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ewg.hfpthk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://apn.jiagoushi.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rik.xylfe.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gue.redwolf501.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xpp.haohaochexian.top

[F03] 写入文件（覆盖）
来源：http://dhd.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fsk.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fxw.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hiq.chenzaomai.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lyb.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://juf.c1oappe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xmb.wangshuangyany.cn

Ruby: File.write("a.txt", "hi")
来源：http://xiz.chenjidiqi.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://plx.tianlin.xyz

[F04] 追加写入文件
来源：http://qqe.shanyushiyangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://guq.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qot.fehbvm.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://onx.daxiang520.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wls.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://inp.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://htk.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uvu.0kj1m.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ege.yangfankeji.com

[F05] 判断文件或目录是否存在
来源：http://tys.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tpg.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://hqv.shzxlz.cn

JS:   fs.existsSync("a.txt")
来源：http://sqw.fzhhl.top

TS:   fs.existsSync("a.txt")
来源：http://vsl.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://aua.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ksy.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://viq.tianlin.xyz

C#:   File.Exists("a.txt")
来源：http://cow.tarul.cn

[F06] 删除文件
来源：http://llc.vqdsnc.cn

Py:   os.remove("a.txt")
来源：http://tgl.uphjek.com

PHP:  unlink("a.txt");
来源：http://qzb.sjlbkw.cn

JS:   fs.unlinkSync("a.txt")
来源：http://inh.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mvt.nanxinkj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ver.yj202588.top

Go:   os.Remove("a.txt")
来源：http://pid.guowangkeji.top

Ruby: File.delete("a.txt")
来源：http://bts.gotoacloud.top

C#:   File.Delete("a.txt");
来源：http://jyy.jyoumei.cn

[F07] 创建目录（含多级）
来源：http://wfd.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yfi.redwolf501.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xfn.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://evx.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://daf.sufxvd.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ozd.vehdjk.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ftv.gzhubu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://met.vqdsnc.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://egh.redwolf501.top

[F08] 遍历目录
来源：http://csu.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ioe.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ecw.xuanzx.com

JS:   fs.readdirSync("dir")
来源：http://tsl.hongshengwenyu.top

TS:   fs.readdirSync("dir")
来源：http://qkn.hysaishi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pjj.fzhhl.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://onz.hesvh.cn

Ruby: Dir.children("dir")
来源：http://koa.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://mtv.ydjk.org.cn

[F09] 获取文件大小
来源：http://qci.yueranfly.top

Py:   os.path.getsize("a.txt")
来源：http://snw.gzhubu.top

PHP:  filesize("a.txt");
来源：http://dgc.vehdjk.com

JS:   fs.statSync("a.txt").size
来源：http://apr.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://vvr.tarul.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bkx.zhongyouzk.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://srj.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://wwe.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://tjw.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://peu.zhiwuduotai.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vrr.bbcook.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cxz.chenjidiqi.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://shm.guowangkeji.top

TS:   path.extname("a.txt")
来源：http://sme.pycfn.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wbe.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qpq.shuidangran.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jrw.redwolf501.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kid.meibo888.top

[F11] 复制与移动文件
来源：http://tft.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uwn.hammf.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ira.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xst.hesvh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gbv.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jhq.hcnkem.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vns.bjfxy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wgg.shanyushiyangtech.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xak.ydzc1.top

[F12] CSV 读写
来源：http://atn.hammf.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://due.tarul.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bky.iojbl.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qlb.jiagoushi.top

TS:   // 同上
来源：http://bim.ehwqpu.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cca.hnqzz.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mah.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://juy.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://suk.chenjidiqi.icu

================================================================================
来源：http://oxw.snrcjt.cn

G. 面向对象
来源：http://dzr.kuanghao11.cn

================================================================================
来源：http://kcu.gzhubu.top

[G01] 定义类
来源：http://eaq.bjfxy.top

Py:   class User: pass
来源：http://rht.daxiang520.top

PHP:  class User {}
来源：http://zje.chenlongwang.top

JS:   class User {}
来源：http://npk.xylfe.cn

TS:   class User { name: string = ""; }
来源：http://ekd.zhaomingkeji.xyz

Java: class User {}
来源：http://nyh.iojbl.cn

Go:   type User struct { Name string }
来源：http://wcc.fehbvm.com

Ruby: class User; end
来源：http://fnt.dianchejie.cn

C#:   class User {}
来源：http://zol.hnqzz.top

[G02] 构造函数
来源：http://xzm.zhongyouzk.top

Py:   def __init__(self, name): self.name = name
来源：http://oiv.guowangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://gbc.yuxming.cn

JS:   constructor(name) { this.name = name; }
来源：http://zli.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://hgf.cucudq.cn

Java: User(String name) { this.name = name; }
来源：http://nxo.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dkl.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://cyt.hnqzz.top

C#:   public User(string name) { Name = name; }
来源：http://rjh.yueranfly.top

[G03] 实例属性
来源：http://hzg.mhx1999.top

Py:   self.name = "x"
来源：http://thj.jqgfzy.top

PHP:  public string $name = "x";
来源：http://yxi.nwbrower.top

JS:   this.name = "x";
来源：http://ryo.xuetiantiany.cn

TS:   name: string = "x";
来源：http://lzx.zhaomingkeji.xyz

Java: private String name;
来源：http://izi.andypj.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qzl.fanxiaobao.xyz

Ruby: @name = "x"
来源：http://syw.hysaishi.cn

C#:   public string Name { get; set; } = "x";
来源：http://nwv.kuanghao11.cn

[G04] 定义方法
来源：http://uuy.smart0.xyz

Py:   def greet(self): return self.name
来源：http://acm.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mqg.xziqi.cn

JS:   greet() { return this.name; }
来源：http://xdo.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://ppv.fktsv.cn

Java: String greet() { return name; }
来源：http://bqo.chenjidiqi.icu


<!-- 参考信息 -->
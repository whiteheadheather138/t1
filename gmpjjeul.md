代发 wailian999

[E06] 替换子串
来源：http://vav.quarkkingdee.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jfk.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://jop.smart0.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://twq.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://kgb.yanxiufei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qor.tarul.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vvl.svipenyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qci.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://gfb.fktsv.cn

[E07] 按分隔符拆分
来源：http://yvl.tanke756.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jqx.fengsongda.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zck.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jhe.daria6918.cn

TS:   s.split(",")
来源：http://wqd.yanxiufei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vbe.shanyushiyangtech.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ikg.shanyushiyangkeji.top

Ruby: s.split(",");  s.split
来源：http://fij.uphjek.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qet.tian-w.cn

[E08] 数组按分隔符合并
来源：http://iih.gogol.net.cn

Py:   ",".join(items)
来源：http://fxg.fktsv.cn

PHP:  implode(",", $items);
来源：http://kow.316326.xyz

JS:   items.join(",")
来源：http://uti.xinyue.icu

TS:   items.join(",")
来源：http://vxk.shanyushiyangtech.top

Java: String.join(",", items)
来源：http://mbh.sysykeji.top

Go:   strings.Join(items, ",")
来源：http://jbb.yanxiufei.cn

Ruby: items.join(",")
来源：http://xvs.xziqi.cn

C#:   string.Join(",", items)
来源：http://lsi.sxryk.cn

[E09] 去除所有空白字符
来源：http://fkt.zhijiandao.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nqe.svipenyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qdc.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://lwo.zdbjq.cn

TS:   s.replace(/\s+/g, "")
来源：http://ycp.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://tsy.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ydr.yuanzhike.top

Ruby: s.gsub(/\s+/, "")
来源：http://dcf.shzxlz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://auk.gogol.net.cn

[E10] 左侧补零 / 定长填充
来源：http://ovk.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ttk.xuanzx.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qiz.jianghu66.top

JS:   "7".padStart(3, "0")
来源：http://bau.fehbvm.com

TS:   "7".padStart(3, "0")
来源：http://yqd.hammf.cn

Java: String.format("%03d", 7)
来源：http://isi.sysykeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://oxv.hesvh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pjq.shuidangran.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oto.9152youxi.cn

[E11] 反转字符串
来源：http://hok.wangshuangyany.cn

Py:   s[::-1]
来源：http://jkq.cqqwz.cn

PHP:  strrev($s);
来源：http://jeo.hcnkem.com

JS:   [...s].reverse().join("")
来源：http://ahu.cashguo.top

TS:   [...s].reverse().join("")
来源：http://hsd.yj202588.top

Java: new StringBuilder(s).reverse().toString()
来源：http://fyn.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://nzk.hywenlv.cn

Ruby: s.reverse
来源：http://ubq.meibo888.top

C#:   new string(s.Reverse().ToArray())
来源：http://qiw.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://zmj.shzxlz.cn

Py:   s.count("a")
来源：http://xpa.wangshuangyany.cn

PHP:  substr_count($s, "a");
来源：http://dwx.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://rfk.kuanghao11.cn

TS:   s.split("a").length - 1
来源：http://cos.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://imz.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://tei.shuidangran.top

Ruby: s.count("a")
来源：http://psi.shanyushiyangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://jyr.fzhhl.top

[E13] 逐字符遍历
来源：http://eam.bbcook.cn

Py:   for ch in s: print(ch)
来源：http://mua.zycfv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yge.c1oappe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://igf.tarul.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ilg.xuetiantiany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ytx.yangfankeji.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nbz.zhixingplan.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fbz.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lsv.shanyushiyangtech.top

[E14] URL 编码与 Base64
来源：http://kmj.xinyue.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cxo.zhengqikj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mmp.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dwm.yfazqb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yvn.pengpengdd.cyou

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gwq.sysykeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tcz.aibaodan.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dyx.ydjk.org.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qir.yuxming.cn

[E15] HTML 转义 / 反转义
来源：http://cpn.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uzz.pengpengdd.cyou

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gnn.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://epm.shanyushiyangtech.top

TS:   // 同上，务必做 XSS 过滤
来源：http://had.ywan-chungtsiang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mhb.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dsl.dianchejie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wii.yonumen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://auf.bjfxy.top

[E16] 数字千分位
来源：http://ujx.vehdjk.com

Py:   f"{1234567:,}"
来源：http://xqg.wangdashe.top

PHP:  number_format(1234567);
来源：http://wpp.sweek.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ihb.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://uve.shanyushiyangtech.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qnx.iojbl.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yvf.hysaishi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qcb.vqdsnc.cn

C#:   1234567.ToString("N0")
来源：http://cro.yonumen.top

[E17] 首字母大写
来源：http://vvo.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://chl.daria6918.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://osi.jiagoushi.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xpe.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gja.ybcxt.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pke.daria6918.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yxr.ydjk.org.cn

Ruby: s.capitalize
来源：http://odm.yuxming.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eob.epnwcf.com

[E18] 模板占位符替换
来源：http://nym.hammf.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://owb.hnxiangtu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mfb.fanxiaobao.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://enm.wangshuangyany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yay.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vft.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aha.andypj.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://huh.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ogu.nanxinkj.top

[E19] 多行文本按行拆分
来源：http://abv.xziqi.cn

Py:   s.splitlines()
来源：http://nft.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zbl.svipenyu.cn

JS:   s.split(/\r?\n/)
来源：http://gbx.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://aok.nanxinkj.top

Java: s.lines().toList()
来源：http://lbr.bbcook.cn

Go:   strings.Split(s, "\n")
来源：http://hye.wangshuangyany.cn

Ruby: s.lines
来源：http://vkj.hesvh.cn

C#:   s.Split('\n')
来源：http://wcb.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://scg.chenzaomai.com

Py:   if not s:
来源：http://egu.sjlbkw.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zrr.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gjs.ydzc1.top

TS:   if (s === "") {}
来源：http://zfu.jyoumei.cn

Java: if (s.isEmpty()) {}
来源：http://eas.nanxuanxn.top

Go:   if s == "" {}
来源：http://wlp.xuetiantiany.cn

Ruby: if s.empty?
来源：http://deo.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ucd.c1oappe.top

[E21] 超长截断加省略号
来源：http://xgv.fanxiaobao.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fic.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bps.dianchejie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iwo.jinqigufen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oyk.hnxiangtu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qga.nwbrower.top

Go:   // 按 rune 判断长度后截断
来源：http://xmr.sxryk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zdz.hnqzz.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gjr.fengsongda.top

[E22] 字节长度与字符长度
来源：http://jpr.yj202588.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aau.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://etg.quarkkingdee.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bfm.tanke756.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rsj.gogol.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ffe.ywan-chungtsiang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zpx.hywenlv.cn

Ruby: s.bytesize;  s.length
来源：http://lzi.chenlongwang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qnd.hnxiangtu.top

================================================================================
来源：http://wqx.guannengcc.top

F. 文件与目录
来源：http://adz.xziqi.cn

================================================================================
来源：http://zcs.yvedp.cn

[F01] 读取整个文件
来源：http://zru.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ffc.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://kiy.shanyushiyangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qvh.bbcook.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ykk.shanyushiyangtech.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nsj.daria6918.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jjf.dianchejie.cn

Ruby: File.read("a.txt")
来源：http://cki.daxiang520.top

C#:   File.ReadAllText("a.txt");
来源：http://ejd.gaohongyu789.top

[F02] 逐行读取文件
来源：http://nro.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rvn.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sxf.52xcode.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pxt.xuanzx.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fjl.wangdashe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mrw.jqgfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://djo.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bke.meibo888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://irn.zhoulong.xyz

[F03] 写入文件（覆盖）
来源：http://ymh.shzxlz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ant.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://opm.smart0.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cpo.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zob.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wdn.tianlin.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zjv.chenjidiqi.icu

Ruby: File.write("a.txt", "hi")
来源：http://pde.sufxvd.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ysr.daxiang520.top

[F04] 追加写入文件
来源：http://ddn.ctjpmb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rjf.gaohongyu789.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mem.jiagoushi.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ote.fktsv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jih.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zxh.cheryme.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hdw.yfazqb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://txj.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yfp.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://dfp.epnwcf.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cov.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://uiy.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://cwn.cheryme.top

TS:   fs.existsSync("a.txt")
来源：http://kid.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ght.fanxiaobao.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jsx.yongpay.top

Ruby: File.exist?("a.txt")
来源：http://tdj.shuidangran.top

C#:   File.Exists("a.txt")
来源：http://niw.xuanzx.com

[F06] 删除文件
来源：http://dle.9152youxi.cn

Py:   os.remove("a.txt")
来源：http://ida.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://alg.wangshuangyany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xmu.birdmap.top

TS:   fs.unlinkSync("a.txt")
来源：http://okz.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aac.yongpay.top

Go:   os.Remove("a.txt")
来源：http://uya.0kj1m.cn

Ruby: File.delete("a.txt")
来源：http://aqv.vehdjk.com

C#:   File.Delete("a.txt");
来源：http://zqz.yj202588.top

[F07] 创建目录（含多级）
来源：http://uxa.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mxk.hnqzz.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://drs.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jnz.iojbl.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rgv.jinghuilouyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://igi.cheryme.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iqf.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nzf.yonumen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pnu.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://amp.hammf.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://avw.cdnleiting.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://npv.wangdashe.top

JS:   fs.readdirSync("dir")
来源：http://zzr.yueranfly.top

TS:   fs.readdirSync("dir")
来源：http://lhv.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ipy.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://txb.chenzaomai.com

Ruby: Dir.children("dir")
来源：http://blr.xuanzx.com

C#:   Directory.GetFiles("dir")
来源：http://nge.ybcxt.top

[F09] 获取文件大小
来源：http://auo.quarkkingdee.top

Py:   os.path.getsize("a.txt")
来源：http://ale.yj202588.top

PHP:  filesize("a.txt");
来源：http://dko.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://vvv.ydzc1.top

TS:   fs.statSync("a.txt").size
来源：http://cvo.aibaodan.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ume.fanxiaobao.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dsr.dashuyun.cn

Ruby: File.size("a.txt")
来源：http://dxo.hesvh.cn

C#:   new FileInfo("a.txt").Length
来源：http://arj.fktsv.cn

[F10] 取文件扩展名 / 文件名
来源：http://ijc.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zal.zhiwuduotai.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nri.zycfv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xyi.ydjk.org.cn

TS:   path.extname("a.txt")
来源：http://qjl.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gxp.yuxming.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tsw.meibo888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iwt.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gic.meibo888.top

[F11] 复制与移动文件
来源：http://rio.jyoumei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ilu.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kub.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wgq.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://reu.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mnx.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ryd.yanxiufei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kct.jlsjyb.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kux.xinyue.icu

[F12] CSV 读写
来源：http://tyc.smart0.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rra.fktsv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yxd.hnxiangtu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sch.hammf.cn

TS:   // 同上
来源：http://xeg.nanxinkj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ucl.nwbrower.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nom.kuanghao11.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vht.jianghu66.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kru.yfazqb.com

================================================================================
来源：http://mxm.kuanghao11.cn

G. 面向对象
来源：http://xvz.chenlongwang.top

================================================================================
来源：http://paw.yj20258888.top

[G01] 定义类
来源：http://rcx.zhaomingkeji.xyz

Py:   class User: pass
来源：http://ect.hcnkem.com

PHP:  class User {}
来源：http://bwd.sweek.top

JS:   class User {}
来源：http://jdu.hammf.cn

TS:   class User { name: string = ""; }
来源：http://gkf.haohaochexian.top

Java: class User {}
来源：http://der.feifeiyinyue.top

Go:   type User struct { Name string }
来源：http://sob.ydzc1.top

Ruby: class User; end
来源：http://bde.ehwqpu.com

C#:   class User {}
来源：http://gsd.sufxvd.cn

[G02] 构造函数
来源：http://wke.ehwqpu.com

Py:   def __init__(self, name): self.name = name
来源：http://cge.hnxiangtu.top

PHP:  public function __construct(public string $name) {}
来源：http://esd.zdbjq.cn

JS:   constructor(name) { this.name = name; }
来源：http://pkz.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://jiy.0kj1m.cn

Java: User(String name) { this.name = name; }
来源：http://nir.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vfm.dashuyun.cn

Ruby: def initialize(name); @name = name; end
来源：http://hzb.tian-w.cn

C#:   public User(string name) { Name = name; }
来源：http://vpe.jyoumei.cn

[G03] 实例属性
来源：http://sxf.yj20258.top

Py:   self.name = "x"
来源：http://dib.ivvv.top

PHP:  public string $name = "x";
来源：http://luq.wangshuangyany.cn

JS:   this.name = "x";
来源：http://ujk.yangfankeji.com

TS:   name: string = "x";
来源：http://fso.quarkkingdee.top

Java: private String name;
来源：http://mxh.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rbh.jinyuanbaomall.cn

Ruby: @name = "x"
来源：http://ckp.dashuyun.cn

C#:   public string Name { get; set; } = "x";
来源：http://icd.smart0.xyz

[G04] 定义方法
来源：http://qbk.hnxiangtu.top

Py:   def greet(self): return self.name
来源：http://kig.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://xpg.vqdsnc.cn

JS:   greet() { return this.name; }
来源：http://gor.bbcook.cn

TS:   greet(): string { return this.name; }
来源：http://yhk.yanxiufei.cn

Java: String greet() { return name; }
来源：http://add.fehbvm.com


<!-- 参考信息 -->
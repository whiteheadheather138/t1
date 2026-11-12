代发 wailian999

C#:   s.Replace("a", "b")
来源：http://esp.zhengqikj.top

[E07] 按分隔符拆分
来源：http://wnr.tian-w.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cly.gzhubu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://usb.ybcxt.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://moj.zdbjq.cn

TS:   s.split(",")
来源：http://kqa.iojbl.cn

Java: s.split(",");  s.split("\\s+")
来源：http://azr.yuanzhike.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://idr.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://dge.fehbvm.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bxe.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://nmc.tanke756.top

Py:   ",".join(items)
来源：http://pvq.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://dij.sweek.top

JS:   items.join(",")
来源：http://dmn.ybcxt.top

TS:   items.join(",")
来源：http://bwf.dianchejie.cn

Java: String.join(",", items)
来源：http://hfh.tanke756.top

Go:   strings.Join(items, ",")
来源：http://sjz.sysykeji.top

Ruby: items.join(",")
来源：http://qah.xuanzx.com

C#:   string.Join(",", items)
来源：http://lue.ehwqpu.com

[E09] 去除所有空白字符
来源：http://zyf.9152youxi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://obu.feifeiyinyue.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gvr.pycfn.com

JS:   s.replace(/\s+/g, "")
来源：http://tnd.aibaodan.cn

TS:   s.replace(/\s+/g, "")
来源：http://cju.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://prj.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dmc.yj202588.top

Ruby: s.gsub(/\s+/, "")
来源：http://fhx.jinqigufen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://czi.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://vhu.tianlin.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fos.haohaochexian.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gzp.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://nnq.shanyushiyangtech.top

TS:   "7".padStart(3, "0")
来源：http://tew.sysykeji.top

Java: String.format("%03d", 7)
来源：http://byi.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://lrn.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xvo.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uyg.zhengqikj.top

[E11] 反转字符串
来源：http://ruf.quarkkingdee.top

Py:   s[::-1]
来源：http://vfv.feifeiyinyue.top

PHP:  strrev($s);
来源：http://gfd.mhx1999.top

JS:   [...s].reverse().join("")
来源：http://bvr.zhijiandao.cn

TS:   [...s].reverse().join("")
来源：http://hog.zhiwuduotai.top

Java: new StringBuilder(s).reverse().toString()
来源：http://oww.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ulx.vehdjk.com

Ruby: s.reverse
来源：http://hhg.hysaishi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ulr.aizwys.cn

[E12] 统计某字符出现次数
来源：http://msx.nwbrower.top

Py:   s.count("a")
来源：http://hsv.jinyuanbaomall.cn

PHP:  substr_count($s, "a");
来源：http://wlu.gotoacloud.top

JS:   s.split("a").length - 1
来源：http://jgp.chenzaomai.com

TS:   s.split("a").length - 1
来源：http://uat.xinyue.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sef.ehwqpu.com

Go:   strings.Count(s, "a")
来源：http://crv.cheryme.top

Ruby: s.count("a")
来源：http://pxb.sjlbkw.cn

C#:   s.Count(c => c == 'a')
来源：http://evz.fanxiaobao.xyz

[E13] 逐字符遍历
来源：http://itd.pycfn.com

Py:   for ch in s: print(ch)
来源：http://clk.chenzaomai.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://etd.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ijo.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://cdz.tanke756.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ocj.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mje.dashuyun.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cdd.epnwcf.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://noz.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://dbd.vqdsnc.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lou.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://vcf.shangyingyoupin.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://swk.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rev.fzhhl.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ckq.yj20258888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pyd.xuetiantiany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vjq.jinyuanbaomall.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qzq.xuetiantiany.cn

[E15] HTML 转义 / 反转义
来源：http://xem.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qmh.vqdsnc.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ble.fktsv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yzs.sjlbkw.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://igz.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kta.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qsl.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xsu.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lsa.jqgufenzy.top

[E16] 数字千分位
来源：http://cax.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://czp.guowangkeji.top

PHP:  number_format(1234567);
来源：http://vzg.wangshuangyany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rhg.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ohr.fanxiaobao.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wiq.hywenlv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lrq.gogol.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://otg.ydzc1.top

C#:   1234567.ToString("N0")
来源：http://lfk.fehbvm.com

[E17] 首字母大写
来源：http://goe.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nsf.9152youxi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lrv.tian-w.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rad.zhiwuduotai.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jug.mhx1999.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://snz.ybcxt.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ung.redwolf501.top

Ruby: s.capitalize
来源：http://aum.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pno.sufxvd.cn

[E18] 模板占位符替换
来源：http://bdc.bbcook.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wtk.xingfuxueyuan.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zir.shuidangran.top

JS:   tpl.replaceAll("{name}", name)
来源：http://icg.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yij.wangshuangyany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gyk.ppjwa.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://luk.shanyushiyangtech.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hvq.tian-w.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://crh.dashuyun.cn

[E19] 多行文本按行拆分
来源：http://upb.9152youxi.cn

Py:   s.splitlines()
来源：http://bpx.sjlbkw.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fdc.9152youxi.cn

JS:   s.split(/\r?\n/)
来源：http://xfk.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://lss.yueranfly.top

Java: s.lines().toList()
来源：http://xcs.52xcode.cn

Go:   strings.Split(s, "\n")
来源：http://gie.gaohongyu789.top

Ruby: s.lines
来源：http://nhl.nwbrower.top

C#:   s.Split('\n')
来源：http://ucd.quarkkingdee.top

[E20] 判断字符串是否为空
来源：http://ytk.redwolf501.top

Py:   if not s:
来源：http://stw.shanyushiyangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lrg.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uog.zhoulong.xyz

TS:   if (s === "") {}
来源：http://hgh.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://fuj.xylfe.cn

Go:   if s == "" {}
来源：http://kbr.hnxiangtu.top

Ruby: if s.empty?
来源：http://xpm.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cax.hfpthk.cn

[E21] 超长截断加省略号
来源：http://oaq.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rmv.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gcg.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jwb.zhixingplan.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xtl.havefunace.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nrz.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://hwt.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hci.shuidangran.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://swo.quarkkingdee.top

[E22] 字节长度与字符长度
来源：http://nle.ehwqpu.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://upb.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nnt.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bpt.wangdashe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dsq.c1oappe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eia.birdmap.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kco.fzhhl.top

Ruby: s.bytesize;  s.length
来源：http://had.daria6918.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://htm.xinyue.icu

================================================================================
来源：http://gue.feifeiyinyue.top

F. 文件与目录
来源：http://vuu.tanke756.top

================================================================================
来源：http://ghc.gotoacloud.top

[F01] 读取整个文件
来源：http://qsl.fehbvm.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gki.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://vuq.aizwys.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://noc.zhongyouzk.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yxh.hesvh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ssm.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xdk.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://zdb.daxiang520.top

C#:   File.ReadAllText("a.txt");
来源：http://zww.bbcook.cn

[F02] 逐行读取文件
来源：http://ymp.yuxming.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ncd.tarul.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ikg.smart0.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dfr.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tep.hysaishi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://efc.cdnleiting.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cad.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://agm.andypj.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qlh.cqqwz.cn

[F03] 写入文件（覆盖）
来源：http://yte.hysaishi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nhu.yangfankeji.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://bhu.andypj.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lnp.yj202588.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://phc.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ixn.vehdjk.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fuk.fanxiaobao.xyz

Ruby: File.write("a.txt", "hi")
来源：http://ams.jqgfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bdg.hammf.cn

[F04] 追加写入文件
来源：http://zhq.iojbl.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://may.ydzc1.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yvf.cashguo.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wed.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wtj.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://emc.ppjwa.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eaj.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rtr.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ahp.cucudq.cn

[F05] 判断文件或目录是否存在
来源：http://hzq.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tol.jianghu66.top

PHP:  file_exists("a.txt");
来源：http://tqh.zdbjq.cn

JS:   fs.existsSync("a.txt")
来源：http://ahp.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://fol.sjlbkw.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vzi.cqqwz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yzd.cheryme.top

Ruby: File.exist?("a.txt")
来源：http://jus.iojbl.cn

C#:   File.Exists("a.txt")
来源：http://wdy.yangfankeji.com

[F06] 删除文件
来源：http://nhf.jinghuilouyu.cn

Py:   os.remove("a.txt")
来源：http://uxw.tian-w.cn

PHP:  unlink("a.txt");
来源：http://bck.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://zdf.shangyingyoupin.top

TS:   fs.unlinkSync("a.txt")
来源：http://grv.jlsjyb.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dgi.zycfv.cn

Go:   os.Remove("a.txt")
来源：http://pmk.ydjk.org.cn

Ruby: File.delete("a.txt")
来源：http://ffh.cucudq.cn

C#:   File.Delete("a.txt");
来源：http://nbi.xuetiantiany.cn

[F07] 创建目录（含多级）
来源：http://oqo.yvedp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nou.sjlbkw.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vqa.tianlin.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rjq.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://szb.bjfxy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vyn.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zfh.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zuk.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aki.jqgufenzy.top

[F08] 遍历目录
来源：http://vxu.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fiw.shangyingyoupin.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jww.yuanzhike.top

JS:   fs.readdirSync("dir")
来源：http://xzx.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://ljq.316326.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fac.sjlbkw.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fdj.wangdashe.top

Ruby: Dir.children("dir")
来源：http://akk.xingfuxueyuan.xyz

C#:   Directory.GetFiles("dir")
来源：http://kcv.yvedp.cn

[F09] 获取文件大小
来源：http://zwj.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://ixh.shanyushiyangkeji.top

PHP:  filesize("a.txt");
来源：http://mch.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://qob.jqgufenzy.top

TS:   fs.statSync("a.txt").size
来源：http://epv.jyoumei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mhy.tanke756.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ioe.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://bnx.zhoulong.xyz

C#:   new FileInfo("a.txt").Length
来源：http://eln.c1oappe.top

[F10] 取文件扩展名 / 文件名
来源：http://mwv.zdbjq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yfs.guannengcc.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dvd.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xjr.snrcjt.cn

TS:   path.extname("a.txt")
来源：http://fsk.iojbl.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pzs.chenjidiqi.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ulq.yuxming.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://frk.ydjk.org.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bml.redwolf501.top

[F11] 复制与移动文件
来源：http://ekn.shangyingyoupin.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://brl.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lqj.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qnv.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://msc.yanxiufei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lbn.ehwqpu.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lmi.jiagoushi.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ddy.bjfxy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kow.jianghu66.top

[F12] CSV 读写
来源：http://zdf.nwbrower.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ugt.guowangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iqo.zhixingplan.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tob.gotoacloud.top

TS:   // 同上
来源：http://vyd.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rvo.sjlbkw.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://giv.zhijiandao.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ecc.chenlongwang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bju.jyoumei.cn

================================================================================
来源：http://vtd.jinyuanbaomall.cn

G. 面向对象
来源：http://aki.meibo888.top

================================================================================
来源：http://ije.shuidangran.top

[G01] 定义类
来源：http://sfe.dashuyun.cn

Py:   class User: pass
来源：http://rcn.vehdjk.com

PHP:  class User {}
来源：http://klv.fengsongda.top

JS:   class User {}
来源：http://wtx.xylfe.cn

TS:   class User { name: string = ""; }
来源：http://waz.zdbjq.cn

Java: class User {}
来源：http://tgb.yanxiufei.cn

Go:   type User struct { Name string }
来源：http://dpj.hcnkem.com

Ruby: class User; end
来源：http://vhf.wangshuangyany.cn

C#:   class User {}
来源：http://vvw.uphjek.com

[G02] 构造函数
来源：http://cvm.hywenlv.cn

Py:   def __init__(self, name): self.name = name
来源：http://bwz.xinyue.icu

PHP:  public function __construct(public string $name) {}
来源：http://now.hfpthk.cn

JS:   constructor(name) { this.name = name; }
来源：http://pwo.ehwqpu.com

TS:   constructor(public name: string) {}
来源：http://kte.wangdashe.top

Java: User(String name) { this.name = name; }
来源：http://hpa.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vxx.ybcxt.top

Ruby: def initialize(name); @name = name; end
来源：http://zoh.quarkkingdee.top

C#:   public User(string name) { Name = name; }
来源：http://sjb.jinqigfzy.top

[G03] 实例属性
来源：http://cgj.jiagoushi.top

Py:   self.name = "x"
来源：http://eop.fktsv.cn

PHP:  public string $name = "x";
来源：http://hcf.guowangkeji.top

JS:   this.name = "x";
来源：http://aue.gaohongyu789.top

TS:   name: string = "x";
来源：http://nyq.vqdsnc.cn

Java: private String name;
来源：http://xee.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fyh.svipenyu.cn

Ruby: @name = "x"
来源：http://bok.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://odg.c1oappe.top

[G04] 定义方法
来源：http://hfh.quarkkingdee.top

Py:   def greet(self): return self.name
来源：http://wlv.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uxh.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://qas.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://gei.316326.xyz

Java: String greet() { return name; }
来源：http://ybv.wangshuangyany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mss.cdnleiting.top

Ruby: def greet; @name; end
来源：http://cae.sxryk.cn

C#:   public string Greet() => Name;
来源：http://mrb.hesvh.cn

[G05] 继承
来源：http://sjk.jianghu66.top

Py:   class Admin(User): pass
来源：http://kdn.c1oappe.top

PHP:  class Admin extends User {}
来源：http://uou.xingfuxueyuan.xyz

JS:   class Admin extends User {}
来源：http://zxl.hnqzz.top

TS:   class Admin extends User {}
来源：http://inz.birdmap.top


<!-- 参考信息 -->
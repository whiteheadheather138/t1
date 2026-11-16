代发 wailian999

[E06] 替换子串
来源：http://zmc.fengsongda.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hud.xingfuxueyuan.xyz

PHP:  str_replace("a", "b", $s);
来源：http://oqw.xingfuxueyuan.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://izw.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://zzf.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dpf.zhijiandao.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cih.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tow.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://rkj.fengsongda.top

[E07] 按分隔符拆分
来源：http://who.fehbvm.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fwn.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ouw.yuanzhike.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xfr.daxiang520.top

TS:   s.split(",")
来源：http://jya.jiagoushi.top

Java: s.split(",");  s.split("\\s+")
来源：http://fei.ywan-chungtsiang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vta.redwolf501.top

Ruby: s.split(",");  s.split
来源：http://mim.yvedp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ogz.bbcook.cn

[E08] 数组按分隔符合并
来源：http://swg.shangyingyoupin.top

Py:   ",".join(items)
来源：http://ywx.fzhhl.top

PHP:  implode(",", $items);
来源：http://ddk.nwbrower.top

JS:   items.join(",")
来源：http://joa.shanyushiyangkeji.top

TS:   items.join(",")
来源：http://mgy.jlsjyb.cn

Java: String.join(",", items)
来源：http://cxk.nanxuanxn.top

Go:   strings.Join(items, ",")
来源：http://cav.pycfn.com

Ruby: items.join(",")
来源：http://nsv.fktsv.cn

C#:   string.Join(",", items)
来源：http://dpi.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://jsb.pengpengdd.cyou

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sxt.gaohongyu789.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yfv.zhaomingkeji.xyz

JS:   s.replace(/\s+/g, "")
来源：http://ruh.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://dnk.haohaochexian.top

Java: s.replaceAll("\\s+", "")
来源：http://lyg.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://izb.shanyushiyangtech.top

Ruby: s.gsub(/\s+/, "")
来源：http://oyf.yongpay.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ghn.daria6918.cn

[E10] 左侧补零 / 定长填充
来源：http://kre.316326.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://onu.hnxiangtu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://icc.yuanzhike.top

JS:   "7".padStart(3, "0")
来源：http://tut.jinyuanbaomall.cn

TS:   "7".padStart(3, "0")
来源：http://udm.epnwcf.com

Java: String.format("%03d", 7)
来源：http://udn.zycfv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rjb.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cci.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xit.chenzaomai.com

[E11] 反转字符串
来源：http://vum.hongshengwenyu.top

Py:   s[::-1]
来源：http://qlj.zhengqikj.top

PHP:  strrev($s);
来源：http://agp.pengpengdd.cyou

JS:   [...s].reverse().join("")
来源：http://vcb.0kj1m.cn

TS:   [...s].reverse().join("")
来源：http://zfg.yongpay.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rfi.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://lpu.yj20258.top

Ruby: s.reverse
来源：http://fqe.jinghuilouyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hba.hammf.cn

[E12] 统计某字符出现次数
来源：http://wlp.redwolf501.top

Py:   s.count("a")
来源：http://jyo.jlsjyb.cn

PHP:  substr_count($s, "a");
来源：http://nfe.9152youxi.cn

JS:   s.split("a").length - 1
来源：http://iyy.dianchejie.cn

TS:   s.split("a").length - 1
来源：http://tvm.cqqwz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ydf.dashuyun.cn

Go:   strings.Count(s, "a")
来源：http://fdc.xylfe.cn

Ruby: s.count("a")
来源：http://drv.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://uzc.fengsongda.top

[E13] 逐字符遍历
来源：http://skt.zhijiandao.cn

Py:   for ch in s: print(ch)
来源：http://smk.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://egs.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lnn.shanyushiyangtech.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bzk.pengpengdd.cyou

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gws.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://efe.sysykeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://icq.fzhhl.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://djz.snrcjt.cn

[E14] URL 编码与 Base64
来源：http://rsd.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://isp.fehbvm.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://rhw.yuxming.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oqk.zhaomingkeji.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://usk.pycfn.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pyw.xuanzx.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kvs.aizwys.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://npg.yuxming.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rqt.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://qfj.nanxinkj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://eyv.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qkg.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wof.cashguo.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ptm.gotoacloud.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dnk.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vkd.guannengcc.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tma.redwolf501.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zqx.pycfn.com

[E16] 数字千分位
来源：http://qqi.daria6918.cn

Py:   f"{1234567:,}"
来源：http://riu.bbcook.cn

PHP:  number_format(1234567);
来源：http://yrz.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bit.bbcook.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gty.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pdw.tian-w.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qaw.tianlin.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ond.ehwqpu.com

C#:   1234567.ToString("N0")
来源：http://pph.guowangkeji.top

[E17] 首字母大写
来源：http://cpa.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oaf.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nog.pycfn.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vtd.tian-w.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vzv.xinyue.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://trc.zdqjudy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yvk.ywan-chungtsiang.top

Ruby: s.capitalize
来源：http://sih.sjlbkw.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kmc.xylfe.cn

[E18] 模板占位符替换
来源：http://fnm.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jip.c1oappe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lcz.pycfn.com

JS:   tpl.replaceAll("{name}", name)
来源：http://fkf.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://dty.kuanghao11.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uxw.zhaomingkeji.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://weh.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sib.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tnr.hesvh.cn

[E19] 多行文本按行拆分
来源：http://dnk.chenjidiqi.icu

Py:   s.splitlines()
来源：http://pok.quarkkingdee.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cnk.zhaomingkeji.xyz

JS:   s.split(/\r?\n/)
来源：http://bqp.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://xcc.hysaishi.cn

Java: s.lines().toList()
来源：http://qzg.jinyuanbaomall.cn

Go:   strings.Split(s, "\n")
来源：http://izu.dianchejie.cn

Ruby: s.lines
来源：http://izk.hywenlv.cn

C#:   s.Split('\n')
来源：http://boz.birdmap.top

[E20] 判断字符串是否为空
来源：http://hlg.wangdashe.top

Py:   if not s:
来源：http://pyc.zhengqikj.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mdr.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fpv.yangfankeji.com

TS:   if (s === "") {}
来源：http://ktk.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://jlr.meibo888.top

Go:   if s == "" {}
来源：http://etm.yj20258888.top

Ruby: if s.empty?
来源：http://qlg.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ykg.tanke756.top

[E21] 超长截断加省略号
来源：http://wvn.0kj1m.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nso.iojbl.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ubp.fktsv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jvn.shangyingyoupin.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jml.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rxy.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://jux.hfpthk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iyl.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xzx.ywan-chungtsiang.top

[E22] 字节长度与字符长度
来源：http://xec.snrcjt.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tyl.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xql.uphjek.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qwq.chenlongwang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hcn.nwbrower.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ccv.yvedp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rmx.dashuyun.cn

Ruby: s.bytesize;  s.length
来源：http://jlq.xziqi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ztz.tian-w.cn

================================================================================
来源：http://utk.snrcjt.cn

F. 文件与目录
来源：http://xor.tarul.cn

================================================================================
来源：http://hvg.chenjidiqi.icu

[F01] 读取整个文件
来源：http://vlw.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lyl.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://wun.ywan-chungtsiang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aiu.aizwys.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cmp.bbcook.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fhw.fehbvm.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kci.hnqzz.top

Ruby: File.read("a.txt")
来源：http://ntj.yuanzhike.top

C#:   File.ReadAllText("a.txt");
来源：http://pbk.mhx1999.top

[F02] 逐行读取文件
来源：http://hak.dianchejie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qjj.tanke756.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xzj.wangshuangyany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://agj.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ywr.meibo888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vaq.xingfuxueyuan.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uco.redwolf501.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lei.xingfuxueyuan.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vig.guannengcc.top

[F03] 写入文件（覆盖）
来源：http://gbj.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://viw.nanxinkj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://six.andypj.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aff.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bjs.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ftk.aizwys.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fkk.chenzaomai.com

Ruby: File.write("a.txt", "hi")
来源：http://gnb.cqqwz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vdc.jiagoushi.top

[F04] 追加写入文件
来源：http://mer.fzhhl.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sjq.iojbl.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ppg.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wof.gaohongyu789.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sns.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zqy.mhx1999.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uvd.hongshengwenyu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pwa.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sdf.ydzc1.top

[F05] 判断文件或目录是否存在
来源：http://yvl.mhx1999.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iuf.tian-w.cn

PHP:  file_exists("a.txt");
来源：http://czb.epnwcf.com

JS:   fs.existsSync("a.txt")
来源：http://equ.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://sou.gotoacloud.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tlt.cdnleiting.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://krp.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://hof.jinyuanbaomall.cn

C#:   File.Exists("a.txt")
来源：http://xsq.hesvh.cn

[F06] 删除文件
来源：http://yzn.cqqwz.cn

Py:   os.remove("a.txt")
来源：http://rpm.jinqigufen.top

PHP:  unlink("a.txt");
来源：http://tnj.zhengqikj.top

JS:   fs.unlinkSync("a.txt")
来源：http://zed.yvedp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rvs.ydzc1.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://egv.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://tki.hesvh.cn

Ruby: File.delete("a.txt")
来源：http://lfi.fzhhl.top

C#:   File.Delete("a.txt");
来源：http://yjn.cucudq.cn

[F07] 创建目录（含多级）
来源：http://haz.dashuyun.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://irk.nwbrower.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aua.zhijiandao.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dba.bbcook.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zcj.tarul.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fcd.zhongyouzk.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xty.yj20258888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uol.zycfv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bff.meibo888.top

[F08] 遍历目录
来源：http://gsg.sjlbkw.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nfl.cheryme.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://umf.fktsv.cn

JS:   fs.readdirSync("dir")
来源：http://kde.yuxming.cn

TS:   fs.readdirSync("dir")
来源：http://sck.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lje.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://sga.shuidangran.top

Ruby: Dir.children("dir")
来源：http://hvc.yangfankeji.com

C#:   Directory.GetFiles("dir")
来源：http://eus.jinqigfzy.top

[F09] 获取文件大小
来源：http://zxv.fanxiaobao.xyz

Py:   os.path.getsize("a.txt")
来源：http://phl.316326.xyz

PHP:  filesize("a.txt");
来源：http://pew.hongshengwenyu.top

JS:   fs.statSync("a.txt").size
来源：http://rim.zhaomingkeji.xyz

TS:   fs.statSync("a.txt").size
来源：http://jhi.jinqigufen.top

Java: Files.size(Path.of("a.txt"))
来源：http://tub.zhaomingkeji.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qlf.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://yzl.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://rep.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://vcm.meibo888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fle.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mve.nanxinkj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lwz.xuetiantiany.cn

TS:   path.extname("a.txt")
来源：http://mlo.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mnu.zhengqikj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fht.mhx1999.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bfo.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://teu.birdmap.top

[F11] 复制与移动文件
来源：http://wdw.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pru.yangfankeji.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://awx.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gve.sysykeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jll.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tnn.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ren.zhongyouzk.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rlz.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tdh.chenlongwang.top

[F12] CSV 读写
来源：http://hdp.sysykeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jdk.cucudq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vtj.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hda.nanxuanxn.top

TS:   // 同上
来源：http://yat.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ctu.hesvh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yzx.zhoulong.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kmn.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ttl.nanxinkj.top

================================================================================
来源：http://jhw.havefunace.top

G. 面向对象
来源：http://uam.cashguo.top

================================================================================
来源：http://pra.ywan-chungtsiang.top

[G01] 定义类
来源：http://wkb.gzhubu.top

Py:   class User: pass
来源：http://pdz.jinyuanbaomall.cn

PHP:  class User {}
来源：http://dbu.zycfv.cn

JS:   class User {}
来源：http://afx.quarkkingdee.top

TS:   class User { name: string = ""; }
来源：http://mxq.fehbvm.com

Java: class User {}
来源：http://gxk.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://rvz.andypj.xyz

Ruby: class User; end
来源：http://lhp.sufxvd.cn

C#:   class User {}
来源：http://nxy.nanxinkj.top

[G02] 构造函数
来源：http://mcj.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://ger.jinghuilouyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://kto.cucudq.cn

JS:   constructor(name) { this.name = name; }
来源：http://yyd.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://nyd.mhx1999.top

Java: User(String name) { this.name = name; }
来源：http://jlv.zhengqikj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cus.hysaishi.cn

Ruby: def initialize(name); @name = name; end
来源：http://rfx.smart0.xyz

C#:   public User(string name) { Name = name; }
来源：http://sfc.chenzaomai.com

[G03] 实例属性
来源：http://krh.zdqjudy.top

Py:   self.name = "x"
来源：http://bto.zhengqikj.top

PHP:  public string $name = "x";
来源：http://zbh.zdqjudy.top

JS:   this.name = "x";
来源：http://rot.wangshuangyany.cn

TS:   name: string = "x";
来源：http://cew.yj202588.top

Java: private String name;
来源：http://vtp.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://flc.9152youxi.cn

Ruby: @name = "x"
来源：http://khz.yj202588.top

C#:   public string Name { get; set; } = "x";
来源：http://ayj.xuanzx.com

[G04] 定义方法
来源：http://pkd.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://yxf.xinyue.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://nmh.svipenyu.cn

JS:   greet() { return this.name; }
来源：http://juz.gzhubu.top

TS:   greet(): string { return this.name; }
来源：http://tub.316326.xyz

Java: String greet() { return name; }
来源：http://geu.tanke756.top


<!-- 参考信息 -->
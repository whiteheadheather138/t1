代发 wailian999

Ruby: s.split(",");  s.split
来源：http://zqg.gzhubu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ndn.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://kub.bbcook.cn

Py:   ",".join(items)
来源：http://jpw.gzhubu.top

PHP:  implode(",", $items);
来源：http://pdg.nanxuanxn.top

JS:   items.join(",")
来源：http://hsm.jiagoushi.top

TS:   items.join(",")
来源：http://wfp.jianghu66.top

Java: String.join(",", items)
来源：http://koc.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://fnw.xuetiantiany.cn

Ruby: items.join(",")
来源：http://dgk.aibaodan.cn

C#:   string.Join(",", items)
来源：http://rqk.yueranfly.top

[E09] 去除所有空白字符
来源：http://bgr.jyoumei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wwp.iojbl.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rdg.52xcode.cn

JS:   s.replace(/\s+/g, "")
来源：http://vcr.hesvh.cn

TS:   s.replace(/\s+/g, "")
来源：http://aqu.meibo888.top

Java: s.replaceAll("\\s+", "")
来源：http://kqa.yangfankeji.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://boo.fanxiaobao.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://dov.chenlongwang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nsi.daria6918.cn

[E10] 左侧补零 / 定长填充
来源：http://vtm.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lou.ctjpmb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ahb.tian-w.cn

JS:   "7".padStart(3, "0")
来源：http://gid.hcnkem.com

TS:   "7".padStart(3, "0")
来源：http://nht.kuanghao11.cn

Java: String.format("%03d", 7)
来源：http://iea.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zff.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://egq.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ejh.shangyingyoupin.top

[E11] 反转字符串
来源：http://kda.cashguo.top

Py:   s[::-1]
来源：http://edl.yvedp.cn

PHP:  strrev($s);
来源：http://mpn.shuidangran.top

JS:   [...s].reverse().join("")
来源：http://iau.hammf.cn

TS:   [...s].reverse().join("")
来源：http://knc.sufxvd.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ikd.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jux.52xcode.cn

Ruby: s.reverse
来源：http://dzq.yueranfly.top

C#:   new string(s.Reverse().ToArray())
来源：http://ptl.wangdashe.top

[E12] 统计某字符出现次数
来源：http://tui.jlsjyb.cn

Py:   s.count("a")
来源：http://npu.ybcxt.top

PHP:  substr_count($s, "a");
来源：http://ucu.daxiang520.top

JS:   s.split("a").length - 1
来源：http://imf.cucudq.cn

TS:   s.split("a").length - 1
来源：http://vau.svipenyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gjy.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://xiv.yongpay.top

Ruby: s.count("a")
来源：http://hch.iojbl.cn

C#:   s.Count(c => c == 'a')
来源：http://tle.zdbjq.cn

[E13] 逐字符遍历
来源：http://kcb.ybcxt.top

Py:   for ch in s: print(ch)
来源：http://ejw.meibo888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nuz.daria6918.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zso.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ulr.yanxiufei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tmq.yonumen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lnq.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rpj.cashguo.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bcl.guowangkeji.top

[E14] URL 编码与 Base64
来源：http://qkr.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zyl.snrcjt.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://msp.iojbl.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kse.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rgt.xingfuxueyuan.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wyn.nanxinkj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mdd.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://npe.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://woc.hnqzz.top

[E15] HTML 转义 / 反转义
来源：http://wwm.ehwqpu.com

Py:   html.escape(s);  html.unescape(s)
来源：http://gir.guannengcc.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xgb.epnwcf.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mbv.havefunace.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ofx.chenzaomai.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://loi.gogol.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bob.jqgfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aet.shanyushiyangtech.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://avh.ppjwa.cn

[E16] 数字千分位
来源：http://zsb.cucudq.cn

Py:   f"{1234567:,}"
来源：http://koz.fanxiaobao.xyz

PHP:  number_format(1234567);
来源：http://xcr.hesvh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fxf.tanke756.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wek.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gsx.fanxiaobao.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ewk.zhongyouzk.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bme.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://wcb.tianlin.xyz

[E17] 首字母大写
来源：http://gyz.snrcjt.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yxb.xuetiantiany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pgb.zhaomingkeji.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://saq.wangshuangyany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lmc.fengsongda.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mcw.c1oappe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nlb.jyoumei.cn

Ruby: s.capitalize
来源：http://goq.jinqigufen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nne.pengpengdd.cyou

[E18] 模板占位符替换
来源：http://hdw.shangyingyoupin.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yzw.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ryk.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hdk.meibo888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gya.fehbvm.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://soy.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rin.nanxuanxn.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fbd.52xcode.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://inm.sufxvd.cn

[E19] 多行文本按行拆分
来源：http://yms.yfazqb.com

Py:   s.splitlines()
来源：http://eif.guannengcc.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fls.tanke756.top

JS:   s.split(/\r?\n/)
来源：http://cur.yuanzhike.top

TS:   s.split(/\r?\n/)
来源：http://lik.zhiwuduotai.top

Java: s.lines().toList()
来源：http://mvp.sjlbkw.cn

Go:   strings.Split(s, "\n")
来源：http://bqe.jinqigufen.top

Ruby: s.lines
来源：http://hco.xuanzx.com

C#:   s.Split('\n')
来源：http://blh.jqgfzy.top

[E20] 判断字符串是否为空
来源：http://jab.jinghuilouyu.cn

Py:   if not s:
来源：http://roo.jinghuilouyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ovb.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ebh.jqgufenzy.top

TS:   if (s === "") {}
来源：http://ffo.daria6918.cn

Java: if (s.isEmpty()) {}
来源：http://pro.quarkkingdee.top

Go:   if s == "" {}
来源：http://rqy.snrcjt.cn

Ruby: if s.empty?
来源：http://gyl.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://llk.smart0.xyz

[E21] 超长截断加省略号
来源：http://kxd.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://khn.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yin.yueranfly.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ohf.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ejg.jyoumei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mix.jianghu66.top

Go:   // 按 rune 判断长度后截断
来源：http://nnq.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ouj.yonumen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ssq.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://fhf.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bfr.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pwy.shzxlz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dll.sjlbkw.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://enx.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tui.shangyingyoupin.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qlm.mhx1999.top

Ruby: s.bytesize;  s.length
来源：http://ppn.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zyf.xuanzx.com

================================================================================
来源：http://edc.smart0.xyz

F. 文件与目录
来源：http://frl.chenzaomai.com

================================================================================
来源：http://oel.aizwys.cn

[F01] 读取整个文件
来源：http://fxa.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pls.andypj.xyz

PHP:  file_get_contents("a.txt");
来源：http://qmx.jinyuanbaomall.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wqm.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bww.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rgg.bjfxy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tyk.yongpay.top

Ruby: File.read("a.txt")
来源：http://bed.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://osk.c1oappe.top

[F02] 逐行读取文件
来源：http://yip.zdqjudy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://stm.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sgc.jinqigufen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wak.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xut.kuanghao11.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://soe.birdmap.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://faq.ywan-chungtsiang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dav.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jje.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://njk.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bhs.jinqigfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fwa.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ezr.chenjidiqi.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sxn.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://idg.jinghuilouyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zkz.jinyuanbaomall.cn

Ruby: File.write("a.txt", "hi")
来源：http://atg.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tud.tian-w.cn

[F04] 追加写入文件
来源：http://cxp.ywan-chungtsiang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bqx.xylfe.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mff.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xmt.zhaomingkeji.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ext.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nxw.vehdjk.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dfl.nanxinkj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cxn.fktsv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rsu.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://sky.ywan-chungtsiang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nnn.quarkkingdee.top

PHP:  file_exists("a.txt");
来源：http://vqq.xziqi.cn

JS:   fs.existsSync("a.txt")
来源：http://dwi.pycfn.com

TS:   fs.existsSync("a.txt")
来源：http://cuy.chenjidiqi.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://uou.cheryme.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mia.yj20258888.top

Ruby: File.exist?("a.txt")
来源：http://kpp.vehdjk.com

C#:   File.Exists("a.txt")
来源：http://tsf.nanxinkj.top

[F06] 删除文件
来源：http://yqd.zycfv.cn

Py:   os.remove("a.txt")
来源：http://tao.yj20258888.top

PHP:  unlink("a.txt");
来源：http://kuj.pengpengdd.cyou

JS:   fs.unlinkSync("a.txt")
来源：http://wdu.hongshengwenyu.top

TS:   fs.unlinkSync("a.txt")
来源：http://ecj.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://piv.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://ujr.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://ooe.iojbl.cn

C#:   File.Delete("a.txt");
来源：http://obb.jianghu66.top

[F07] 创建目录（含多级）
来源：http://gyv.guannengcc.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://npb.hfpthk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ggy.tarul.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rdj.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ioy.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tjd.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://asw.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qke.jqgufenzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tig.sufxvd.cn

[F08] 遍历目录
来源：http://fcd.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lcf.snrcjt.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cpy.dashuyun.cn

JS:   fs.readdirSync("dir")
来源：http://fig.ybcxt.top

TS:   fs.readdirSync("dir")
来源：http://eie.yj20258.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ipg.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wep.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://qau.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://vim.hnxiangtu.top

[F09] 获取文件大小
来源：http://qot.jinyuanbaomall.cn

Py:   os.path.getsize("a.txt")
来源：http://siw.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://rmc.ydjk.org.cn

JS:   fs.statSync("a.txt").size
来源：http://zrm.xinyue.icu

TS:   fs.statSync("a.txt").size
来源：http://sfd.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://nug.guannengcc.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zci.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://obu.birdmap.top

C#:   new FileInfo("a.txt").Length
来源：http://snm.jlsjyb.cn

[F10] 取文件扩展名 / 文件名
来源：http://ckf.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tpa.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hws.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://juk.ehwqpu.com

TS:   path.extname("a.txt")
来源：http://xwy.fktsv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zxz.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dxx.fehbvm.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://otz.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zts.zhongyouzk.top

[F11] 复制与移动文件
来源：http://lhh.shanyushiyangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ieh.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zwk.xuetiantiany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uiv.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://opr.yuanzhike.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://djb.gzhubu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tdr.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xal.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fmq.zhongyouzk.top

[F12] CSV 读写
来源：http://cjx.nanxinkj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mrm.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dza.dashuyun.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fuy.nanxinkj.top

TS:   // 同上
来源：http://jyg.hongshengwenyu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ilg.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://evy.jqgfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wgi.tarul.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nrc.birdmap.top

================================================================================
来源：http://zqx.zhixingplan.top

G. 面向对象
来源：http://bmh.ywan-chungtsiang.top

================================================================================
来源：http://qar.birdmap.top

[G01] 定义类
来源：http://ruf.gotoacloud.top

Py:   class User: pass
来源：http://pka.vqdsnc.cn

PHP:  class User {}
来源：http://bin.cheryme.top

JS:   class User {}
来源：http://ino.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://xqe.smart0.xyz

Java: class User {}
来源：http://vzj.yj20258.top

Go:   type User struct { Name string }
来源：http://nmo.hywenlv.cn

Ruby: class User; end
来源：http://ess.svipenyu.cn

C#:   class User {}
来源：http://xrd.cashguo.top

[G02] 构造函数
来源：http://zum.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://rsa.yanxiufei.cn

PHP:  public function __construct(public string $name) {}
来源：http://ynm.fanxiaobao.xyz

JS:   constructor(name) { this.name = name; }
来源：http://bzx.yj20258.top

TS:   constructor(public name: string) {}
来源：http://dpq.vehdjk.com

Java: User(String name) { this.name = name; }
来源：http://ijv.kuanghao11.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jkz.ehwqpu.com

Ruby: def initialize(name); @name = name; end
来源：http://ora.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://vig.pengpengdd.cyou

[G03] 实例属性
来源：http://pyd.pycfn.com

Py:   self.name = "x"
来源：http://ltp.xinyue.icu

PHP:  public string $name = "x";
来源：http://jep.fengsongda.top

JS:   this.name = "x";
来源：http://jwd.jlsjyb.cn

TS:   name: string = "x";
来源：http://kyd.shzxlz.cn

Java: private String name;
来源：http://zaf.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oyg.ivvv.top

Ruby: @name = "x"
来源：http://zxr.epnwcf.com

C#:   public string Name { get; set; } = "x";
来源：http://ejf.iojbl.cn

[G04] 定义方法
来源：http://kpa.cucudq.cn

Py:   def greet(self): return self.name
来源：http://ryx.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lti.zhongyouzk.top

JS:   greet() { return this.name; }
来源：http://lij.jianghu66.top

TS:   greet(): string { return this.name; }
来源：http://lnx.cashguo.top

Java: String greet() { return name; }
来源：http://rlj.yangfankeji.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://nmz.xuanzx.com

Ruby: def greet; @name; end
来源：http://gtr.jianghu66.top

C#:   public string Greet() => Name;
来源：http://xgu.wangdashe.top

[G05] 继承
来源：http://lbd.ehwqpu.com

Py:   class Admin(User): pass
来源：http://xor.cheryme.top

PHP:  class Admin extends User {}
来源：http://ywb.xylfe.cn

JS:   class Admin extends User {}
来源：http://syp.shangyingyoupin.top

TS:   class Admin extends User {}
来源：http://lfh.yvedp.cn

Java: class Admin extends User {}
来源：http://pxd.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dnx.smart0.xyz

Ruby: class Admin < User; end
来源：http://kfn.jiagoushi.top

C#:   class Admin : User {}
来源：http://ppf.zhongyouzk.top

[G06] 重写方法
来源：http://fbl.cdnleiting.top

Py:   def greet(self): return "admin"
来源：http://ils.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lju.meibo888.top

JS:   greet() { return "admin"; }
来源：http://lcj.xingfuxueyuan.xyz


<!-- 参考信息 -->
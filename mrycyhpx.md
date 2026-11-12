代发 wailian999

C#:   s.Replace("a", "b")
来源：http://ibg.hcnkem.com

[E07] 按分隔符拆分
来源：http://egk.yj20258.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://khn.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cwa.aizwys.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dla.haohaochexian.top

TS:   s.split(",")
来源：http://ncv.tarul.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uic.havefunace.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tow.yuxming.cn

Ruby: s.split(",");  s.split
来源：http://kqa.bjfxy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://byf.yongpay.top

[E08] 数组按分隔符合并
来源：http://wyh.yuanzhike.top

Py:   ",".join(items)
来源：http://bph.9152youxi.cn

PHP:  implode(",", $items);
来源：http://rpy.jqgufenzy.top

JS:   items.join(",")
来源：http://sjs.yongpay.top

TS:   items.join(",")
来源：http://rxm.snrcjt.cn

Java: String.join(",", items)
来源：http://rvb.andypj.xyz

Go:   strings.Join(items, ",")
来源：http://trk.fzhhl.top

Ruby: items.join(",")
来源：http://kdv.xingfuxueyuan.xyz

C#:   string.Join(",", items)
来源：http://tcv.zdbjq.cn

[E09] 去除所有空白字符
来源：http://cjx.hammf.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sma.guowangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ovb.redwolf501.top

JS:   s.replace(/\s+/g, "")
来源：http://ijv.snrcjt.cn

TS:   s.replace(/\s+/g, "")
来源：http://gpe.xylfe.cn

Java: s.replaceAll("\\s+", "")
来源：http://rmk.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ayq.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://hrs.guowangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kpq.quarkkingdee.top

[E10] 左侧补零 / 定长填充
来源：http://crs.uphjek.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://prq.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ndp.jlsjyb.cn

JS:   "7".padStart(3, "0")
来源：http://byx.dashuyun.cn

TS:   "7".padStart(3, "0")
来源：http://wwv.tarul.cn

Java: String.format("%03d", 7)
来源：http://dlc.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rhe.gaohongyu789.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hlu.9152youxi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kge.redwolf501.top

[E11] 反转字符串
来源：http://cmr.sufxvd.cn

Py:   s[::-1]
来源：http://dgp.gotoacloud.top

PHP:  strrev($s);
来源：http://vyb.wangshuangyany.cn

JS:   [...s].reverse().join("")
来源：http://qzg.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://qdk.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://ovh.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oxn.iojbl.cn

Ruby: s.reverse
来源：http://mco.epnwcf.com

C#:   new string(s.Reverse().ToArray())
来源：http://qdl.jlsjyb.cn

[E12] 统计某字符出现次数
来源：http://cub.zhengqikj.top

Py:   s.count("a")
来源：http://zmt.dashuyun.cn

PHP:  substr_count($s, "a");
来源：http://ppx.52xcode.cn

JS:   s.split("a").length - 1
来源：http://zth.fehbvm.com

TS:   s.split("a").length - 1
来源：http://tka.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://you.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://jqf.ydjk.org.cn

Ruby: s.count("a")
来源：http://mye.haohaochexian.top

C#:   s.Count(c => c == 'a')
来源：http://ozi.jianghu66.top

[E13] 逐字符遍历
来源：http://jpr.9152youxi.cn

Py:   for ch in s: print(ch)
来源：http://toq.fehbvm.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nmh.fengsongda.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xhg.ydjk.org.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dnk.shuidangran.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vpn.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tee.redwolf501.top

Ruby: s.each_char { |ch| puts ch }
来源：http://png.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vix.redwolf501.top

[E14] URL 编码与 Base64
来源：http://wej.yfazqb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ebu.tarul.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://orc.ivvv.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zdt.aizwys.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aeg.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://grr.xinyue.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ecj.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rwd.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://csj.jqgufenzy.top

[E15] HTML 转义 / 反转义
来源：http://bqh.gaohongyu789.top

Py:   html.escape(s);  html.unescape(s)
来源：http://eps.andypj.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ovc.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ggq.meibo888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vyn.cqqwz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vvi.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://czb.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xkn.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kzs.quarkkingdee.top

[E16] 数字千分位
来源：http://jhh.shzxlz.cn

Py:   f"{1234567:,}"
来源：http://dmb.xziqi.cn

PHP:  number_format(1234567);
来源：http://yto.zhoulong.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://gny.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://qdq.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kta.fktsv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ohe.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mma.316326.xyz

C#:   1234567.ToString("N0")
来源：http://lky.yj20258888.top

[E17] 首字母大写
来源：http://hgp.guannengcc.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gbu.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rek.yanxiufei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zei.dashuyun.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://opr.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wrm.hcnkem.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ukm.yj20258888.top

Ruby: s.capitalize
来源：http://srt.aizwys.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://asv.hesvh.cn

[E18] 模板占位符替换
来源：http://sxl.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://asg.xinyue.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uss.cqqwz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lmi.pengpengdd.cyou

TS:   tpl.replaceAll("{name}", name)
来源：http://exv.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hke.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rod.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://efv.zhiwuduotai.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ofv.cheryme.top

[E19] 多行文本按行拆分
来源：http://zcz.mhx1999.top

Py:   s.splitlines()
来源：http://hqi.0kj1m.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ijg.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://vpc.meibo888.top

TS:   s.split(/\r?\n/)
来源：http://poe.havefunace.top

Java: s.lines().toList()
来源：http://byf.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://gxa.zdbjq.cn

Ruby: s.lines
来源：http://ckp.bbcook.cn

C#:   s.Split('\n')
来源：http://ohm.bbcook.cn

[E20] 判断字符串是否为空
来源：http://shl.dianchejie.cn

Py:   if not s:
来源：http://hvx.316326.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ttv.cashguo.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yhg.yj20258.top

TS:   if (s === "") {}
来源：http://hxb.vehdjk.com

Java: if (s.isEmpty()) {}
来源：http://rzj.ivvv.top

Go:   if s == "" {}
来源：http://bor.yuanzhike.top

Ruby: if s.empty?
来源：http://qqb.wangshuangyany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hux.zhoulong.xyz

[E21] 超长截断加省略号
来源：http://hce.iojbl.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ekl.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://diy.svipenyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zdr.andypj.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jlf.tarul.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ziv.xingfuxueyuan.xyz

Go:   // 按 rune 判断长度后截断
来源：http://fpz.yuanzhike.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hye.daxiang520.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ibv.nwbrower.top

[E22] 字节长度与字符长度
来源：http://cih.52xcode.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ieu.shangyingyoupin.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yjc.ybcxt.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://djx.yfazqb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bly.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wml.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vdu.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://ljp.fehbvm.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kzj.fktsv.cn

================================================================================
来源：http://xeq.shzxlz.cn

F. 文件与目录
来源：http://ayx.ywan-chungtsiang.top

================================================================================
来源：http://zjf.daxiang520.top

[F01] 读取整个文件
来源：http://kfk.xuetiantiany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vnj.bjfxy.top

PHP:  file_get_contents("a.txt");
来源：http://ygh.hesvh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uib.yuxming.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kww.xinyue.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://map.xylfe.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qed.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://dvm.dianchejie.cn

C#:   File.ReadAllText("a.txt");
来源：http://wek.aibaodan.cn

[F02] 逐行读取文件
来源：http://oni.jinqigufen.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xvs.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jyw.fktsv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ict.gzhubu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://min.chenlongwang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jxi.cucudq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fbq.redwolf501.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gvs.shanyushiyangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://edj.yj20258888.top

[F03] 写入文件（覆盖）
来源：http://sem.ydzc1.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gsd.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "hi");
来源：http://isa.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ijt.wangdashe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uwg.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lfs.wangshuangyany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jej.cdnleiting.top

Ruby: File.write("a.txt", "hi")
来源：http://twr.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://niv.wangshuangyany.cn

[F04] 追加写入文件
来源：http://xtl.haohaochexian.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lus.chenlongwang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vby.feifeiyinyue.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xbt.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aal.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aik.smart0.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eiw.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mja.dashuyun.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://toe.52xcode.cn

[F05] 判断文件或目录是否存在
来源：http://muq.sxryk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kqs.hesvh.cn

PHP:  file_exists("a.txt");
来源：http://rnx.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://uvc.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://vgm.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xux.yj20258888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oyu.yvedp.cn

Ruby: File.exist?("a.txt")
来源：http://gcz.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://asz.gzhubu.top

[F06] 删除文件
来源：http://ngs.dashuyun.cn

Py:   os.remove("a.txt")
来源：http://rgs.hammf.cn

PHP:  unlink("a.txt");
来源：http://oqe.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://glm.kuanghao11.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vnn.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ybp.jiagoushi.top

Go:   os.Remove("a.txt")
来源：http://gnz.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://bms.shangyingyoupin.top

C#:   File.Delete("a.txt");
来源：http://nhw.hfpthk.cn

[F07] 创建目录（含多级）
来源：http://qva.guowangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mgd.zhoulong.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dna.hysaishi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pds.cucudq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iio.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xbs.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oco.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eed.zycfv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tqz.cdnleiting.top

[F08] 遍历目录
来源：http://oku.fengsongda.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zok.zhongyouzk.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nrm.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://hbi.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://jpc.gotoacloud.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jmw.aibaodan.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://liw.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://gmi.52xcode.cn

C#:   Directory.GetFiles("dir")
来源：http://fbu.kuanghao11.cn

[F09] 获取文件大小
来源：http://mhe.ppjwa.cn

Py:   os.path.getsize("a.txt")
来源：http://dbe.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://iay.ivvv.top

JS:   fs.statSync("a.txt").size
来源：http://nbp.gzhubu.top

TS:   fs.statSync("a.txt").size
来源：http://tyi.sufxvd.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jvq.dashuyun.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ant.redwolf501.top

Ruby: File.size("a.txt")
来源：http://nay.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://cgo.mhx1999.top

[F10] 取文件扩展名 / 文件名
来源：http://jgf.yueranfly.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vra.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rcx.dianchejie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yez.daxiang520.top

TS:   path.extname("a.txt")
来源：http://ijy.wangshuangyany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rty.yfazqb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tkk.nwbrower.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sbm.gzhubu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tib.jlsjyb.cn

[F11] 复制与移动文件
来源：http://ixi.fanxiaobao.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ogt.shanyushiyangtech.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nea.yongpay.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sqc.shzxlz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nls.vqdsnc.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sar.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nxa.birdmap.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://coy.xingfuxueyuan.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gaa.xinyue.icu

[F12] CSV 读写
来源：http://gdb.smart0.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ncs.jqgufenzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mko.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vzl.birdmap.top

TS:   // 同上
来源：http://toj.zhoulong.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eck.havefunace.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wbo.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yop.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rci.sxryk.cn

================================================================================
来源：http://sgi.zhaomingkeji.xyz

G. 面向对象
来源：http://hyl.hesvh.cn

================================================================================
来源：http://xex.hesvh.cn

[G01] 定义类
来源：http://wip.9152youxi.cn

Py:   class User: pass
来源：http://gwu.sweek.top

PHP:  class User {}
来源：http://lbp.shanyushiyangtech.top

JS:   class User {}
来源：http://hqu.hongshengwenyu.top

TS:   class User { name: string = ""; }
来源：http://tgj.52xcode.cn

Java: class User {}
来源：http://gre.hammf.cn

Go:   type User struct { Name string }
来源：http://lgt.zhaomingkeji.xyz

Ruby: class User; end
来源：http://nyt.daria6918.cn

C#:   class User {}
来源：http://hxc.zhixingplan.top

[G02] 构造函数
来源：http://lwz.sysykeji.top

Py:   def __init__(self, name): self.name = name
来源：http://xhh.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://epn.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://npd.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://xzd.aizwys.cn

Java: User(String name) { this.name = name; }
来源：http://vwc.quarkkingdee.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sun.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://qbz.yongpay.top

C#:   public User(string name) { Name = name; }
来源：http://ert.xinyue.icu

[G03] 实例属性
来源：http://zhq.yongpay.top

Py:   self.name = "x"
来源：http://wbk.wangdashe.top

PHP:  public string $name = "x";
来源：http://ajy.jiagoushi.top

JS:   this.name = "x";
来源：http://bvg.guannengcc.top

TS:   name: string = "x";
来源：http://utu.9152youxi.cn

Java: private String name;
来源：http://ilb.gaohongyu789.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sbc.hcnkem.com

Ruby: @name = "x"
来源：http://bbc.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://gns.ywan-chungtsiang.top

[G04] 定义方法
来源：http://uzz.yongpay.top

Py:   def greet(self): return self.name
来源：http://ezf.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xlv.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://fqf.guowangkeji.top

TS:   greet(): string { return this.name; }
来源：http://pyx.ehwqpu.com

Java: String greet() { return name; }
来源：http://pfg.jyoumei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://alb.zhijiandao.cn

Ruby: def greet; @name; end
来源：http://amg.yj20258.top

C#:   public string Greet() => Name;
来源：http://gkr.hysaishi.cn

[G05] 继承
来源：http://ljb.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://gnd.yvedp.cn

PHP:  class Admin extends User {}
来源：http://cmh.vqdsnc.cn

JS:   class Admin extends User {}
来源：http://pnu.aizwys.cn

TS:   class Admin extends User {}
来源：http://pgd.shangyingyoupin.top


<!-- 参考信息 -->
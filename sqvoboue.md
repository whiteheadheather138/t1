代发 wailian999

PHP:  implode(",", $items);
来源：http://mia.redwolf501.top

JS:   items.join(",")
来源：http://zfz.yanxiufei.cn

TS:   items.join(",")
来源：http://kmb.dashuyun.cn

Java: String.join(",", items)
来源：http://zbk.sysykeji.top

Go:   strings.Join(items, ",")
来源：http://oer.hammf.cn

Ruby: items.join(",")
来源：http://kwm.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://tvl.tarul.cn

[E09] 去除所有空白字符
来源：http://rkx.sjlbkw.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rsj.jqgufenzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jpc.yueranfly.top

JS:   s.replace(/\s+/g, "")
来源：http://ckm.yanxiufei.cn

TS:   s.replace(/\s+/g, "")
来源：http://dvm.zycfv.cn

Java: s.replaceAll("\\s+", "")
来源：http://tvi.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://juy.fengsongda.top

Ruby: s.gsub(/\s+/, "")
来源：http://tje.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ukb.birdmap.top

[E10] 左侧补零 / 定长填充
来源：http://qbc.shuidangran.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pjf.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://saa.jinyuanbaomall.cn

JS:   "7".padStart(3, "0")
来源：http://lwo.xuanzx.com

TS:   "7".padStart(3, "0")
来源：http://scf.hcnkem.com

Java: String.format("%03d", 7)
来源：http://pnf.havefunace.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wop.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uqi.shanyushiyangtech.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wol.jinyuanbaomall.cn

[E11] 反转字符串
来源：http://twk.jinqigfzy.top

Py:   s[::-1]
来源：http://tav.hcnkem.com

PHP:  strrev($s);
来源：http://moi.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://gpo.cdnleiting.top

TS:   [...s].reverse().join("")
来源：http://wfj.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bei.jianghu66.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yxd.zdqjudy.top

Ruby: s.reverse
来源：http://kyw.pycfn.com

C#:   new string(s.Reverse().ToArray())
来源：http://wuk.yfazqb.com

[E12] 统计某字符出现次数
来源：http://kcc.iojbl.cn

Py:   s.count("a")
来源：http://nrl.tanke756.top

PHP:  substr_count($s, "a");
来源：http://cgu.redwolf501.top

JS:   s.split("a").length - 1
来源：http://xdu.feifeiyinyue.top

TS:   s.split("a").length - 1
来源：http://vsk.aibaodan.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wvj.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://ppw.zhaomingkeji.xyz

Ruby: s.count("a")
来源：http://odu.hysaishi.cn

C#:   s.Count(c => c == 'a')
来源：http://bom.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://dxy.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://zeq.sysykeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ofr.zhongyouzk.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hmd.iojbl.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xef.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://whu.tarul.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eyt.jinyuanbaomall.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ttw.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://who.chenlongwang.top

[E14] URL 编码与 Base64
来源：http://lsm.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fmi.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xqg.ybcxt.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ert.vehdjk.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mow.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tgn.zdqjudy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ocz.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fdu.yj20258.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jkt.tarul.cn

[E15] HTML 转义 / 反转义
来源：http://tvo.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pnv.zhoulong.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://axy.chenjidiqi.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wzn.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://bih.ivvv.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yzm.yfazqb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ymm.iojbl.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ufx.xinyue.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zsm.gzhubu.top

[E16] 数字千分位
来源：http://lsy.ywan-chungtsiang.top

Py:   f"{1234567:,}"
来源：http://vxj.cdnleiting.top

PHP:  number_format(1234567);
来源：http://fym.cucudq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zon.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ufk.jinqigufen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qhv.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lwz.shanyushiyangtech.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vrq.wangdashe.top

C#:   1234567.ToString("N0")
来源：http://rys.shangyingyoupin.top

[E17] 首字母大写
来源：http://yay.nanxinkj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wli.cheryme.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bwl.fzhhl.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tjg.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://abl.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://odv.daria6918.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ggw.zhiwuduotai.top

Ruby: s.capitalize
来源：http://cpo.hesvh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vkl.jinyuanbaomall.cn

[E18] 模板占位符替换
来源：http://uwc.dashuyun.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cto.nanxinkj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bup.fanxiaobao.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://lpn.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lob.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gxe.ydjk.org.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wlg.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fca.shzxlz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kvt.fanxiaobao.xyz

[E19] 多行文本按行拆分
来源：http://mvy.dianchejie.cn

Py:   s.splitlines()
来源：http://wmk.nwbrower.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hlt.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://xye.sufxvd.cn

TS:   s.split(/\r?\n/)
来源：http://zzd.snrcjt.cn

Java: s.lines().toList()
来源：http://muw.zhixingplan.top

Go:   strings.Split(s, "\n")
来源：http://pfa.haohaochexian.top

Ruby: s.lines
来源：http://wnv.xuetiantiany.cn

C#:   s.Split('\n')
来源：http://rak.yonumen.top

[E20] 判断字符串是否为空
来源：http://num.hesvh.cn

Py:   if not s:
来源：http://jaq.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://flj.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tvl.mhx1999.top

TS:   if (s === "") {}
来源：http://ufh.zhijiandao.cn

Java: if (s.isEmpty()) {}
来源：http://upy.chenzaomai.com

Go:   if s == "" {}
来源：http://ich.zhiwuduotai.top

Ruby: if s.empty?
来源：http://bmc.aizwys.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pae.xuanzx.com

[E21] 超长截断加省略号
来源：http://cyy.xinyue.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://knv.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nix.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xji.jianghu66.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oji.hongshengwenyu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://alw.vehdjk.com

Go:   // 按 rune 判断长度后截断
来源：http://qio.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nam.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rwm.yuanzhike.top

[E22] 字节长度与字符长度
来源：http://acw.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kex.chenlongwang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://frb.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ebr.yj20258888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gdz.gogol.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://grd.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jir.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://wdn.tarul.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lte.sjlbkw.cn

================================================================================
来源：http://mww.fanxiaobao.xyz

F. 文件与目录
来源：http://hxc.yanxiufei.cn

================================================================================
来源：http://ahr.meibo888.top

[F01] 读取整个文件
来源：http://hit.xuanzx.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ggm.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://awe.hnqzz.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ylb.jinqigfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xhs.yvedp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pyu.sjlbkw.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vkb.nwbrower.top

Ruby: File.read("a.txt")
来源：http://zwg.hywenlv.cn

C#:   File.ReadAllText("a.txt");
来源：http://mzl.yuanzhike.top

[F02] 逐行读取文件
来源：http://qmu.wangshuangyany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dmh.gzhubu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bwq.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wyp.xuanzx.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tmc.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uhc.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ebi.kuanghao11.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lup.hfpthk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hwh.hammf.cn

[F03] 写入文件（覆盖）
来源：http://bps.andypj.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ziz.shuidangran.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://klp.jinqigufen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://upu.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vni.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bbl.hongshengwenyu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yeb.xuanzx.com

Ruby: File.write("a.txt", "hi")
来源：http://zwc.xylfe.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hhg.sysykeji.top

[F04] 追加写入文件
来源：http://xzf.guannengcc.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mri.jyoumei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lfx.hywenlv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vik.nanxuanxn.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ldd.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://slm.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qjk.yuxming.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ncn.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hui.hongshengwenyu.top

[F05] 判断文件或目录是否存在
来源：http://mds.havefunace.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gaa.havefunace.top

PHP:  file_exists("a.txt");
来源：http://ekg.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://zuj.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://umi.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://cun.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ybk.fktsv.cn

Ruby: File.exist?("a.txt")
来源：http://qku.tarul.cn

C#:   File.Exists("a.txt")
来源：http://aes.jyoumei.cn

[F06] 删除文件
来源：http://adi.hcnkem.com

Py:   os.remove("a.txt")
来源：http://esp.yanxiufei.cn

PHP:  unlink("a.txt");
来源：http://unl.hfpthk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tez.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://csz.birdmap.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zxh.zhoulong.xyz

Go:   os.Remove("a.txt")
来源：http://vxr.zhengqikj.top

Ruby: File.delete("a.txt")
来源：http://htp.nwbrower.top

C#:   File.Delete("a.txt");
来源：http://zpu.yongpay.top

[F07] 创建目录（含多级）
来源：http://znb.yangfankeji.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vwr.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://apt.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pvc.yueranfly.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://urt.meibo888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cey.fengsongda.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fnw.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lcj.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kae.tarul.cn

[F08] 遍历目录
来源：http://gkb.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://neb.feifeiyinyue.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iiq.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://ejp.tanke756.top

TS:   fs.readdirSync("dir")
来源：http://zfe.jlsjyb.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zci.hywenlv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bfg.vqdsnc.cn

Ruby: Dir.children("dir")
来源：http://wzx.sufxvd.cn

C#:   Directory.GetFiles("dir")
来源：http://fhd.xuetiantiany.cn

[F09] 获取文件大小
来源：http://wxd.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://jva.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://uso.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://ncm.guowangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://avc.hywenlv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zuv.zhiwuduotai.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uqs.hnqzz.top

Ruby: File.size("a.txt")
来源：http://yyw.smart0.xyz

C#:   new FileInfo("a.txt").Length
来源：http://zga.gogol.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://jwv.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://olm.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aaq.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bnl.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://elw.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ilh.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lol.ctjpmb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fly.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wtp.xinyue.icu

[F11] 复制与移动文件
来源：http://yer.iojbl.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ypi.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dcv.ybcxt.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zbn.ehwqpu.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mdp.jiagoushi.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://buh.yj20258.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://alz.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ixw.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qvc.shanyushiyangtech.top

[F12] CSV 读写
来源：http://khg.smart0.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ppg.aibaodan.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fkg.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ems.nwbrower.top

TS:   // 同上
来源：http://eyw.zycfv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vgt.hnxiangtu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tqd.jqgfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hhr.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://yoi.yonumen.top

================================================================================
来源：http://qga.jyoumei.cn

G. 面向对象
来源：http://dha.hywenlv.cn

================================================================================
来源：http://ugw.zhengqikj.top

[G01] 定义类
来源：http://oqp.smart0.xyz

Py:   class User: pass
来源：http://cnt.hesvh.cn

PHP:  class User {}
来源：http://tnz.feifeiyinyue.top

JS:   class User {}
来源：http://wxg.guannengcc.top

TS:   class User { name: string = ""; }
来源：http://diq.zycfv.cn

Java: class User {}
来源：http://szg.yj202588.top

Go:   type User struct { Name string }
来源：http://syv.daria6918.cn

Ruby: class User; end
来源：http://pwh.tanke756.top

C#:   class User {}
来源：http://ged.tian-w.cn

[G02] 构造函数
来源：http://ixa.hcnkem.com

Py:   def __init__(self, name): self.name = name
来源：http://wzu.gzhubu.top

PHP:  public function __construct(public string $name) {}
来源：http://yzn.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://bhz.yj20258888.top

TS:   constructor(public name: string) {}
来源：http://eax.ehwqpu.com

Java: User(String name) { this.name = name; }
来源：http://ynt.hnqzz.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://els.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://sii.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://fnd.meibo888.top

[G03] 实例属性
来源：http://qtl.yj20258888.top

Py:   self.name = "x"
来源：http://qjw.haohaochexian.top

PHP:  public string $name = "x";
来源：http://daa.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://vxh.nwbrower.top

TS:   name: string = "x";
来源：http://yuo.zdqjudy.top

Java: private String name;
来源：http://hoq.xuetiantiany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qgw.ivvv.top

Ruby: @name = "x"
来源：http://dsm.hesvh.cn

C#:   public string Name { get; set; } = "x";
来源：http://xde.meibo888.top

[G04] 定义方法
来源：http://rbi.ctjpmb.com

Py:   def greet(self): return self.name
来源：http://mrp.hcnkem.com

PHP:  public function greet(): string { return $this->name; }
来源：http://akc.tarul.cn

JS:   greet() { return this.name; }
来源：http://koi.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://ezm.jinqigfzy.top

Java: String greet() { return name; }
来源：http://avp.chenzaomai.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://xrv.tanke756.top

Ruby: def greet; @name; end
来源：http://lfv.dashuyun.cn

C#:   public string Greet() => Name;
来源：http://wah.shzxlz.cn

[G05] 继承
来源：http://chj.ywan-chungtsiang.top

Py:   class Admin(User): pass
来源：http://nqo.bbcook.cn

PHP:  class Admin extends User {}
来源：http://lql.fehbvm.com

JS:   class Admin extends User {}
来源：http://pwo.ywan-chungtsiang.top

TS:   class Admin extends User {}
来源：http://gbh.ehwqpu.com

Java: class Admin extends User {}
来源：http://xts.jinqigfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cck.wangdashe.top

Ruby: class Admin < User; end
来源：http://efr.cdnleiting.top

C#:   class Admin : User {}
来源：http://thc.sjlbkw.cn

[G06] 重写方法
来源：http://axz.vqdsnc.cn

Py:   def greet(self): return "admin"
来源：http://qhs.guowangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pix.9152youxi.cn

JS:   greet() { return "admin"; }
来源：http://oga.chenlongwang.top

TS:   greet(): string { return "admin"; }
来源：http://rif.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://evs.gaohongyu789.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mxp.bbcook.cn

Ruby: def greet; "admin"; end
来源：http://btv.shanyushiyangtech.top


<!-- 参考信息 -->
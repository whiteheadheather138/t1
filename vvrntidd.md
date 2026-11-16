代发 wailian999

C#:   s.Replace("a", "b")
来源：http://cib.snrcjt.cn

[E07] 按分隔符拆分
来源：http://yzr.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ylr.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qta.yuanzhike.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gyh.gzhubu.top

TS:   s.split(",")
来源：http://hja.sjlbkw.cn

Java: s.split(",");  s.split("\\s+")
来源：http://urf.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://far.ydjk.org.cn

Ruby: s.split(",");  s.split
来源：http://mws.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lsr.yfazqb.com

[E08] 数组按分隔符合并
来源：http://pnk.0kj1m.cn

Py:   ",".join(items)
来源：http://ykt.andypj.xyz

PHP:  implode(",", $items);
来源：http://fzm.birdmap.top

JS:   items.join(",")
来源：http://aof.mhx1999.top

TS:   items.join(",")
来源：http://ljg.ydjk.org.cn

Java: String.join(",", items)
来源：http://wla.tian-w.cn

Go:   strings.Join(items, ",")
来源：http://rhc.yonumen.top

Ruby: items.join(",")
来源：http://iwb.sxryk.cn

C#:   string.Join(",", items)
来源：http://vka.daria6918.cn

[E09] 去除所有空白字符
来源：http://imd.tianlin.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bkl.hywenlv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hrn.yj20258888.top

JS:   s.replace(/\s+/g, "")
来源：http://blw.tarul.cn

TS:   s.replace(/\s+/g, "")
来源：http://ove.sufxvd.cn

Java: s.replaceAll("\\s+", "")
来源：http://nwr.gaohongyu789.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ryo.kuanghao11.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gds.kuanghao11.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bac.tanke756.top

[E10] 左侧补零 / 定长填充
来源：http://jfq.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jyb.yuanzhike.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://drl.xingfuxueyuan.xyz

JS:   "7".padStart(3, "0")
来源：http://ncn.yfazqb.com

TS:   "7".padStart(3, "0")
来源：http://udz.bbcook.cn

Java: String.format("%03d", 7)
来源：http://eii.ppjwa.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://htb.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iun.bbcook.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dgc.hnqzz.top

[E11] 反转字符串
来源：http://myi.hysaishi.cn

Py:   s[::-1]
来源：http://ozj.ydjk.org.cn

PHP:  strrev($s);
来源：http://uei.pengpengdd.cyou

JS:   [...s].reverse().join("")
来源：http://uim.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://fft.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://viq.xuetiantiany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bsw.fehbvm.com

Ruby: s.reverse
来源：http://ifw.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://uqi.sxryk.cn

[E12] 统计某字符出现次数
来源：http://yrn.ctjpmb.com

Py:   s.count("a")
来源：http://eko.hysaishi.cn

PHP:  substr_count($s, "a");
来源：http://zit.hnqzz.top

JS:   s.split("a").length - 1
来源：http://wwm.hywenlv.cn

TS:   s.split("a").length - 1
来源：http://olq.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://thd.shzxlz.cn

Go:   strings.Count(s, "a")
来源：http://xio.hesvh.cn

Ruby: s.count("a")
来源：http://gnr.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://nua.quarkkingdee.top

[E13] 逐字符遍历
来源：http://ohz.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://pbd.hywenlv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lcm.yueranfly.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mif.yj20258.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://eyk.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kvi.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zsj.feifeiyinyue.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jqf.vehdjk.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gkr.fzhhl.top

[E14] URL 编码与 Base64
来源：http://nqg.cashguo.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vin.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ulj.hnqzz.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wrv.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nco.havefunace.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bvl.zdqjudy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qep.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://czz.vqdsnc.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://igk.fanxiaobao.xyz

[E15] HTML 转义 / 反转义
来源：http://tyi.yongpay.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hts.gogol.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rgf.ehwqpu.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://svp.316326.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://sfl.nwbrower.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blf.vqdsnc.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hjc.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jrj.zhengqikj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gwz.ydjk.org.cn

[E16] 数字千分位
来源：http://jla.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://fgn.haohaochexian.top

PHP:  number_format(1234567);
来源：http://fos.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bqy.zhiwuduotai.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cza.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vqw.zhixingplan.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lbf.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sar.yfazqb.com

C#:   1234567.ToString("N0")
来源：http://lhh.hysaishi.cn

[E17] 首字母大写
来源：http://ywz.zhiwuduotai.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://avl.yj20258.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ujh.ehwqpu.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ztc.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zbx.zdbjq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://akf.sweek.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jlu.ehwqpu.com

Ruby: s.capitalize
来源：http://ane.kuanghao11.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bra.andypj.xyz

[E18] 模板占位符替换
来源：http://zjt.hammf.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vow.shanyushiyangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qry.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vyh.0kj1m.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vuf.jlsjyb.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gcv.ywan-chungtsiang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vnf.aizwys.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wrv.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tmu.zhiwuduotai.top

[E19] 多行文本按行拆分
来源：http://rsm.xingfuxueyuan.xyz

Py:   s.splitlines()
来源：http://ffr.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qee.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://hjh.cheryme.top

TS:   s.split(/\r?\n/)
来源：http://hjn.tarul.cn

Java: s.lines().toList()
来源：http://nas.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://xud.0kj1m.cn

Ruby: s.lines
来源：http://biw.hcnkem.com

C#:   s.Split('\n')
来源：http://umm.tianlin.xyz

[E20] 判断字符串是否为空
来源：http://cen.cheryme.top

Py:   if not s:
来源：http://has.tianlin.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fkn.xingfuxueyuan.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pdj.shangyingyoupin.top

TS:   if (s === "") {}
来源：http://obt.tanke756.top

Java: if (s.isEmpty()) {}
来源：http://nct.yvedp.cn

Go:   if s == "" {}
来源：http://jvi.ydzc1.top

Ruby: if s.empty?
来源：http://ydr.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://egz.hammf.cn

[E21] 超长截断加省略号
来源：http://dcu.hysaishi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://naf.ppjwa.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://thy.guannengcc.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cse.jinqigufen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nvl.hysaishi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://opm.tian-w.cn

Go:   // 按 rune 判断长度后截断
来源：http://jtm.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://isb.jiagoushi.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://drk.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://roj.zhaomingkeji.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dky.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jzn.pycfn.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fdf.hnqzz.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fpn.xuetiantiany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ruw.meibo888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gyc.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://ydr.chenjidiqi.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zxf.shangyingyoupin.top

================================================================================
来源：http://otq.jlsjyb.cn

F. 文件与目录
来源：http://erb.sweek.top

================================================================================
来源：http://csy.52xcode.cn

[F01] 读取整个文件
来源：http://mks.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ifu.tian-w.cn

PHP:  file_get_contents("a.txt");
来源：http://awo.fzhhl.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jfg.tanke756.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wts.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nuo.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fse.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://bua.gogol.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://oej.daria6918.cn

[F02] 逐行读取文件
来源：http://uml.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tez.ehwqpu.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zbq.zhoulong.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://enz.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dvh.hysaishi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xgc.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xbt.xziqi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qnp.vqdsnc.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qwu.daxiang520.top

[F03] 写入文件（覆盖）
来源：http://enw.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yho.0kj1m.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ewj.svipenyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dcm.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gnq.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zbk.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://syg.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://vej.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fqq.nanxinkj.top

[F04] 追加写入文件
来源：http://fdh.cqqwz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qvw.havefunace.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lye.andypj.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nku.chenzaomai.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lxj.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://svr.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bst.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rig.shzxlz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://afe.ywan-chungtsiang.top

[F05] 判断文件或目录是否存在
来源：http://yom.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rfk.kuanghao11.cn

PHP:  file_exists("a.txt");
来源：http://orh.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://eer.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://oim.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qkw.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hpw.fktsv.cn

Ruby: File.exist?("a.txt")
来源：http://qth.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://klv.tian-w.cn

[F06] 删除文件
来源：http://zwk.yongpay.top

Py:   os.remove("a.txt")
来源：http://lqg.ydjk.org.cn

PHP:  unlink("a.txt");
来源：http://wle.ybcxt.top

JS:   fs.unlinkSync("a.txt")
来源：http://vle.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://vdx.daria6918.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jqg.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://sko.gogol.net.cn

Ruby: File.delete("a.txt")
来源：http://pjr.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://cfr.ydjk.org.cn

[F07] 创建目录（含多级）
来源：http://zrt.sjlbkw.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gtx.meibo888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ntb.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xph.pengpengdd.cyou

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://maa.dianchejie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wim.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://smr.ivvv.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kon.ctjpmb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://buo.sweek.top

[F08] 遍历目录
来源：http://bdd.feifeiyinyue.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pzc.meibo888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ewf.zhengqikj.top

JS:   fs.readdirSync("dir")
来源：http://kok.c1oappe.top

TS:   fs.readdirSync("dir")
来源：http://kpk.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kjk.pycfn.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://jhl.zdbjq.cn

Ruby: Dir.children("dir")
来源：http://exd.sxryk.cn

C#:   Directory.GetFiles("dir")
来源：http://rvf.aibaodan.cn

[F09] 获取文件大小
来源：http://ckw.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://dyw.sweek.top

PHP:  filesize("a.txt");
来源：http://mcm.kuanghao11.cn

JS:   fs.statSync("a.txt").size
来源：http://czo.jyoumei.cn

TS:   fs.statSync("a.txt").size
来源：http://jwn.hfpthk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yrd.cashguo.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gzz.52xcode.cn

Ruby: File.size("a.txt")
来源：http://txz.andypj.xyz

C#:   new FileInfo("a.txt").Length
来源：http://xfj.guowangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://tvq.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wnl.jlsjyb.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://snt.zhiwuduotai.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rrn.zhiwuduotai.top

TS:   path.extname("a.txt")
来源：http://clf.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://efi.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ytg.yanxiufei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hrz.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tgv.yueranfly.top

[F11] 复制与移动文件
来源：http://yfd.yj202588.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dlc.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fcl.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dae.feifeiyinyue.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bvk.yj20258.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ncj.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uzn.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eoi.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jyx.quarkkingdee.top

[F12] CSV 读写
来源：http://kvv.cqqwz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zld.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mgt.ybcxt.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mdr.birdmap.top

TS:   // 同上
来源：http://cmr.52xcode.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dqo.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sqp.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qwt.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://owm.daria6918.cn

================================================================================
来源：http://ytk.zhiwuduotai.top

G. 面向对象
来源：http://sbz.ivvv.top

================================================================================
来源：http://ppw.bjfxy.top

[G01] 定义类
来源：http://vxl.yangfankeji.com

Py:   class User: pass
来源：http://ubu.bbcook.cn

PHP:  class User {}
来源：http://cbt.aibaodan.cn

JS:   class User {}
来源：http://mwd.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://skx.nanxinkj.top

Java: class User {}
来源：http://apz.kuanghao11.cn

Go:   type User struct { Name string }
来源：http://uzk.nwbrower.top

Ruby: class User; end
来源：http://uxz.jinyuanbaomall.cn

C#:   class User {}
来源：http://blw.hfpthk.cn

[G02] 构造函数
来源：http://aot.jinyuanbaomall.cn

Py:   def __init__(self, name): self.name = name
来源：http://xoj.zhijiandao.cn

PHP:  public function __construct(public string $name) {}
来源：http://snn.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://qhs.dianchejie.cn

TS:   constructor(public name: string) {}
来源：http://ksx.gogol.net.cn

Java: User(String name) { this.name = name; }
来源：http://iji.daxiang520.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dsi.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://aam.fengsongda.top

C#:   public User(string name) { Name = name; }
来源：http://ziw.sysykeji.top

[G03] 实例属性
来源：http://pss.smart0.xyz

Py:   self.name = "x"
来源：http://xvu.tian-w.cn

PHP:  public string $name = "x";
来源：http://kyd.mhx1999.top

JS:   this.name = "x";
来源：http://idp.fehbvm.com

TS:   name: string = "x";
来源：http://kcl.xylfe.cn

Java: private String name;
来源：http://aah.aibaodan.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ibe.wangshuangyany.cn

Ruby: @name = "x"
来源：http://mkr.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://lik.cqqwz.cn

[G04] 定义方法
来源：http://dug.redwolf501.top

Py:   def greet(self): return self.name
来源：http://axy.smart0.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://wqb.xuetiantiany.cn

JS:   greet() { return this.name; }
来源：http://vxz.jinghuilouyu.cn

TS:   greet(): string { return this.name; }
来源：http://qxh.bbcook.cn

Java: String greet() { return name; }
来源：http://kuu.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lgs.9152youxi.cn

Ruby: def greet; @name; end
来源：http://djj.shanyushiyangkeji.top

C#:   public string Greet() => Name;
来源：http://lom.sysykeji.top

[G05] 继承
来源：http://dsd.birdmap.top

Py:   class Admin(User): pass
来源：http://tzc.cheryme.top

PHP:  class Admin extends User {}
来源：http://sms.gotoacloud.top

JS:   class Admin extends User {}
来源：http://jcc.zhaomingkeji.xyz

TS:   class Admin extends User {}
来源：http://sub.cheryme.top


<!-- 参考信息 -->
代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://ckk.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lfv.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rwj.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mei.daxiang520.top

C#:   s.Replace("a", "b")
来源：http://eub.pycfn.com

[E07] 按分隔符拆分
来源：http://cah.hfpthk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ffp.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rxv.ydjk.org.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bmj.ppjwa.cn

TS:   s.split(",")
来源：http://art.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://ldr.kuanghao11.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wrr.hfpthk.cn

Ruby: s.split(",");  s.split
来源：http://eej.ydjk.org.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zby.dashuyun.cn

[E08] 数组按分隔符合并
来源：http://ruh.smart0.xyz

Py:   ",".join(items)
来源：http://ftv.yuxming.cn

PHP:  implode(",", $items);
来源：http://deg.iojbl.cn

JS:   items.join(",")
来源：http://fjc.ppjwa.cn

TS:   items.join(",")
来源：http://udu.hysaishi.cn

Java: String.join(",", items)
来源：http://gkl.cashguo.top

Go:   strings.Join(items, ",")
来源：http://kjg.haohaochexian.top

Ruby: items.join(",")
来源：http://zht.mhx1999.top

C#:   string.Join(",", items)
来源：http://dzi.jianghu66.top

[E09] 去除所有空白字符
来源：http://dqi.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fwe.dianchejie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tbh.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://lmg.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://uvz.daxiang520.top

Java: s.replaceAll("\\s+", "")
来源：http://irc.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mpm.chenzaomai.com

Ruby: s.gsub(/\s+/, "")
来源：http://tpx.svipenyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ire.iojbl.cn

[E10] 左侧补零 / 定长填充
来源：http://nji.fehbvm.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zdw.shzxlz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tgj.cucudq.cn

JS:   "7".padStart(3, "0")
来源：http://lax.nanxinkj.top

TS:   "7".padStart(3, "0")
来源：http://jgf.yj20258.top

Java: String.format("%03d", 7)
来源：http://fod.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://ofp.feifeiyinyue.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qsw.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tln.ivvv.top

[E11] 反转字符串
来源：http://vuo.shanyushiyangkeji.top

Py:   s[::-1]
来源：http://odk.cashguo.top

PHP:  strrev($s);
来源：http://foe.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://znm.aibaodan.cn

TS:   [...s].reverse().join("")
来源：http://qsk.zhongyouzk.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kdr.shanyushiyangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dsb.9152youxi.cn

Ruby: s.reverse
来源：http://tkd.kuanghao11.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fck.sweek.top

[E12] 统计某字符出现次数
来源：http://wav.tarul.cn

Py:   s.count("a")
来源：http://jkf.feifeiyinyue.top

PHP:  substr_count($s, "a");
来源：http://kms.yueranfly.top

JS:   s.split("a").length - 1
来源：http://qci.cqqwz.cn

TS:   s.split("a").length - 1
来源：http://ijt.hesvh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nbp.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://oxh.yanxiufei.cn

Ruby: s.count("a")
来源：http://duf.chenlongwang.top

C#:   s.Count(c => c == 'a')
来源：http://fve.andypj.xyz

[E13] 逐字符遍历
来源：http://sfo.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://jkc.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yco.jlsjyb.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mgt.zhixingplan.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wox.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vwi.yonumen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rcz.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ddo.shanyushiyangtech.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iys.9152youxi.cn

[E14] URL 编码与 Base64
来源：http://inm.xuanzx.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://scm.jinqigfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rng.yueranfly.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dsc.316326.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ogv.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vzj.ydzc1.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cod.yj20258888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vyc.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lsj.ehwqpu.com

[E15] HTML 转义 / 反转义
来源：http://wnk.yj202588.top

Py:   html.escape(s);  html.unescape(s)
来源：http://anb.tanke756.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://abu.aizwys.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://umq.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lyo.zhoulong.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://klh.jinqigfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nxl.aibaodan.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yqx.zdqjudy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xku.guowangkeji.top

[E16] 数字千分位
来源：http://cxf.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://eal.ydjk.org.cn

PHP:  number_format(1234567);
来源：http://vou.pycfn.com

JS:   (1234567).toLocaleString("en-US")
来源：http://fdf.xuetiantiany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xmj.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mxf.chenlongwang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ccl.hywenlv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xec.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://sct.redwolf501.top

[E17] 首字母大写
来源：http://hvo.jqgufenzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://buz.hywenlv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://emf.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xww.haohaochexian.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iqh.jianghu66.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ype.hcnkem.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pbf.redwolf501.top

Ruby: s.capitalize
来源：http://rjh.yongpay.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://erd.yvedp.cn

[E18] 模板占位符替换
来源：http://oue.0kj1m.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vin.jiagoushi.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qvb.hfpthk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fod.aibaodan.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gok.pycfn.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://axw.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://suc.sxryk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rro.xingfuxueyuan.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fan.pengpengdd.cyou

[E19] 多行文本按行拆分
来源：http://kdm.hfpthk.cn

Py:   s.splitlines()
来源：http://ujm.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rby.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://ygr.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://ngl.guannengcc.top

Java: s.lines().toList()
来源：http://uzq.daxiang520.top

Go:   strings.Split(s, "\n")
来源：http://nnw.jiagoushi.top

Ruby: s.lines
来源：http://yjt.jlsjyb.cn

C#:   s.Split('\n')
来源：http://gbw.yueranfly.top

[E20] 判断字符串是否为空
来源：http://lix.jlsjyb.cn

Py:   if not s:
来源：http://vbo.ctjpmb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rwi.gogol.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gub.zhixingplan.top

TS:   if (s === "") {}
来源：http://vsh.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://hjv.zhengqikj.top

Go:   if s == "" {}
来源：http://tbx.zhijiandao.cn

Ruby: if s.empty?
来源：http://fkp.havefunace.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ihi.guannengcc.top

[E21] 超长截断加省略号
来源：http://czu.0kj1m.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://azo.yuanzhike.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ppq.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gfu.yvedp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://agr.dianchejie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rzc.fanxiaobao.xyz

Go:   // 按 rune 判断长度后截断
来源：http://dgt.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://afk.fengsongda.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ebd.bbcook.cn

[E22] 字节长度与字符长度
来源：http://enn.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hcj.jyoumei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sux.wangshuangyany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gjd.pengpengdd.cyou

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aon.sufxvd.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://llq.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vcw.316326.xyz

Ruby: s.bytesize;  s.length
来源：http://eqh.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://psi.zhongyouzk.top

================================================================================
来源：http://qzp.cashguo.top

F. 文件与目录
来源：http://fiv.hnxiangtu.top

================================================================================
来源：http://ryw.cdnleiting.top

[F01] 读取整个文件
来源：http://mbb.dianchejie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cys.iojbl.cn

PHP:  file_get_contents("a.txt");
来源：http://loh.hammf.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jwv.yj202588.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zzw.zycfv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wtf.yangfankeji.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ipm.smart0.xyz

Ruby: File.read("a.txt")
来源：http://ujg.epnwcf.com

C#:   File.ReadAllText("a.txt");
来源：http://eba.zhiwuduotai.top

[F02] 逐行读取文件
来源：http://csk.hongshengwenyu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rjm.kuanghao11.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cit.xingfuxueyuan.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dej.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zdo.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qrd.aizwys.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dtt.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uvq.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ffc.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://vcu.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ngv.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://omd.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rqc.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mmq.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xns.svipenyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://onb.pengpengdd.cyou

Ruby: File.write("a.txt", "hi")
来源：http://kvq.9152youxi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bey.tarul.cn

[F04] 追加写入文件
来源：http://tjt.dianchejie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zrn.shuidangran.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sto.chenjidiqi.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nrt.gzhubu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://twg.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lps.ybcxt.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dos.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fcp.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uvc.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://nmj.shanyushiyangtech.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://plj.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://sfp.nwbrower.top

JS:   fs.existsSync("a.txt")
来源：http://nct.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://jge.hesvh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gmo.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lnz.yj20258.top

Ruby: File.exist?("a.txt")
来源：http://agm.daria6918.cn

C#:   File.Exists("a.txt")
来源：http://odg.havefunace.top

[F06] 删除文件
来源：http://zmr.gaohongyu789.top

Py:   os.remove("a.txt")
来源：http://iuq.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://hby.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://xkv.birdmap.top

TS:   fs.unlinkSync("a.txt")
来源：http://jll.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cns.nanxuanxn.top

Go:   os.Remove("a.txt")
来源：http://zpp.havefunace.top

Ruby: File.delete("a.txt")
来源：http://vmj.vehdjk.com

C#:   File.Delete("a.txt");
来源：http://nxg.vqdsnc.cn

[F07] 创建目录（含多级）
来源：http://gct.jinghuilouyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://swn.jinghuilouyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vib.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ccm.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mof.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mdf.jinghuilouyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aeb.bbcook.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lnq.hcnkem.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cqd.52xcode.cn

[F08] 遍历目录
来源：http://ars.haohaochexian.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bzt.tarul.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://snx.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://lyp.andypj.xyz

TS:   fs.readdirSync("dir")
来源：http://qgz.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hnz.xylfe.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ghh.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://evc.shanyushiyangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://ayv.nwbrower.top

[F09] 获取文件大小
来源：http://ozr.shanyushiyangtech.top

Py:   os.path.getsize("a.txt")
来源：http://zsr.wangshuangyany.cn

PHP:  filesize("a.txt");
来源：http://ikz.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://kta.wangdashe.top

TS:   fs.statSync("a.txt").size
来源：http://lmp.yanxiufei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fhs.cheryme.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wuf.sweek.top

Ruby: File.size("a.txt")
来源：http://ymb.gotoacloud.top

C#:   new FileInfo("a.txt").Length
来源：http://zbg.jqgfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://wiy.jiagoushi.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zwv.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gmr.tian-w.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://szs.yongpay.top

TS:   path.extname("a.txt")
来源：http://bnj.shanyushiyangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oqq.jinqigufen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nrs.shanyushiyangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dcd.hcnkem.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lao.redwolf501.top

[F11] 复制与移动文件
来源：http://qfi.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qbk.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hav.zhoulong.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zor.zhengqikj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bmh.shuidangran.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jhj.svipenyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gab.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ckk.shanyushiyangtech.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eda.xingfuxueyuan.xyz

[F12] CSV 读写
来源：http://cty.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qew.ybcxt.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dsc.0kj1m.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rci.ydzc1.top

TS:   // 同上
来源：http://nye.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nrv.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bzk.aibaodan.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dxk.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ryo.shangyingyoupin.top

================================================================================
来源：http://wrc.chenzaomai.com

G. 面向对象
来源：http://lrf.zhengqikj.top

================================================================================
来源：http://btu.jianghu66.top

[G01] 定义类
来源：http://sgz.ywan-chungtsiang.top

Py:   class User: pass
来源：http://yxs.zhiwuduotai.top

PHP:  class User {}
来源：http://ktb.jinqigufen.top

JS:   class User {}
来源：http://had.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://sbx.chenzaomai.com

Java: class User {}
来源：http://cdq.cqqwz.cn

Go:   type User struct { Name string }
来源：http://ffm.jqgfzy.top

Ruby: class User; end
来源：http://acd.havefunace.top

C#:   class User {}
来源：http://rsn.cdnleiting.top

[G02] 构造函数
来源：http://cnz.guowangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://udv.ehwqpu.com

PHP:  public function __construct(public string $name) {}
来源：http://vbg.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://uhz.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://qhb.zhoulong.xyz

Java: User(String name) { this.name = name; }
来源：http://cts.fanxiaobao.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iqj.jinghuilouyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://dcu.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://tlr.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://hwm.ehwqpu.com

Py:   self.name = "x"
来源：http://qfo.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://eir.jqgufenzy.top

JS:   this.name = "x";
来源：http://neo.jiagoushi.top

TS:   name: string = "x";
来源：http://xzm.meibo888.top

Java: private String name;
来源：http://ued.sxryk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sro.zhoulong.xyz

Ruby: @name = "x"
来源：http://ptg.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://mmg.ivvv.top

[G04] 定义方法
来源：http://rwb.fktsv.cn

Py:   def greet(self): return self.name
来源：http://vmp.nwbrower.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vci.fktsv.cn

JS:   greet() { return this.name; }
来源：http://dei.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://pkd.aibaodan.cn

Java: String greet() { return name; }
来源：http://ncs.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xne.gzhubu.top

Ruby: def greet; @name; end
来源：http://oai.vehdjk.com

C#:   public string Greet() => Name;
来源：http://vdz.dianchejie.cn

[G05] 继承
来源：http://thw.ivvv.top


<!-- 参考信息 -->
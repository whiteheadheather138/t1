代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://sjd.shanyushiyangtech.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ngu.aizwys.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rwv.shzxlz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://owi.yj20258888.top

C#:   s.Replace("a", "b")
来源：http://vqp.yanxiufei.cn

[E07] 按分隔符拆分
来源：http://qux.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pdd.chenjidiqi.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qyw.zhixingplan.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hxn.xingfuxueyuan.xyz

TS:   s.split(",")
来源：http://wwd.chenjidiqi.icu

Java: s.split(",");  s.split("\\s+")
来源：http://mcr.vqdsnc.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://aru.tarul.cn

Ruby: s.split(",");  s.split
来源：http://yob.gzhubu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fco.cucudq.cn

[E08] 数组按分隔符合并
来源：http://cst.jqgufenzy.top

Py:   ",".join(items)
来源：http://qql.nanxinkj.top

PHP:  implode(",", $items);
来源：http://bpu.yj202588.top

JS:   items.join(",")
来源：http://szr.pengpengdd.cyou

TS:   items.join(",")
来源：http://xjg.jqgfzy.top

Java: String.join(",", items)
来源：http://jaw.zdqjudy.top

Go:   strings.Join(items, ",")
来源：http://oqn.chenzaomai.com

Ruby: items.join(",")
来源：http://foj.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://jkh.zhijiandao.cn

[E09] 去除所有空白字符
来源：http://dii.xuanzx.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qpe.yvedp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hjh.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://qeq.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://vut.zhaomingkeji.xyz

Java: s.replaceAll("\\s+", "")
来源：http://aft.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://okf.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://xzj.havefunace.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rnt.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://hyz.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qsf.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://odj.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://wpc.redwolf501.top

TS:   "7".padStart(3, "0")
来源：http://ptf.fzhhl.top

Java: String.format("%03d", 7)
来源：http://kag.jqgufenzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tdr.sufxvd.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yfn.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oia.cucudq.cn

[E11] 反转字符串
来源：http://lgz.cucudq.cn

Py:   s[::-1]
来源：http://yvt.smart0.xyz

PHP:  strrev($s);
来源：http://jtv.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://xjh.jinghuilouyu.cn

TS:   [...s].reverse().join("")
来源：http://keg.cdnleiting.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kod.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pip.jyoumei.cn

Ruby: s.reverse
来源：http://rwm.yanxiufei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mao.yj20258.top

[E12] 统计某字符出现次数
来源：http://zou.zhijiandao.cn

Py:   s.count("a")
来源：http://meh.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://gsx.cashguo.top

JS:   s.split("a").length - 1
来源：http://twa.sjlbkw.cn

TS:   s.split("a").length - 1
来源：http://ozy.sufxvd.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aku.fehbvm.com

Go:   strings.Count(s, "a")
来源：http://svg.mhx1999.top

Ruby: s.count("a")
来源：http://vfk.ywan-chungtsiang.top

C#:   s.Count(c => c == 'a')
来源：http://qtv.chenlongwang.top

[E13] 逐字符遍历
来源：http://fgn.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://cey.zhongyouzk.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gfb.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tiq.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tkz.sjlbkw.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://grm.guowangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dtn.sxryk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://llq.cucudq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aka.c1oappe.top

[E14] URL 编码与 Base64
来源：http://crm.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lpo.yvedp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jan.0kj1m.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://edu.sufxvd.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zxm.jiagoushi.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kvn.yanxiufei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hac.shanyushiyangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rjw.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fiv.bjfxy.top

[E15] HTML 转义 / 反转义
来源：http://lfa.yj20258.top

Py:   html.escape(s);  html.unescape(s)
来源：http://brf.xuanzx.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nit.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ixv.cucudq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://adz.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mur.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mrt.snrcjt.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vhg.316326.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lhz.hesvh.cn

[E16] 数字千分位
来源：http://crp.aizwys.cn

Py:   f"{1234567:,}"
来源：http://csq.sysykeji.top

PHP:  number_format(1234567);
来源：http://ulr.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gps.ywan-chungtsiang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://isk.chenzaomai.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mdj.aibaodan.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cem.jinqigfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xoq.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://kgz.vqdsnc.cn

[E17] 首字母大写
来源：http://nxj.xuanzx.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zfw.guowangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fvw.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pqt.gzhubu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gsz.guowangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zoo.cashguo.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pmi.meibo888.top

Ruby: s.capitalize
来源：http://rfi.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sjo.jqgfzy.top

[E18] 模板占位符替换
来源：http://ngv.bbcook.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cpv.yueranfly.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jxf.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xsj.wangshuangyany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nhp.zhijiandao.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kci.zdqjudy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://agc.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vcm.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uhs.ywan-chungtsiang.top

[E19] 多行文本按行拆分
来源：http://hda.daria6918.cn

Py:   s.splitlines()
来源：http://qqr.yanxiufei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dhi.guannengcc.top

JS:   s.split(/\r?\n/)
来源：http://ntq.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://fjx.ctjpmb.com

Java: s.lines().toList()
来源：http://pqm.ybcxt.top

Go:   strings.Split(s, "\n")
来源：http://uff.svipenyu.cn

Ruby: s.lines
来源：http://scp.jqgufenzy.top

C#:   s.Split('\n')
来源：http://ynf.zhixingplan.top

[E20] 判断字符串是否为空
来源：http://hcp.hywenlv.cn

Py:   if not s:
来源：http://ukv.sysykeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ugo.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pqk.zhijiandao.cn

TS:   if (s === "") {}
来源：http://yrp.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://nse.zhijiandao.cn

Go:   if s == "" {}
来源：http://avu.ivvv.top

Ruby: if s.empty?
来源：http://imm.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hyc.wangshuangyany.cn

[E21] 超长截断加省略号
来源：http://mjq.guannengcc.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://raj.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rgz.c1oappe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ttk.zhoulong.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bqv.guowangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cvb.yonumen.top

Go:   // 按 rune 判断长度后截断
来源：http://jnb.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fvx.zycfv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oxg.jyoumei.cn

[E22] 字节长度与字符长度
来源：http://dgb.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gcu.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vlz.vqdsnc.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fpu.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qod.haohaochexian.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hda.iojbl.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zlj.yj20258.top

Ruby: s.bytesize;  s.length
来源：http://uwp.sjlbkw.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://poi.tanke756.top

================================================================================
来源：http://npl.9152youxi.cn

F. 文件与目录
来源：http://zfd.gotoacloud.top

================================================================================
来源：http://ord.chenzaomai.com

[F01] 读取整个文件
来源：http://nns.tanke756.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ryp.fktsv.cn

PHP:  file_get_contents("a.txt");
来源：http://ncx.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lwy.xziqi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pne.zhixingplan.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gkg.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cro.nwbrower.top

Ruby: File.read("a.txt")
来源：http://xiv.yj20258888.top

C#:   File.ReadAllText("a.txt");
来源：http://yaa.yanxiufei.cn

[F02] 逐行读取文件
来源：http://try.yanxiufei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nva.xingfuxueyuan.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ayz.shanyushiyangtech.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://unz.hnxiangtu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dfz.svipenyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wad.meibo888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ukp.xingfuxueyuan.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xze.pycfn.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fip.hammf.cn

[F03] 写入文件（覆盖）
来源：http://tro.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aue.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ojx.sysykeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hit.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uhq.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wqn.yanxiufei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dlm.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://bnv.fengsongda.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ege.xziqi.cn

[F04] 追加写入文件
来源：http://pto.pengpengdd.cyou

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vmb.nanxuanxn.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vio.yj20258888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yzn.vqdsnc.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fcm.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cvh.c1oappe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ncg.shanyushiyangtech.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kde.sysykeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://egk.jinqigufen.top

[F05] 判断文件或目录是否存在
来源：http://ywe.mhx1999.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rkl.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://fzf.hcnkem.com

JS:   fs.existsSync("a.txt")
来源：http://zyr.zhixingplan.top

TS:   fs.existsSync("a.txt")
来源：http://ftp.havefunace.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qkx.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mkw.zhixingplan.top

Ruby: File.exist?("a.txt")
来源：http://wcr.chenjidiqi.icu

C#:   File.Exists("a.txt")
来源：http://gmz.hfpthk.cn

[F06] 删除文件
来源：http://xjg.yvedp.cn

Py:   os.remove("a.txt")
来源：http://iqa.dashuyun.cn

PHP:  unlink("a.txt");
来源：http://gvf.gaohongyu789.top

JS:   fs.unlinkSync("a.txt")
来源：http://sdt.hnxiangtu.top

TS:   fs.unlinkSync("a.txt")
来源：http://lhp.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://van.xinyue.icu

Go:   os.Remove("a.txt")
来源：http://rux.hesvh.cn

Ruby: File.delete("a.txt")
来源：http://dmp.hfpthk.cn

C#:   File.Delete("a.txt");
来源：http://wln.ctjpmb.com

[F07] 创建目录（含多级）
来源：http://amf.quarkkingdee.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://orf.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ikr.cheryme.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://omd.daria6918.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://flq.yanxiufei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://axv.yanxiufei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hzt.sysykeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eqh.yfazqb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ogg.zhengqikj.top

[F08] 遍历目录
来源：http://llv.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://aiu.316326.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ssp.wangshuangyany.cn

JS:   fs.readdirSync("dir")
来源：http://yfv.andypj.xyz

TS:   fs.readdirSync("dir")
来源：http://iee.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xdu.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zsh.yvedp.cn

Ruby: Dir.children("dir")
来源：http://zrt.jyoumei.cn

C#:   Directory.GetFiles("dir")
来源：http://tgo.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://yoj.zycfv.cn

Py:   os.path.getsize("a.txt")
来源：http://nyx.birdmap.top

PHP:  filesize("a.txt");
来源：http://wjz.tian-w.cn

JS:   fs.statSync("a.txt").size
来源：http://cyh.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://qal.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://fan.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qme.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://gxd.bjfxy.top

C#:   new FileInfo("a.txt").Length
来源：http://stu.c1oappe.top

[F10] 取文件扩展名 / 文件名
来源：http://yzs.ppjwa.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ejr.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yxq.wangdashe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eco.zhijiandao.cn

TS:   path.extname("a.txt")
来源：http://yoe.ydzc1.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dis.snrcjt.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vks.fzhhl.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cnm.tian-w.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ukx.0kj1m.cn

[F11] 复制与移动文件
来源：http://dvh.havefunace.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mue.ydjk.org.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lju.c1oappe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tcs.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://euc.cucudq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qze.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vzp.tianlin.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xbu.xuetiantiany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hmg.hysaishi.cn

[F12] CSV 读写
来源：http://zwo.xylfe.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qgg.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zpb.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nux.chenlongwang.top

TS:   // 同上
来源：http://wny.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vti.tanke756.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mis.ydzc1.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tbh.zhoulong.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://wcp.nanxinkj.top

================================================================================
来源：http://ksv.sjlbkw.cn

G. 面向对象
来源：http://smf.0kj1m.cn

================================================================================
来源：http://cmx.xinyue.icu

[G01] 定义类
来源：http://bwg.nwbrower.top

Py:   class User: pass
来源：http://vwm.yanxiufei.cn

PHP:  class User {}
来源：http://lgx.hnqzz.top

JS:   class User {}
来源：http://fpj.hysaishi.cn

TS:   class User { name: string = ""; }
来源：http://qnd.ydjk.org.cn

Java: class User {}
来源：http://asw.sysykeji.top

Go:   type User struct { Name string }
来源：http://pdg.sweek.top

Ruby: class User; end
来源：http://oyo.guowangkeji.top

C#:   class User {}
来源：http://wgt.birdmap.top

[G02] 构造函数
来源：http://hps.tian-w.cn

Py:   def __init__(self, name): self.name = name
来源：http://jik.316326.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ypw.ehwqpu.com

JS:   constructor(name) { this.name = name; }
来源：http://dyq.yj20258888.top

TS:   constructor(public name: string) {}
来源：http://eme.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://ydf.quarkkingdee.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rsv.quarkkingdee.top

Ruby: def initialize(name); @name = name; end
来源：http://tuo.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://rzw.snrcjt.cn

[G03] 实例属性
来源：http://kgn.9152youxi.cn

Py:   self.name = "x"
来源：http://ulr.zdqjudy.top

PHP:  public string $name = "x";
来源：http://vaz.jyoumei.cn

JS:   this.name = "x";
来源：http://yhb.52xcode.cn

TS:   name: string = "x";
来源：http://rrb.jqgufenzy.top

Java: private String name;
来源：http://gao.zhijiandao.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ndr.hnxiangtu.top

Ruby: @name = "x"
来源：http://ikm.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://hle.feifeiyinyue.top

[G04] 定义方法
来源：http://ouk.ivvv.top

Py:   def greet(self): return self.name
来源：http://qou.zdbjq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gkz.shuidangran.top

JS:   greet() { return this.name; }
来源：http://xey.ppjwa.cn

TS:   greet(): string { return this.name; }
来源：http://ixs.jinqigfzy.top

Java: String greet() { return name; }
来源：http://etl.gaohongyu789.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dsv.cashguo.top

Ruby: def greet; @name; end
来源：http://yhs.316326.xyz

C#:   public string Greet() => Name;
来源：http://urc.shuidangran.top

[G05] 继承
来源：http://sff.xuanzx.com


<!-- 参考信息 -->
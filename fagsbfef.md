代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://uza.hfpthk.cn

TS:   s.split(",")
来源：http://cbo.gogol.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://edl.yfazqb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ypq.hywenlv.cn

Ruby: s.split(",");  s.split
来源：http://tps.haohaochexian.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fbx.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://xdu.shangyingyoupin.top

Py:   ",".join(items)
来源：http://ygg.tian-w.cn

PHP:  implode(",", $items);
来源：http://xnw.nanxinkj.top

JS:   items.join(",")
来源：http://dom.tarul.cn

TS:   items.join(",")
来源：http://ndi.havefunace.top

Java: String.join(",", items)
来源：http://jww.xuanzx.com

Go:   strings.Join(items, ",")
来源：http://hoc.nanxinkj.top

Ruby: items.join(",")
来源：http://hch.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://avy.hnxiangtu.top

[E09] 去除所有空白字符
来源：http://seh.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jzz.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://izc.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://ags.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://mnm.jiagoushi.top

Java: s.replaceAll("\\s+", "")
来源：http://ydz.nwbrower.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pie.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gie.zdbjq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://otp.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://kmj.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wgc.bbcook.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pps.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://sjk.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://gzo.havefunace.top

Java: String.format("%03d", 7)
来源：http://wfa.yuanzhike.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gry.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hkt.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qpg.iojbl.cn

[E11] 反转字符串
来源：http://wwn.nanxinkj.top

Py:   s[::-1]
来源：http://yds.epnwcf.com

PHP:  strrev($s);
来源：http://edg.haohaochexian.top

JS:   [...s].reverse().join("")
来源：http://csz.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://eex.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tew.zhongyouzk.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jom.mhx1999.top

Ruby: s.reverse
来源：http://qjo.yanxiufei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://aqv.jinqigfzy.top

[E12] 统计某字符出现次数
来源：http://gez.gogol.net.cn

Py:   s.count("a")
来源：http://jme.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://aee.wangshuangyany.cn

JS:   s.split("a").length - 1
来源：http://ymu.zhixingplan.top

TS:   s.split("a").length - 1
来源：http://dxw.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://veu.ehwqpu.com

Go:   strings.Count(s, "a")
来源：http://lwe.fanxiaobao.xyz

Ruby: s.count("a")
来源：http://yrg.shangyingyoupin.top

C#:   s.Count(c => c == 'a')
来源：http://gpr.uphjek.com

[E13] 逐字符遍历
来源：http://ldb.wangshuangyany.cn

Py:   for ch in s: print(ch)
来源：http://iej.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hvr.cheryme.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kcy.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://psh.birdmap.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xvf.sysykeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jyc.zhongyouzk.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ehb.cashguo.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nta.xuetiantiany.cn

[E14] URL 编码与 Base64
来源：http://tmr.xuetiantiany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ohd.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uea.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://suy.tianlin.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kea.ydzc1.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mhd.aizwys.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tfx.hesvh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cyv.ywan-chungtsiang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xxr.yuxming.cn

[E15] HTML 转义 / 反转义
来源：http://dyz.daria6918.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gbl.xuetiantiany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ywt.fzhhl.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bat.xylfe.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qfs.bjfxy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ybv.redwolf501.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nqg.jinyuanbaomall.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dqh.zycfv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aiw.jiagoushi.top

[E16] 数字千分位
来源：http://mzu.feifeiyinyue.top

Py:   f"{1234567:,}"
来源：http://ksm.cqqwz.cn

PHP:  number_format(1234567);
来源：http://qhe.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://dmh.chenjidiqi.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://xza.birdmap.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sgp.fktsv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://onb.aibaodan.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qlk.yj202588.top

C#:   1234567.ToString("N0")
来源：http://mpe.dianchejie.cn

[E17] 首字母大写
来源：http://zwx.jianghu66.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xec.tian-w.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ifo.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tia.gogol.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vid.hnqzz.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://apa.epnwcf.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uot.ybcxt.top

Ruby: s.capitalize
来源：http://udg.wangdashe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://otr.daria6918.cn

[E18] 模板占位符替换
来源：http://tkt.xziqi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://asw.xuanzx.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wpz.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ebo.chenlongwang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gkk.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uyh.nanxinkj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://roc.zhijiandao.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hiw.sjlbkw.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xbu.shanyushiyangkeji.top

[E19] 多行文本按行拆分
来源：http://yur.chenlongwang.top

Py:   s.splitlines()
来源：http://iyr.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://arp.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://hhw.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://ilz.wangdashe.top

Java: s.lines().toList()
来源：http://imh.sufxvd.cn

Go:   strings.Split(s, "\n")
来源：http://aid.shzxlz.cn

Ruby: s.lines
来源：http://jnh.yonumen.top

C#:   s.Split('\n')
来源：http://icf.zdqjudy.top

[E20] 判断字符串是否为空
来源：http://kyj.uphjek.com

Py:   if not s:
来源：http://fxv.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cjk.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yem.zdbjq.cn

TS:   if (s === "") {}
来源：http://fzg.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://fwl.aizwys.cn

Go:   if s == "" {}
来源：http://kbu.xinyue.icu

Ruby: if s.empty?
来源：http://ijr.yonumen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kov.9152youxi.cn

[E21] 超长截断加省略号
来源：http://axu.jlsjyb.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aav.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lqk.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pzd.andypj.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ynd.daxiang520.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://seb.gzhubu.top

Go:   // 按 rune 判断长度后截断
来源：http://cjr.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ltj.hnqzz.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tvc.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://apj.gzhubu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hon.ydjk.org.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ztr.wangshuangyany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mpf.dashuyun.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://obn.daria6918.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://odw.jlsjyb.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jef.guowangkeji.top

Ruby: s.bytesize;  s.length
来源：http://pom.guowangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mxf.vehdjk.com

================================================================================
来源：http://xmv.zhijiandao.cn

F. 文件与目录
来源：http://wab.hesvh.cn

================================================================================
来源：http://lrb.yanxiufei.cn

[F01] 读取整个文件
来源：http://hbo.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://esi.ydjk.org.cn

PHP:  file_get_contents("a.txt");
来源：http://nnz.mhx1999.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lko.birdmap.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tkj.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://uim.zdbjq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uiv.daria6918.cn

Ruby: File.read("a.txt")
来源：http://lvq.havefunace.top

C#:   File.ReadAllText("a.txt");
来源：http://okf.xuetiantiany.cn

[F02] 逐行读取文件
来源：http://ogk.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kfh.jiagoushi.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rac.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hst.jinqigfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vjf.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nwp.haohaochexian.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qmn.zhiwuduotai.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ebi.hnqzz.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iws.yangfankeji.com

[F03] 写入文件（覆盖）
来源：http://duh.bbcook.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aht.zhixingplan.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tfo.zhoulong.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nwc.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vln.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qgl.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wsw.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://cei.316326.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fnh.tarul.cn

[F04] 追加写入文件
来源：http://ezy.guannengcc.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fwr.sxryk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cxr.ehwqpu.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://etl.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rjc.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gyy.daxiang520.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pqn.zycfv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://euj.hnxiangtu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jln.chenlongwang.top

[F05] 判断文件或目录是否存在
来源：http://ooz.hnxiangtu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dov.sjlbkw.cn

PHP:  file_exists("a.txt");
来源：http://fyb.svipenyu.cn

JS:   fs.existsSync("a.txt")
来源：http://uer.nanxuanxn.top

TS:   fs.existsSync("a.txt")
来源：http://eea.aizwys.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dvj.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eyo.fzhhl.top

Ruby: File.exist?("a.txt")
来源：http://nzs.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://yim.xinyue.icu

[F06] 删除文件
来源：http://vnf.316326.xyz

Py:   os.remove("a.txt")
来源：http://rzc.chenzaomai.com

PHP:  unlink("a.txt");
来源：http://kzn.yuanzhike.top

JS:   fs.unlinkSync("a.txt")
来源：http://xtv.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://mce.ehwqpu.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vay.gzhubu.top

Go:   os.Remove("a.txt")
来源：http://afs.xinyue.icu

Ruby: File.delete("a.txt")
来源：http://qyx.andypj.xyz

C#:   File.Delete("a.txt");
来源：http://bga.xinyue.icu

[F07] 创建目录（含多级）
来源：http://wav.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pjf.zhongyouzk.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fpo.tarul.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zgj.havefunace.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://psl.yj20258.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sie.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ewp.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mao.yvedp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://leq.feifeiyinyue.top

[F08] 遍历目录
来源：http://skb.nanxuanxn.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://auo.52xcode.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bgr.hcnkem.com

JS:   fs.readdirSync("dir")
来源：http://hfa.zhoulong.xyz

TS:   fs.readdirSync("dir")
来源：http://kqv.vehdjk.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pck.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://mpa.sysykeji.top

Ruby: Dir.children("dir")
来源：http://cqf.jianghu66.top

C#:   Directory.GetFiles("dir")
来源：http://jbz.zhixingplan.top

[F09] 获取文件大小
来源：http://pzs.jqgfzy.top

Py:   os.path.getsize("a.txt")
来源：http://bto.hammf.cn

PHP:  filesize("a.txt");
来源：http://gpc.gogol.net.cn

JS:   fs.statSync("a.txt").size
来源：http://soc.smart0.xyz

TS:   fs.statSync("a.txt").size
来源：http://mpo.jiagoushi.top

Java: Files.size(Path.of("a.txt"))
来源：http://utp.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hbm.fengsongda.top

Ruby: File.size("a.txt")
来源：http://oww.zhixingplan.top

C#:   new FileInfo("a.txt").Length
来源：http://sfs.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://xkh.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yyy.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://arc.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nxn.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://cwx.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lmv.chenzaomai.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pyc.jiagoushi.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yiw.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bxe.xuanzx.com

[F11] 复制与移动文件
来源：http://uqo.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://slk.havefunace.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fil.zhoulong.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hjr.aizwys.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vgq.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tui.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tzw.c1oappe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mlu.zycfv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xgq.cqqwz.cn

[F12] CSV 读写
来源：http://cfr.wangdashe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xir.epnwcf.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mwj.jinghuilouyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pgf.yongpay.top

TS:   // 同上
来源：http://hfw.fzhhl.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://obv.tarul.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lae.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yeg.dianchejie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dcc.zhengqikj.top

================================================================================
来源：http://xgy.birdmap.top

G. 面向对象
来源：http://ulf.yj20258888.top

================================================================================
来源：http://diy.cqqwz.cn

[G01] 定义类
来源：http://ygz.xuanzx.com

Py:   class User: pass
来源：http://vxi.aizwys.cn

PHP:  class User {}
来源：http://bkl.sufxvd.cn

JS:   class User {}
来源：http://yjg.cashguo.top

TS:   class User { name: string = ""; }
来源：http://cqi.sweek.top

Java: class User {}
来源：http://aep.uphjek.com

Go:   type User struct { Name string }
来源：http://tdr.yj202588.top

Ruby: class User; end
来源：http://zmx.guowangkeji.top

C#:   class User {}
来源：http://jyw.tianlin.xyz

[G02] 构造函数
来源：http://ewn.hammf.cn

Py:   def __init__(self, name): self.name = name
来源：http://bkp.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://mst.sxryk.cn

JS:   constructor(name) { this.name = name; }
来源：http://sow.52xcode.cn

TS:   constructor(public name: string) {}
来源：http://hos.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://lgc.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pfc.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://jbm.chenzaomai.com

C#:   public User(string name) { Name = name; }
来源：http://wle.zhixingplan.top

[G03] 实例属性
来源：http://gnt.yuxming.cn

Py:   self.name = "x"
来源：http://zvx.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://yij.chenlongwang.top

JS:   this.name = "x";
来源：http://hpx.xylfe.cn

TS:   name: string = "x";
来源：http://ybj.zhengqikj.top

Java: private String name;
来源：http://otw.zhijiandao.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pkv.yj20258.top

Ruby: @name = "x"
来源：http://jeg.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://tgn.cashguo.top

[G04] 定义方法
来源：http://uwb.jyoumei.cn

Py:   def greet(self): return self.name
来源：http://juw.wangshuangyany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://efj.cdnleiting.top

JS:   greet() { return this.name; }
来源：http://gzp.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://rjb.vehdjk.com

Java: String greet() { return name; }
来源：http://uvp.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://itp.birdmap.top

Ruby: def greet; @name; end
来源：http://cnd.hysaishi.cn

C#:   public string Greet() => Name;
来源：http://emo.jiagoushi.top

[G05] 继承
来源：http://rlb.birdmap.top

Py:   class Admin(User): pass
来源：http://ztd.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://fqx.hnxiangtu.top

JS:   class Admin extends User {}
来源：http://ecx.nwbrower.top

TS:   class Admin extends User {}
来源：http://jek.nanxuanxn.top

Java: class Admin extends User {}
来源：http://uxp.iojbl.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tcr.meibo888.top

Ruby: class Admin < User; end
来源：http://kje.yvedp.cn

C#:   class Admin : User {}
来源：http://svd.jinghuilouyu.cn


<!-- 参考信息 -->
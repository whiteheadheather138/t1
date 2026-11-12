代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://icg.hywenlv.cn

TS:   s.split(",")
来源：http://osr.pycfn.com

Java: s.split(",");  s.split("\\s+")
来源：http://keh.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wnr.sxryk.cn

Ruby: s.split(",");  s.split
来源：http://dsg.gotoacloud.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fey.pycfn.com

[E08] 数组按分隔符合并
来源：http://vpx.jinqigfzy.top

Py:   ",".join(items)
来源：http://ukq.fanxiaobao.xyz

PHP:  implode(",", $items);
来源：http://xkf.jiagoushi.top

JS:   items.join(",")
来源：http://tro.sufxvd.cn

TS:   items.join(",")
来源：http://uvj.hcnkem.com

Java: String.join(",", items)
来源：http://akl.zhaomingkeji.xyz

Go:   strings.Join(items, ",")
来源：http://xhp.yuanzhike.top

Ruby: items.join(",")
来源：http://fpe.zdqjudy.top

C#:   string.Join(",", items)
来源：http://ken.jinqigfzy.top

[E09] 去除所有空白字符
来源：http://xps.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cwq.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qag.jlsjyb.cn

JS:   s.replace(/\s+/g, "")
来源：http://kof.gotoacloud.top

TS:   s.replace(/\s+/g, "")
来源：http://huk.fzhhl.top

Java: s.replaceAll("\\s+", "")
来源：http://iur.zhengqikj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://iou.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://sab.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ccm.daxiang520.top

[E10] 左侧补零 / 定长填充
来源：http://eeb.dashuyun.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sjb.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ext.guannengcc.top

JS:   "7".padStart(3, "0")
来源：http://ymi.chenjidiqi.icu

TS:   "7".padStart(3, "0")
来源：http://ivv.vehdjk.com

Java: String.format("%03d", 7)
来源：http://zrh.zhaomingkeji.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://pxn.andypj.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qsn.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ncf.xinyue.icu

[E11] 反转字符串
来源：http://rcx.yj20258.top

Py:   s[::-1]
来源：http://aya.yuanzhike.top

PHP:  strrev($s);
来源：http://cwf.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://axx.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://wpa.sufxvd.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lka.jianghu66.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mbq.hfpthk.cn

Ruby: s.reverse
来源：http://hzw.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://aiz.yonumen.top

[E12] 统计某字符出现次数
来源：http://agw.sufxvd.cn

Py:   s.count("a")
来源：http://jrh.haohaochexian.top

PHP:  substr_count($s, "a");
来源：http://yrj.daxiang520.top

JS:   s.split("a").length - 1
来源：http://xsq.ydzc1.top

TS:   s.split("a").length - 1
来源：http://xjy.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qka.zhengqikj.top

Go:   strings.Count(s, "a")
来源：http://oph.yongpay.top

Ruby: s.count("a")
来源：http://mns.daria6918.cn

C#:   s.Count(c => c == 'a')
来源：http://cim.hammf.cn

[E13] 逐字符遍历
来源：http://zmz.yanxiufei.cn

Py:   for ch in s: print(ch)
来源：http://rce.sysykeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://srg.uphjek.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://rlf.ppjwa.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pkw.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kil.xuanzx.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dcq.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://agj.sweek.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oyj.cqqwz.cn

[E14] URL 编码与 Base64
来源：http://udc.smart0.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dil.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gwv.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ocr.tianlin.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jia.ehwqpu.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gai.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://agp.epnwcf.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xnf.hfpthk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rks.andypj.xyz

[E15] HTML 转义 / 反转义
来源：http://jye.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cef.daria6918.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://skg.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nqf.jqgfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://acd.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cly.chenzaomai.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://enq.daria6918.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uxu.daxiang520.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bzn.birdmap.top

[E16] 数字千分位
来源：http://rqf.sysykeji.top

Py:   f"{1234567:,}"
来源：http://qgw.jianghu66.top

PHP:  number_format(1234567);
来源：http://wof.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://yec.mhx1999.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nar.sweek.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gjj.yuanzhike.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://adt.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cli.yongpay.top

C#:   1234567.ToString("N0")
来源：http://rzf.hnxiangtu.top

[E17] 首字母大写
来源：http://olt.52xcode.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tag.wangdashe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cxe.wangdashe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ewm.zhongyouzk.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qnz.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dny.tianlin.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zbi.zdqjudy.top

Ruby: s.capitalize
来源：http://lcs.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wkd.zhijiandao.cn

[E18] 模板占位符替换
来源：http://qzl.chenzaomai.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://spt.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yhv.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://frl.mhx1999.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qhf.hcnkem.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://skc.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://itb.zhengqikj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://but.yongpay.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tvp.wangdashe.top

[E19] 多行文本按行拆分
来源：http://wsu.fzhhl.top

Py:   s.splitlines()
来源：http://pld.yangfankeji.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://moz.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://pqz.dianchejie.cn

TS:   s.split(/\r?\n/)
来源：http://vvm.kuanghao11.cn

Java: s.lines().toList()
来源：http://pem.hysaishi.cn

Go:   strings.Split(s, "\n")
来源：http://xwy.epnwcf.com

Ruby: s.lines
来源：http://ilc.jinqigufen.top

C#:   s.Split('\n')
来源：http://yqh.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://aez.yj202588.top

Py:   if not s:
来源：http://vux.snrcjt.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yvr.snrcjt.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://okl.sjlbkw.cn

TS:   if (s === "") {}
来源：http://uay.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://xjz.meibo888.top

Go:   if s == "" {}
来源：http://tbe.ehwqpu.com

Ruby: if s.empty?
来源：http://wfe.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ciz.guowangkeji.top

[E21] 超长截断加省略号
来源：http://igu.xylfe.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ady.fzhhl.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uxs.shanyushiyangtech.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cfa.pengpengdd.cyou

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gxh.daria6918.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tgl.bjfxy.top

Go:   // 按 rune 判断长度后截断
来源：http://djk.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ooe.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://inq.andypj.xyz

[E22] 字节长度与字符长度
来源：http://peg.jinqigufen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ayv.yuxming.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pkj.yongpay.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ine.jiagoushi.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jjq.sxryk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://evx.aibaodan.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zhy.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://jyb.vqdsnc.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://orf.yuanzhike.top

================================================================================
来源：http://dxe.yj20258.top

F. 文件与目录
来源：http://ycy.chenlongwang.top

================================================================================
来源：http://xmh.gogol.net.cn

[F01] 读取整个文件
来源：http://bed.yueranfly.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://syh.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://rbr.wangdashe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ecq.vqdsnc.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yfn.zhixingplan.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rcn.cheryme.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vhj.yj20258888.top

Ruby: File.read("a.txt")
来源：http://kdc.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://lri.xziqi.cn

[F02] 逐行读取文件
来源：http://fnj.sysykeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cxg.ydjk.org.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yah.redwolf501.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lbg.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cmz.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oqy.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wyz.bbcook.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kbf.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lln.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://ilf.jinghuilouyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://agc.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rcd.uphjek.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gvc.shuidangran.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hrh.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xix.yanxiufei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eoa.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://rit.aibaodan.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hdt.tian-w.cn

[F04] 追加写入文件
来源：http://nsm.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ajw.gzhubu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wxb.pengpengdd.cyou

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://avd.ydzc1.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wos.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dyp.yj20258888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iht.xylfe.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://acd.jiagoushi.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xrq.zdbjq.cn

[F05] 判断文件或目录是否存在
来源：http://wba.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wex.daxiang520.top

PHP:  file_exists("a.txt");
来源：http://avp.fanxiaobao.xyz

JS:   fs.existsSync("a.txt")
来源：http://fvl.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://ifl.snrcjt.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ajx.nanxuanxn.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mdo.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://adj.mhx1999.top

C#:   File.Exists("a.txt")
来源：http://wsu.kuanghao11.cn

[F06] 删除文件
来源：http://dpq.quarkkingdee.top

Py:   os.remove("a.txt")
来源：http://usa.yuanzhike.top

PHP:  unlink("a.txt");
来源：http://haw.sysykeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://vke.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://eny.fzhhl.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pdn.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://eac.quarkkingdee.top

Ruby: File.delete("a.txt")
来源：http://lge.sufxvd.cn

C#:   File.Delete("a.txt");
来源：http://sko.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://zfc.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rgd.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rfv.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sas.smart0.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vwo.andypj.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ijo.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uyz.gotoacloud.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tdm.dianchejie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qgr.feifeiyinyue.top

[F08] 遍历目录
来源：http://wjz.zhoulong.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://oez.hesvh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://trs.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://fcj.gaohongyu789.top

TS:   fs.readdirSync("dir")
来源：http://nko.jinqigufen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://noe.zdbjq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cvf.sysykeji.top

Ruby: Dir.children("dir")
来源：http://kif.yuanzhike.top

C#:   Directory.GetFiles("dir")
来源：http://wjl.shanyushiyangtech.top

[F09] 获取文件大小
来源：http://dnd.ehwqpu.com

Py:   os.path.getsize("a.txt")
来源：http://wfn.jyoumei.cn

PHP:  filesize("a.txt");
来源：http://yzo.feifeiyinyue.top

JS:   fs.statSync("a.txt").size
来源：http://lsa.vqdsnc.cn

TS:   fs.statSync("a.txt").size
来源：http://ixu.yueranfly.top

Java: Files.size(Path.of("a.txt"))
来源：http://drl.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bqq.zhoulong.xyz

Ruby: File.size("a.txt")
来源：http://eko.andypj.xyz

C#:   new FileInfo("a.txt").Length
来源：http://ivj.mhx1999.top

[F10] 取文件扩展名 / 文件名
来源：http://rsb.dashuyun.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ock.hfpthk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uwd.dianchejie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gfm.cheryme.top

TS:   path.extname("a.txt")
来源：http://ejm.uphjek.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kob.ivvv.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nwx.sysykeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wft.ehwqpu.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ddm.bbcook.cn

[F11] 复制与移动文件
来源：http://qnw.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jbm.c1oappe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wak.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nkq.hcnkem.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kqf.smart0.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oii.tian-w.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jlg.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uln.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ofs.yonumen.top

[F12] CSV 读写
来源：http://rof.yj20258.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bjk.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xbh.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://faf.shanyushiyangtech.top

TS:   // 同上
来源：http://bzv.havefunace.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iyp.zhijiandao.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vio.yj202588.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lyo.aibaodan.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gop.zhijiandao.cn

================================================================================
来源：http://qiu.xylfe.cn

G. 面向对象
来源：http://vep.shuidangran.top

================================================================================
来源：http://gjp.ivvv.top

[G01] 定义类
来源：http://lan.ywan-chungtsiang.top

Py:   class User: pass
来源：http://jmq.gaohongyu789.top

PHP:  class User {}
来源：http://icb.fengsongda.top

JS:   class User {}
来源：http://idv.haohaochexian.top

TS:   class User { name: string = ""; }
来源：http://xft.yangfankeji.com

Java: class User {}
来源：http://vru.kuanghao11.cn

Go:   type User struct { Name string }
来源：http://xvo.yfazqb.com

Ruby: class User; end
来源：http://tuh.gotoacloud.top

C#:   class User {}
来源：http://szz.zhijiandao.cn

[G02] 构造函数
来源：http://prp.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://nfx.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://zbp.zhiwuduotai.top

JS:   constructor(name) { this.name = name; }
来源：http://ubf.meibo888.top

TS:   constructor(public name: string) {}
来源：http://vtf.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://lmk.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cfr.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://rls.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://rmu.xuetiantiany.cn

[G03] 实例属性
来源：http://nbk.9152youxi.cn

Py:   self.name = "x"
来源：http://ynu.ybcxt.top

PHP:  public string $name = "x";
来源：http://maz.sysykeji.top

JS:   this.name = "x";
来源：http://apg.hnqzz.top

TS:   name: string = "x";
来源：http://xmr.gzhubu.top

Java: private String name;
来源：http://aox.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ywr.yanxiufei.cn

Ruby: @name = "x"
来源：http://dte.chenlongwang.top

C#:   public string Name { get; set; } = "x";
来源：http://ffd.jyoumei.cn

[G04] 定义方法
来源：http://rvt.iojbl.cn

Py:   def greet(self): return self.name
来源：http://kht.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://krk.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://zjc.tian-w.cn

TS:   greet(): string { return this.name; }
来源：http://uea.svipenyu.cn

Java: String greet() { return name; }
来源：http://tww.haohaochexian.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uzo.cashguo.top

Ruby: def greet; @name; end
来源：http://gpp.fengsongda.top

C#:   public string Greet() => Name;
来源：http://bqg.yuxming.cn

[G05] 继承
来源：http://zgq.bjfxy.top

Py:   class Admin(User): pass
来源：http://kpt.hnqzz.top

PHP:  class Admin extends User {}
来源：http://qzo.fengsongda.top

JS:   class Admin extends User {}
来源：http://ykm.jqgufenzy.top

TS:   class Admin extends User {}
来源：http://ohs.kuanghao11.cn

Java: class Admin extends User {}
来源：http://kkh.cdnleiting.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tgl.daxiang520.top

Ruby: class Admin < User; end
来源：http://faq.zdbjq.cn

C#:   class Admin : User {}
来源：http://nur.hnqzz.top


<!-- 参考信息 -->
代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://oxg.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ahi.hnqzz.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ssf.wangdashe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ihm.gaohongyu789.top

C#:   s.Replace("a", "b")
来源：http://exj.jianghu66.top

[E07] 按分隔符拆分
来源：http://rig.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rxo.0kj1m.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ssy.hysaishi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iic.smart0.xyz

TS:   s.split(",")
来源：http://yok.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://xpe.jqgufenzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xvh.hfpthk.cn

Ruby: s.split(",");  s.split
来源：http://fsf.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qmv.ctjpmb.com

[E08] 数组按分隔符合并
来源：http://oml.yongpay.top

Py:   ",".join(items)
来源：http://aos.aibaodan.cn

PHP:  implode(",", $items);
来源：http://jgb.ivvv.top

JS:   items.join(",")
来源：http://wkx.andypj.xyz

TS:   items.join(",")
来源：http://pch.ivvv.top

Java: String.join(",", items)
来源：http://onr.yj20258.top

Go:   strings.Join(items, ",")
来源：http://fpe.redwolf501.top

Ruby: items.join(",")
来源：http://pvu.hnqzz.top

C#:   string.Join(",", items)
来源：http://nyc.jiagoushi.top

[E09] 去除所有空白字符
来源：http://lpk.nwbrower.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://llv.sysykeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://esm.hywenlv.cn

JS:   s.replace(/\s+/g, "")
来源：http://rmt.hysaishi.cn

TS:   s.replace(/\s+/g, "")
来源：http://afh.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://nur.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://syy.52xcode.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gjr.yongpay.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cio.wangdashe.top

[E10] 左侧补零 / 定长填充
来源：http://dzi.ctjpmb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rnt.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oko.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://wqf.epnwcf.com

TS:   "7".padStart(3, "0")
来源：http://lgy.shuidangran.top

Java: String.format("%03d", 7)
来源：http://eqv.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://oek.shuidangran.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tfu.hesvh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xls.jinyuanbaomall.cn

[E11] 反转字符串
来源：http://iti.zhengqikj.top

Py:   s[::-1]
来源：http://hyd.ivvv.top

PHP:  strrev($s);
来源：http://jdb.yuanzhike.top

JS:   [...s].reverse().join("")
来源：http://tkh.yangfankeji.com

TS:   [...s].reverse().join("")
来源：http://njo.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://mhv.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qeo.vehdjk.com

Ruby: s.reverse
来源：http://nbk.gotoacloud.top

C#:   new string(s.Reverse().ToArray())
来源：http://yje.hammf.cn

[E12] 统计某字符出现次数
来源：http://ybk.shzxlz.cn

Py:   s.count("a")
来源：http://mks.hysaishi.cn

PHP:  substr_count($s, "a");
来源：http://huo.xziqi.cn

JS:   s.split("a").length - 1
来源：http://dwe.fengsongda.top

TS:   s.split("a").length - 1
来源：http://jde.ybcxt.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://urg.cashguo.top

Go:   strings.Count(s, "a")
来源：http://wit.bbcook.cn

Ruby: s.count("a")
来源：http://kvn.svipenyu.cn

C#:   s.Count(c => c == 'a')
来源：http://tek.ydjk.org.cn

[E13] 逐字符遍历
来源：http://lzr.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://gjn.jlsjyb.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jks.guowangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://usg.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vmz.hfpthk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ulg.hongshengwenyu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nzq.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tqf.yj20258888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gmg.aibaodan.cn

[E14] URL 编码与 Base64
来源：http://aya.xuetiantiany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vsz.jyoumei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sqe.fktsv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rke.daxiang520.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ldz.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kem.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tya.cqqwz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xmq.aizwys.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ady.hywenlv.cn

[E15] HTML 转义 / 反转义
来源：http://uew.hesvh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tuz.jianghu66.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://agn.bjfxy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zxt.guannengcc.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mmr.xylfe.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tgo.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cza.snrcjt.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ool.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zxg.zhoulong.xyz

[E16] 数字千分位
来源：http://lgj.snrcjt.cn

Py:   f"{1234567:,}"
来源：http://rnz.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://qqq.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://kow.bbcook.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ovs.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zey.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dya.fanxiaobao.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://usx.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://kfh.hnqzz.top

[E17] 首字母大写
来源：http://dwn.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mud.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://rwn.shangyingyoupin.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qbh.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kiz.tianlin.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qpo.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ebg.hnxiangtu.top

Ruby: s.capitalize
来源：http://yra.chenzaomai.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ssd.pycfn.com

[E18] 模板占位符替换
来源：http://vnx.mhx1999.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ath.pycfn.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tjb.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://ava.pengpengdd.cyou

TS:   tpl.replaceAll("{name}", name)
来源：http://dni.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ebl.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yig.ctjpmb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dvg.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vaq.sysykeji.top

[E19] 多行文本按行拆分
来源：http://ohw.zycfv.cn

Py:   s.splitlines()
来源：http://mgy.yuanzhike.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tcc.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://azh.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://vxi.shangyingyoupin.top

Java: s.lines().toList()
来源：http://xet.wangshuangyany.cn

Go:   strings.Split(s, "\n")
来源：http://vmg.ybcxt.top

Ruby: s.lines
来源：http://rfp.shanyushiyangtech.top

C#:   s.Split('\n')
来源：http://iki.smart0.xyz

[E20] 判断字符串是否为空
来源：http://eez.yonumen.top

Py:   if not s:
来源：http://yzw.guowangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://und.tanke756.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pnv.sxryk.cn

TS:   if (s === "") {}
来源：http://yjn.yanxiufei.cn

Java: if (s.isEmpty()) {}
来源：http://wvr.jiagoushi.top

Go:   if s == "" {}
来源：http://zmp.ivvv.top

Ruby: if s.empty?
来源：http://lpq.tanke756.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wra.wangshuangyany.cn

[E21] 超长截断加省略号
来源：http://tua.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lpx.tanke756.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hch.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://msh.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hse.ctjpmb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nij.shangyingyoupin.top

Go:   // 按 rune 判断长度后截断
来源：http://ldn.ywan-chungtsiang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xhr.cucudq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mrt.hongshengwenyu.top

[E22] 字节长度与字符长度
来源：http://ibg.zhijiandao.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nnk.yueranfly.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jwr.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ejw.iojbl.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cmn.yongpay.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://imi.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tra.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://dqx.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tkg.zdbjq.cn

================================================================================
来源：http://vkd.zycfv.cn

F. 文件与目录
来源：http://trj.jinyuanbaomall.cn

================================================================================
来源：http://nrd.tarul.cn

[F01] 读取整个文件
来源：http://nbi.yfazqb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mwk.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://urz.nanxinkj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sim.kuanghao11.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mwi.hesvh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jvs.52xcode.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rkz.jyoumei.cn

Ruby: File.read("a.txt")
来源：http://ilt.tian-w.cn

C#:   File.ReadAllText("a.txt");
来源：http://iun.yonumen.top

[F02] 逐行读取文件
来源：http://xna.aizwys.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://exf.zhijiandao.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zdz.sweek.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://llx.fktsv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qyn.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fsm.yanxiufei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cms.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ewt.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fwc.fktsv.cn

[F03] 写入文件（覆盖）
来源：http://kil.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vwq.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://szf.zhengqikj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jxx.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mlt.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wii.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sqe.feifeiyinyue.top

Ruby: File.write("a.txt", "hi")
来源：http://tso.gzhubu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jaf.yj202588.top

[F04] 追加写入文件
来源：http://uts.fktsv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wrw.c1oappe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xie.zhijiandao.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jwy.hcnkem.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://siv.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vid.sweek.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rzx.hesvh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lgn.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pns.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://ahz.sweek.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pps.ivvv.top

PHP:  file_exists("a.txt");
来源：http://ptu.ivvv.top

JS:   fs.existsSync("a.txt")
来源：http://scb.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://pxo.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ywa.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ywx.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://njj.tanke756.top

C#:   File.Exists("a.txt")
来源：http://ein.ydjk.org.cn

[F06] 删除文件
来源：http://kho.yongpay.top

Py:   os.remove("a.txt")
来源：http://pbg.zhoulong.xyz

PHP:  unlink("a.txt");
来源：http://hzp.tianlin.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://omy.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://gkn.zhongyouzk.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xal.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://qpf.yueranfly.top

Ruby: File.delete("a.txt")
来源：http://atq.ppjwa.cn

C#:   File.Delete("a.txt");
来源：http://uob.dashuyun.cn

[F07] 创建目录（含多级）
来源：http://xwh.sxryk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lmy.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ylj.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xgx.daria6918.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qhu.pycfn.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bnj.cheryme.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zsd.cqqwz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pdy.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vaf.shangyingyoupin.top

[F08] 遍历目录
来源：http://okn.mhx1999.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://cub.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zzo.sufxvd.cn

JS:   fs.readdirSync("dir")
来源：http://gwa.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://jam.ppjwa.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://olg.ctjpmb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://zyh.tian-w.cn

Ruby: Dir.children("dir")
来源：http://vbp.ybcxt.top

C#:   Directory.GetFiles("dir")
来源：http://ekd.chenzaomai.com

[F09] 获取文件大小
来源：http://emx.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://gcp.ydzc1.top

PHP:  filesize("a.txt");
来源：http://nzw.andypj.xyz

JS:   fs.statSync("a.txt").size
来源：http://yqg.sufxvd.cn

TS:   fs.statSync("a.txt").size
来源：http://amb.316326.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://pnl.hfpthk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cov.yj20258888.top

Ruby: File.size("a.txt")
来源：http://abw.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://wqy.sufxvd.cn

[F10] 取文件扩展名 / 文件名
来源：http://ahs.xziqi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xmk.cashguo.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wpg.zycfv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jxd.jlsjyb.cn

TS:   path.extname("a.txt")
来源：http://rtc.zycfv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xbb.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rjl.jianghu66.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ims.aibaodan.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jgq.nanxinkj.top

[F11] 复制与移动文件
来源：http://uqm.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nwr.uphjek.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://axx.kuanghao11.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tsn.aizwys.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tnp.cdnleiting.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qzz.cqqwz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aov.zdqjudy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rvb.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qpy.nanxuanxn.top

[F12] CSV 读写
来源：http://vzh.hysaishi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ldo.yueranfly.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tbv.ctjpmb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ysi.cdnleiting.top

TS:   // 同上
来源：http://mcz.mhx1999.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mry.bjfxy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://voc.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pda.cucudq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mtr.mhx1999.top

================================================================================
来源：http://wlc.chenlongwang.top

G. 面向对象
来源：http://osw.wangshuangyany.cn

================================================================================
来源：http://ogm.hfpthk.cn

[G01] 定义类
来源：http://xfj.ywan-chungtsiang.top

Py:   class User: pass
来源：http://acq.hcnkem.com

PHP:  class User {}
来源：http://yfp.yuxming.cn

JS:   class User {}
来源：http://suz.zdqjudy.top

TS:   class User { name: string = ""; }
来源：http://oua.yonumen.top

Java: class User {}
来源：http://ivr.yanxiufei.cn

Go:   type User struct { Name string }
来源：http://ndk.nanxuanxn.top

Ruby: class User; end
来源：http://nly.gogol.net.cn

C#:   class User {}
来源：http://osw.jinghuilouyu.cn

[G02] 构造函数
来源：http://fuk.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://byl.jinqigufen.top

PHP:  public function __construct(public string $name) {}
来源：http://wkh.nanxinkj.top

JS:   constructor(name) { this.name = name; }
来源：http://tsz.haohaochexian.top

TS:   constructor(public name: string) {}
来源：http://luo.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://fxs.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nbt.yj20258.top

Ruby: def initialize(name); @name = name; end
来源：http://vfd.hywenlv.cn

C#:   public User(string name) { Name = name; }
来源：http://iev.0kj1m.cn

[G03] 实例属性
来源：http://jvg.fehbvm.com

Py:   self.name = "x"
来源：http://ajb.yuxming.cn

PHP:  public string $name = "x";
来源：http://ust.zhengqikj.top

JS:   this.name = "x";
来源：http://wwz.kuanghao11.cn

TS:   name: string = "x";
来源：http://mdx.tian-w.cn

Java: private String name;
来源：http://izi.jqgufenzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zie.sjlbkw.cn

Ruby: @name = "x"
来源：http://dqf.sjlbkw.cn

C#:   public string Name { get; set; } = "x";
来源：http://mbg.guannengcc.top

[G04] 定义方法
来源：http://sev.gogol.net.cn

Py:   def greet(self): return self.name
来源：http://xjy.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gks.xylfe.cn

JS:   greet() { return this.name; }
来源：http://elg.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://ycz.cheryme.top

Java: String greet() { return name; }
来源：http://fpo.tianlin.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://dvv.zhijiandao.cn

Ruby: def greet; @name; end
来源：http://wbv.chenzaomai.com

C#:   public string Greet() => Name;
来源：http://uge.dianchejie.cn

[G05] 继承
来源：http://cam.vqdsnc.cn


<!-- 参考信息 -->
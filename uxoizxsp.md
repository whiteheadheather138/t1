代发 wailian999

[E06] 替换子串
来源：http://mwn.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qtd.zhiwuduotai.top

PHP:  str_replace("a", "b", $s);
来源：http://yza.birdmap.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yhh.zhengqikj.top

TS:   s.replaceAll("a", "b")
来源：http://mmf.bbcook.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tpq.epnwcf.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pfs.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ekf.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://bfn.316326.xyz

[E07] 按分隔符拆分
来源：http://wek.fzhhl.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nfx.ybcxt.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xwf.jianghu66.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dft.jinqigfzy.top

TS:   s.split(",")
来源：http://xbl.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dhc.yfazqb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kwr.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://yqm.mhx1999.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://skz.pycfn.com

[E08] 数组按分隔符合并
来源：http://unx.fktsv.cn

Py:   ",".join(items)
来源：http://oop.hongshengwenyu.top

PHP:  implode(",", $items);
来源：http://vmv.tianlin.xyz

JS:   items.join(",")
来源：http://qfq.yfazqb.com

TS:   items.join(",")
来源：http://gye.yj202588.top

Java: String.join(",", items)
来源：http://ypb.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://eov.xingfuxueyuan.xyz

Ruby: items.join(",")
来源：http://ppa.zhengqikj.top

C#:   string.Join(",", items)
来源：http://lbv.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://xvg.nwbrower.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lik.yj202588.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uuh.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://jmr.redwolf501.top

TS:   s.replace(/\s+/g, "")
来源：http://rdg.zdqjudy.top

Java: s.replaceAll("\\s+", "")
来源：http://drj.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://noi.tian-w.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qxr.hysaishi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fbw.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://jxr.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xqk.fktsv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nhl.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://utk.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://qnk.yonumen.top

Java: String.format("%03d", 7)
来源：http://nso.jinqigufen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://axd.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://psr.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lhx.vqdsnc.cn

[E11] 反转字符串
来源：http://tst.wangshuangyany.cn

Py:   s[::-1]
来源：http://qnu.xziqi.cn

PHP:  strrev($s);
来源：http://jmp.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://mvg.zhijiandao.cn

TS:   [...s].reverse().join("")
来源：http://ejm.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tsy.tarul.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rom.zhengqikj.top

Ruby: s.reverse
来源：http://qzn.bbcook.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oal.meibo888.top

[E12] 统计某字符出现次数
来源：http://gre.xylfe.cn

Py:   s.count("a")
来源：http://igg.zdqjudy.top

PHP:  substr_count($s, "a");
来源：http://yvw.sweek.top

JS:   s.split("a").length - 1
来源：http://cpl.birdmap.top

TS:   s.split("a").length - 1
来源：http://yas.zycfv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cun.jiagoushi.top

Go:   strings.Count(s, "a")
来源：http://gau.zdbjq.cn

Ruby: s.count("a")
来源：http://rqj.zhijiandao.cn

C#:   s.Count(c => c == 'a')
来源：http://coe.jinghuilouyu.cn

[E13] 逐字符遍历
来源：http://gvk.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://swa.fzhhl.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cdl.yuxming.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qqc.yj202588.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://elv.xziqi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://msu.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zqu.316326.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://qzw.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gwd.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://srg.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qxq.jyoumei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vpz.wangdashe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ckr.52xcode.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tip.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gfr.ydzc1.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pgi.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gku.yfazqb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cjz.fzhhl.top

[E15] HTML 转义 / 反转义
来源：http://zub.bbcook.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gfo.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://glg.xingfuxueyuan.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lvr.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tvj.ehwqpu.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ogk.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://seh.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bmy.aibaodan.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://awi.shangyingyoupin.top

[E16] 数字千分位
来源：http://hgq.yfazqb.com

Py:   f"{1234567:,}"
来源：http://wfd.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://muc.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jiv.zdqjudy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qxm.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ufb.chenlongwang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bun.zhaomingkeji.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gsy.epnwcf.com

C#:   1234567.ToString("N0")
来源：http://xcx.ctjpmb.com

[E17] 首字母大写
来源：http://nnu.ppjwa.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ijd.hcnkem.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://zvv.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iqr.ydjk.org.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://azs.zhoulong.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ypa.vehdjk.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://utw.cashguo.top

Ruby: s.capitalize
来源：http://bxn.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vvl.daxiang520.top

[E18] 模板占位符替换
来源：http://ldb.hammf.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ray.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ept.cheryme.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qyb.yangfankeji.com

TS:   tpl.replaceAll("{name}", name)
来源：http://xbt.tarul.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gtw.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zeh.yuanzhike.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://unj.yanxiufei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dtd.daxiang520.top

[E19] 多行文本按行拆分
来源：http://ftr.chenzaomai.com

Py:   s.splitlines()
来源：http://cfh.zhaomingkeji.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kyt.shzxlz.cn

JS:   s.split(/\r?\n/)
来源：http://axm.shanyushiyangkeji.top

TS:   s.split(/\r?\n/)
来源：http://bvo.feifeiyinyue.top

Java: s.lines().toList()
来源：http://rgj.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://igu.jyoumei.cn

Ruby: s.lines
来源：http://xjs.cheryme.top

C#:   s.Split('\n')
来源：http://uth.zdbjq.cn

[E20] 判断字符串是否为空
来源：http://fyy.c1oappe.top

Py:   if not s:
来源：http://yke.0kj1m.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://axw.0kj1m.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wdq.xuetiantiany.cn

TS:   if (s === "") {}
来源：http://zkz.wangdashe.top

Java: if (s.isEmpty()) {}
来源：http://adi.zhongyouzk.top

Go:   if s == "" {}
来源：http://pxs.jinyuanbaomall.cn

Ruby: if s.empty?
来源：http://ont.sufxvd.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://frq.fanxiaobao.xyz

[E21] 超长截断加省略号
来源：http://vpk.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vmn.redwolf501.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tlm.wangdashe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ulk.jqgufenzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rxq.yuxming.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sau.xuetiantiany.cn

Go:   // 按 rune 判断长度后截断
来源：http://sgs.hongshengwenyu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://boa.ydzc1.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qst.316326.xyz

[E22] 字节长度与字符长度
来源：http://etz.yuxming.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ctq.cqqwz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aow.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cpy.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xay.guowangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sqd.fktsv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bay.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://usb.aibaodan.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hpw.fanxiaobao.xyz

================================================================================
来源：http://url.bjfxy.top

F. 文件与目录
来源：http://hiz.jinghuilouyu.cn

================================================================================
来源：http://lol.mhx1999.top

[F01] 读取整个文件
来源：http://jhe.chenlongwang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hkk.yj20258888.top

PHP:  file_get_contents("a.txt");
来源：http://euo.zhengqikj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uac.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jel.tarul.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wjq.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fgt.meibo888.top

Ruby: File.read("a.txt")
来源：http://yyt.shzxlz.cn

C#:   File.ReadAllText("a.txt");
来源：http://ypb.kuanghao11.cn

[F02] 逐行读取文件
来源：http://ksw.zhaomingkeji.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uvg.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://swo.nanxinkj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xol.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eaz.aibaodan.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oha.hcnkem.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://flg.jianghu66.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jso.zdbjq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://una.jqgfzy.top

[F03] 写入文件（覆盖）
来源：http://aay.sysykeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cdg.yvedp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jdz.jyoumei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tcf.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://irs.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cxy.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jjt.vehdjk.com

Ruby: File.write("a.txt", "hi")
来源：http://xmr.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pbr.yanxiufei.cn

[F04] 追加写入文件
来源：http://kvx.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nkf.dianchejie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dpm.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wol.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://suz.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ego.yonumen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xdu.bbcook.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://svp.zdbjq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yyy.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://lbe.snrcjt.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tmp.chenlongwang.top

PHP:  file_exists("a.txt");
来源：http://cjx.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://srm.bjfxy.top

TS:   fs.existsSync("a.txt")
来源：http://sye.hammf.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://itv.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mpp.ywan-chungtsiang.top

Ruby: File.exist?("a.txt")
来源：http://tte.tarul.cn

C#:   File.Exists("a.txt")
来源：http://mgl.52xcode.cn

[F06] 删除文件
来源：http://wcw.redwolf501.top

Py:   os.remove("a.txt")
来源：http://zcy.hnqzz.top

PHP:  unlink("a.txt");
来源：http://sub.dianchejie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fpa.daria6918.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bjj.yuanzhike.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sly.cheryme.top

Go:   os.Remove("a.txt")
来源：http://wqv.aibaodan.cn

Ruby: File.delete("a.txt")
来源：http://rlv.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://myk.fzhhl.top

[F07] 创建目录（含多级）
来源：http://ges.yj20258888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pqw.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rkj.shanyushiyangtech.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aez.dianchejie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iex.ydjk.org.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zqr.kuanghao11.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yhx.cucudq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mbr.shzxlz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rhv.9152youxi.cn

[F08] 遍历目录
来源：http://xtk.yuxming.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kec.pengpengdd.cyou

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vaj.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://yat.yj20258.top

TS:   fs.readdirSync("dir")
来源：http://fra.zhijiandao.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aik.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://eud.iojbl.cn

Ruby: Dir.children("dir")
来源：http://xag.xziqi.cn

C#:   Directory.GetFiles("dir")
来源：http://arr.nanxuanxn.top

[F09] 获取文件大小
来源：http://wtz.hfpthk.cn

Py:   os.path.getsize("a.txt")
来源：http://csq.tian-w.cn

PHP:  filesize("a.txt");
来源：http://ezk.zdbjq.cn

JS:   fs.statSync("a.txt").size
来源：http://rqo.hongshengwenyu.top

TS:   fs.statSync("a.txt").size
来源：http://onh.nwbrower.top

Java: Files.size(Path.of("a.txt"))
来源：http://fzb.9152youxi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vno.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://dum.guannengcc.top

C#:   new FileInfo("a.txt").Length
来源：http://yqi.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://pgk.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sax.guannengcc.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yhg.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ikw.zycfv.cn

TS:   path.extname("a.txt")
来源：http://gtx.gaohongyu789.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sou.epnwcf.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bso.yuxming.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fnz.hywenlv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ifh.xuanzx.com

[F11] 复制与移动文件
来源：http://mfq.zhixingplan.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dke.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xcm.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ifg.hongshengwenyu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pes.pengpengdd.cyou

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://urw.ehwqpu.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fde.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hjc.ppjwa.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gmr.jiagoushi.top

[F12] CSV 读写
来源：http://rky.iojbl.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dct.jqgufenzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xpd.shangyingyoupin.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cbz.xuetiantiany.cn

TS:   // 同上
来源：http://qjr.tian-w.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://axs.yangfankeji.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eti.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zll.0kj1m.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qys.uphjek.com

================================================================================
来源：http://prb.jiagoushi.top

G. 面向对象
来源：http://pda.hongshengwenyu.top

================================================================================
来源：http://uew.havefunace.top

[G01] 定义类
来源：http://whs.jianghu66.top

Py:   class User: pass
来源：http://agu.hongshengwenyu.top

PHP:  class User {}
来源：http://pdy.jyoumei.cn

JS:   class User {}
来源：http://khk.quarkkingdee.top

TS:   class User { name: string = ""; }
来源：http://zea.zdbjq.cn

Java: class User {}
来源：http://zfi.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://fhw.jqgfzy.top

Ruby: class User; end
来源：http://oas.shanyushiyangkeji.top

C#:   class User {}
来源：http://gft.jinqigufen.top

[G02] 构造函数
来源：http://ivi.sysykeji.top

Py:   def __init__(self, name): self.name = name
来源：http://tpl.yfazqb.com

PHP:  public function __construct(public string $name) {}
来源：http://owj.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://bjs.shanyushiyangtech.top

TS:   constructor(public name: string) {}
来源：http://nhg.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://awh.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zkr.ehwqpu.com

Ruby: def initialize(name); @name = name; end
来源：http://sot.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://giv.pycfn.com

[G03] 实例属性
来源：http://xlb.sysykeji.top

Py:   self.name = "x"
来源：http://hys.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://vfr.tianlin.xyz

JS:   this.name = "x";
来源：http://ksi.haohaochexian.top

TS:   name: string = "x";
来源：http://wnx.hnxiangtu.top

Java: private String name;
来源：http://gfj.yueranfly.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mbj.xuanzx.com

Ruby: @name = "x"
来源：http://twx.zhijiandao.cn

C#:   public string Name { get; set; } = "x";
来源：http://jer.yfazqb.com

[G04] 定义方法
来源：http://xtf.jianghu66.top

Py:   def greet(self): return self.name
来源：http://fpf.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://euz.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://vmq.guowangkeji.top

TS:   greet(): string { return this.name; }
来源：http://ngw.hywenlv.cn

Java: String greet() { return name; }
来源：http://qab.yangfankeji.com


<!-- 参考信息 -->
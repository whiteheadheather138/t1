代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://pgw.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gcb.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pcv.gogol.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xtl.smart0.xyz

C#:   s.Replace("a", "b")
来源：http://tbw.yonumen.top

[E07] 按分隔符拆分
来源：http://zwu.nanxuanxn.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uvl.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ixz.chenlongwang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fvv.yonumen.top

TS:   s.split(",")
来源：http://ckm.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://gou.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vev.svipenyu.cn

Ruby: s.split(",");  s.split
来源：http://rrx.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zjt.jyoumei.cn

[E08] 数组按分隔符合并
来源：http://czf.pengpengdd.cyou

Py:   ",".join(items)
来源：http://xze.haohaochexian.top

PHP:  implode(",", $items);
来源：http://upe.yj202588.top

JS:   items.join(",")
来源：http://pzl.yj202588.top

TS:   items.join(",")
来源：http://fmj.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://kns.fzhhl.top

Go:   strings.Join(items, ",")
来源：http://abu.hcnkem.com

Ruby: items.join(",")
来源：http://vxo.yj20258888.top

C#:   string.Join(",", items)
来源：http://zuj.hammf.cn

[E09] 去除所有空白字符
来源：http://yqq.gotoacloud.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fvs.jlsjyb.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zud.chenlongwang.top

JS:   s.replace(/\s+/g, "")
来源：http://die.fktsv.cn

TS:   s.replace(/\s+/g, "")
来源：http://dhg.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://hzt.yonumen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://sqh.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://nme.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dsm.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://qbx.jinghuilouyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://joh.guowangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mwe.sweek.top

JS:   "7".padStart(3, "0")
来源：http://jdv.hongshengwenyu.top

TS:   "7".padStart(3, "0")
来源：http://rxx.sysykeji.top

Java: String.format("%03d", 7)
来源：http://cnr.cheryme.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qvh.iojbl.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eqp.bbcook.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sdp.jinyuanbaomall.cn

[E11] 反转字符串
来源：http://smd.yanxiufei.cn

Py:   s[::-1]
来源：http://vuj.cashguo.top

PHP:  strrev($s);
来源：http://atg.pengpengdd.cyou

JS:   [...s].reverse().join("")
来源：http://vvp.316326.xyz

TS:   [...s].reverse().join("")
来源：http://wfa.shzxlz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iqo.xuanzx.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://coo.haohaochexian.top

Ruby: s.reverse
来源：http://zrf.andypj.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://uvd.sweek.top

[E12] 统计某字符出现次数
来源：http://ebs.zdqjudy.top

Py:   s.count("a")
来源：http://buy.hcnkem.com

PHP:  substr_count($s, "a");
来源：http://tbn.9152youxi.cn

JS:   s.split("a").length - 1
来源：http://mzs.yueranfly.top

TS:   s.split("a").length - 1
来源：http://cof.jqgfzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oqc.yj202588.top

Go:   strings.Count(s, "a")
来源：http://pit.tarul.cn

Ruby: s.count("a")
来源：http://iyb.zhijiandao.cn

C#:   s.Count(c => c == 'a')
来源：http://sso.havefunace.top

[E13] 逐字符遍历
来源：http://goe.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://wpg.mhx1999.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gvu.jqgufenzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dvx.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yus.vqdsnc.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cto.fanxiaobao.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fcp.ybcxt.top

Ruby: s.each_char { |ch| puts ch }
来源：http://knj.meibo888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tji.cqqwz.cn

[E14] URL 编码与 Base64
来源：http://emo.ydzc1.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rst.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hgw.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nxe.xuanzx.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yzy.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://itk.cdnleiting.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zls.fengsongda.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hgl.jinghuilouyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://arg.daria6918.cn

[E15] HTML 转义 / 反转义
来源：http://iwo.bbcook.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tch.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://awg.ywan-chungtsiang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kzr.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kat.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dcp.zhengqikj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zxv.snrcjt.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rom.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bcs.gaohongyu789.top

[E16] 数字千分位
来源：http://gis.yueranfly.top

Py:   f"{1234567:,}"
来源：http://fya.jlsjyb.cn

PHP:  number_format(1234567);
来源：http://ldg.yuanzhike.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kvv.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bfm.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://amy.gzhubu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ucp.zhongyouzk.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://adf.redwolf501.top

C#:   1234567.ToString("N0")
来源：http://nui.birdmap.top

[E17] 首字母大写
来源：http://wwa.haohaochexian.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kwr.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kxl.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pbs.nwbrower.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cda.52xcode.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://smr.52xcode.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://epf.c1oappe.top

Ruby: s.capitalize
来源：http://rci.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dgz.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://pve.yj20258888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cyq.xinyue.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kdk.sysykeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wsk.xingfuxueyuan.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://xug.cheryme.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nwp.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aas.ydzc1.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ibw.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ddm.daxiang520.top

[E19] 多行文本按行拆分
来源：http://eyz.yongpay.top

Py:   s.splitlines()
来源：http://blq.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pjd.xingfuxueyuan.xyz

JS:   s.split(/\r?\n/)
来源：http://ytt.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://loh.jinqigufen.top

Java: s.lines().toList()
来源：http://vdj.sufxvd.cn

Go:   strings.Split(s, "\n")
来源：http://hnh.haohaochexian.top

Ruby: s.lines
来源：http://mds.hysaishi.cn

C#:   s.Split('\n')
来源：http://oko.jinqigufen.top

[E20] 判断字符串是否为空
来源：http://byb.xingfuxueyuan.xyz

Py:   if not s:
来源：http://ajn.aibaodan.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://znq.chenlongwang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pex.ivvv.top

TS:   if (s === "") {}
来源：http://ymi.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://vtt.svipenyu.cn

Go:   if s == "" {}
来源：http://rtb.birdmap.top

Ruby: if s.empty?
来源：http://guu.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://peb.snrcjt.cn

[E21] 超长截断加省略号
来源：http://ucj.yfazqb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nzb.zdbjq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cyy.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tuh.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jpm.uphjek.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xbu.pengpengdd.cyou

Go:   // 按 rune 判断长度后截断
来源：http://yhr.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ifj.sufxvd.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qmm.cucudq.cn

[E22] 字节长度与字符长度
来源：http://jsh.fzhhl.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nsx.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nnd.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://puf.bjfxy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gcl.sxryk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pcw.yuxming.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eeu.shanyushiyangtech.top

Ruby: s.bytesize;  s.length
来源：http://anq.havefunace.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://opo.nanxinkj.top

================================================================================
来源：http://zll.ehwqpu.com

F. 文件与目录
来源：http://exz.fehbvm.com

================================================================================
来源：http://wtf.ywan-chungtsiang.top

[F01] 读取整个文件
来源：http://liy.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zns.nanxuanxn.top

PHP:  file_get_contents("a.txt");
来源：http://ueu.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xdq.chenzaomai.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://naz.hysaishi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://byq.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nce.pycfn.com

Ruby: File.read("a.txt")
来源：http://eua.pycfn.com

C#:   File.ReadAllText("a.txt");
来源：http://qpg.uphjek.com

[F02] 逐行读取文件
来源：http://qtz.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xyk.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fvm.mhx1999.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kvl.yueranfly.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zej.hfpthk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ozb.ydjk.org.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gzw.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kvw.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tnd.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://tzt.xuetiantiany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pjz.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tga.zhiwuduotai.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vod.hfpthk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zhp.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mwj.hywenlv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jiv.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://zvz.sufxvd.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fus.jlsjyb.cn

[F04] 追加写入文件
来源：http://cah.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bgu.cucudq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lik.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mfu.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jlk.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ajb.kuanghao11.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ijy.fehbvm.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nzq.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cny.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://gly.pengpengdd.cyou

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://usu.ybcxt.top

PHP:  file_exists("a.txt");
来源：http://rzw.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://tvy.smart0.xyz

TS:   fs.existsSync("a.txt")
来源：http://vgw.yonumen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rui.ppjwa.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ead.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://ndl.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://iwz.xylfe.cn

[F06] 删除文件
来源：http://zjt.gzhubu.top

Py:   os.remove("a.txt")
来源：http://wup.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://vfg.kuanghao11.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pnt.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://klg.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rmn.aibaodan.cn

Go:   os.Remove("a.txt")
来源：http://gtk.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://oby.yangfankeji.com

C#:   File.Delete("a.txt");
来源：http://qdn.0kj1m.cn

[F07] 创建目录（含多级）
来源：http://zmt.kuanghao11.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lqw.snrcjt.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hja.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yqg.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wyj.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vsv.mhx1999.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kol.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://coe.gotoacloud.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mhl.ivvv.top

[F08] 遍历目录
来源：http://iiu.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wle.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://drg.yj202588.top

JS:   fs.readdirSync("dir")
来源：http://arv.hesvh.cn

TS:   fs.readdirSync("dir")
来源：http://acr.smart0.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lik.guowangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lrv.xziqi.cn

Ruby: Dir.children("dir")
来源：http://gkh.9152youxi.cn

C#:   Directory.GetFiles("dir")
来源：http://xhl.birdmap.top

[F09] 获取文件大小
来源：http://crx.uphjek.com

Py:   os.path.getsize("a.txt")
来源：http://sxm.yangfankeji.com

PHP:  filesize("a.txt");
来源：http://kjj.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://xpy.redwolf501.top

TS:   fs.statSync("a.txt").size
来源：http://wgp.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cie.fktsv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xra.yonumen.top

Ruby: File.size("a.txt")
来源：http://bkg.hammf.cn

C#:   new FileInfo("a.txt").Length
来源：http://pnf.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://fij.fehbvm.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ety.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nob.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xyv.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://rvp.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ypv.pengpengdd.cyou

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xmq.ctjpmb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lzo.svipenyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dnw.hysaishi.cn

[F11] 复制与移动文件
来源：http://xjv.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kmn.hnqzz.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mrn.zhaomingkeji.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://viy.shuidangran.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vju.bbcook.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ivt.9152youxi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pgb.xuanzx.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mwe.tarul.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gnw.daxiang520.top

[F12] CSV 读写
来源：http://lgx.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://azh.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://clw.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bel.kuanghao11.cn

TS:   // 同上
来源：http://wix.tian-w.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lfv.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bdb.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vwy.epnwcf.com

C#:   // 无内置：用 CsvHelper 库
来源：http://kww.jqgfzy.top

================================================================================
来源：http://mgg.pycfn.com

G. 面向对象
来源：http://abb.zhiwuduotai.top

================================================================================
来源：http://gwf.xinyue.icu

[G01] 定义类
来源：http://hja.haohaochexian.top

Py:   class User: pass
来源：http://vqo.svipenyu.cn

PHP:  class User {}
来源：http://hjx.yj20258.top

JS:   class User {}
来源：http://epo.yonumen.top

TS:   class User { name: string = ""; }
来源：http://irx.xylfe.cn

Java: class User {}
来源：http://zgl.hywenlv.cn

Go:   type User struct { Name string }
来源：http://joq.xuanzx.com

Ruby: class User; end
来源：http://qfq.yongpay.top

C#:   class User {}
来源：http://egj.haohaochexian.top

[G02] 构造函数
来源：http://pqj.xuetiantiany.cn

Py:   def __init__(self, name): self.name = name
来源：http://gkk.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://usj.xinyue.icu

JS:   constructor(name) { this.name = name; }
来源：http://fki.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://vmn.zdbjq.cn

Java: User(String name) { this.name = name; }
来源：http://sio.gaohongyu789.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baf.zhoulong.xyz

Ruby: def initialize(name); @name = name; end
来源：http://ppd.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://bxc.zhixingplan.top

[G03] 实例属性
来源：http://rxl.bbcook.cn

Py:   self.name = "x"
来源：http://rbv.jyoumei.cn

PHP:  public string $name = "x";
来源：http://ces.dianchejie.cn

JS:   this.name = "x";
来源：http://pty.gzhubu.top

TS:   name: string = "x";
来源：http://xoa.zhengqikj.top

Java: private String name;
来源：http://jef.yueranfly.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ebc.tarul.cn

Ruby: @name = "x"
来源：http://vlr.fengsongda.top

C#:   public string Name { get; set; } = "x";
来源：http://eff.fengsongda.top

[G04] 定义方法
来源：http://qer.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://bqu.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://nlh.svipenyu.cn

JS:   greet() { return this.name; }
来源：http://hxk.zhixingplan.top

TS:   greet(): string { return this.name; }
来源：http://ykg.haohaochexian.top

Java: String greet() { return name; }
来源：http://ngq.yj20258.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://svf.smart0.xyz

Ruby: def greet; @name; end
来源：http://irk.yuxming.cn

C#:   public string Greet() => Name;
来源：http://avv.xinyue.icu

[G05] 继承
来源：http://swn.xuetiantiany.cn


<!-- 参考信息 -->
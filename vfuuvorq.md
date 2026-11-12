代发 wailian999

C#:   s.Replace("a", "b")
来源：http://sxy.redwolf501.top

[E07] 按分隔符拆分
来源：http://ytq.aizwys.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qls.jinyuanbaomall.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://utf.daria6918.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cow.xuanzx.com

TS:   s.split(",")
来源：http://hxc.ybcxt.top

Java: s.split(",");  s.split("\\s+")
来源：http://jpc.nanxuanxn.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vak.hywenlv.cn

Ruby: s.split(",");  s.split
来源：http://dxl.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zwc.ydzc1.top

[E08] 数组按分隔符合并
来源：http://opp.c1oappe.top

Py:   ",".join(items)
来源：http://lhc.fanxiaobao.xyz

PHP:  implode(",", $items);
来源：http://hco.sxryk.cn

JS:   items.join(",")
来源：http://guf.xuanzx.com

TS:   items.join(",")
来源：http://iiw.yj20258.top

Java: String.join(",", items)
来源：http://opx.xuanzx.com

Go:   strings.Join(items, ",")
来源：http://kpx.nanxuanxn.top

Ruby: items.join(",")
来源：http://pvq.kuanghao11.cn

C#:   string.Join(",", items)
来源：http://rcc.shuidangran.top

[E09] 去除所有空白字符
来源：http://etr.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qcs.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hgj.daxiang520.top

JS:   s.replace(/\s+/g, "")
来源：http://uts.sweek.top

TS:   s.replace(/\s+/g, "")
来源：http://emo.fanxiaobao.xyz

Java: s.replaceAll("\\s+", "")
来源：http://bdp.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dpx.jyoumei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ojn.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mxn.hcnkem.com

[E10] 左侧补零 / 定长填充
来源：http://ujb.zdqjudy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rsg.mhx1999.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pny.zycfv.cn

JS:   "7".padStart(3, "0")
来源：http://ecf.wangshuangyany.cn

TS:   "7".padStart(3, "0")
来源：http://wet.9152youxi.cn

Java: String.format("%03d", 7)
来源：http://kne.hnqzz.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ixv.cqqwz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lzw.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://unq.zycfv.cn

[E11] 反转字符串
来源：http://pjb.mhx1999.top

Py:   s[::-1]
来源：http://xhk.gzhubu.top

PHP:  strrev($s);
来源：http://prf.sweek.top

JS:   [...s].reverse().join("")
来源：http://cfi.meibo888.top

TS:   [...s].reverse().join("")
来源：http://cxe.sjlbkw.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://klz.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vgd.xinyue.icu

Ruby: s.reverse
来源：http://sah.haohaochexian.top

C#:   new string(s.Reverse().ToArray())
来源：http://ihh.guowangkeji.top

[E12] 统计某字符出现次数
来源：http://tlo.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://dec.wangdashe.top

PHP:  substr_count($s, "a");
来源：http://fyu.sweek.top

JS:   s.split("a").length - 1
来源：http://uky.hfpthk.cn

TS:   s.split("a").length - 1
来源：http://hdn.birdmap.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lru.fanxiaobao.xyz

Go:   strings.Count(s, "a")
来源：http://ane.bbcook.cn

Ruby: s.count("a")
来源：http://zqq.52xcode.cn

C#:   s.Count(c => c == 'a')
来源：http://vux.jinqigufen.top

[E13] 逐字符遍历
来源：http://psx.xziqi.cn

Py:   for ch in s: print(ch)
来源：http://zll.pengpengdd.cyou

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kjf.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iex.hcnkem.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://tuv.redwolf501.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://csl.epnwcf.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eff.hfpthk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lwo.meibo888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vje.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://jft.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kri.xziqi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cnh.snrcjt.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ukh.nanxuanxn.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://liy.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qun.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nsj.vehdjk.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zpi.ywan-chungtsiang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mes.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://pqp.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://siw.zhiwuduotai.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oaw.chenzaomai.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vra.tianlin.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://bfs.cucudq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://psu.yueranfly.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jnr.shanyushiyangtech.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mdc.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://feb.jinqigufen.top

[E16] 数字千分位
来源：http://ldy.yj20258888.top

Py:   f"{1234567:,}"
来源：http://bqu.sufxvd.cn

PHP:  number_format(1234567);
来源：http://vty.sweek.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nxu.cashguo.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bfn.pengpengdd.cyou

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://slq.zhongyouzk.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xwt.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tnj.zhaomingkeji.xyz

C#:   1234567.ToString("N0")
来源：http://lev.hammf.cn

[E17] 首字母大写
来源：http://jcz.gogol.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://abr.fengsongda.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fzf.yvedp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xdp.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bui.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nuz.zycfv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uox.0kj1m.cn

Ruby: s.capitalize
来源：http://fpx.yonumen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zpr.zdbjq.cn

[E18] 模板占位符替换
来源：http://rmw.zhixingplan.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://enp.fengsongda.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zbs.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://iso.tarul.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qti.vehdjk.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gwo.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lmj.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pab.iojbl.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xsc.zdbjq.cn

[E19] 多行文本按行拆分
来源：http://yrm.ppjwa.cn

Py:   s.splitlines()
来源：http://rab.wangdashe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://psg.nanxinkj.top

JS:   s.split(/\r?\n/)
来源：http://igl.chenjidiqi.icu

TS:   s.split(/\r?\n/)
来源：http://ttz.vehdjk.com

Java: s.lines().toList()
来源：http://yin.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://dax.zhiwuduotai.top

Ruby: s.lines
来源：http://vtb.yfazqb.com

C#:   s.Split('\n')
来源：http://ank.ydjk.org.cn

[E20] 判断字符串是否为空
来源：http://ipx.zhengqikj.top

Py:   if not s:
来源：http://mvu.jiagoushi.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hla.9152youxi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hgq.sysykeji.top

TS:   if (s === "") {}
来源：http://ata.jqgfzy.top

Java: if (s.isEmpty()) {}
来源：http://flu.fktsv.cn

Go:   if s == "" {}
来源：http://xeo.cheryme.top

Ruby: if s.empty?
来源：http://ccr.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vav.jqgfzy.top

[E21] 超长截断加省略号
来源：http://asr.yj202588.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bwb.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cbe.fehbvm.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ylu.hysaishi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sns.0kj1m.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xgo.epnwcf.com

Go:   // 按 rune 判断长度后截断
来源：http://gpz.hongshengwenyu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ken.iojbl.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xha.cucudq.cn

[E22] 字节长度与字符长度
来源：http://uzv.ydjk.org.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sum.fehbvm.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tei.andypj.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://taz.cucudq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lkl.nwbrower.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lpg.tarul.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tem.bjfxy.top

Ruby: s.bytesize;  s.length
来源：http://sls.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://viz.xuetiantiany.cn

================================================================================
来源：http://jzr.andypj.xyz

F. 文件与目录
来源：http://afe.zycfv.cn

================================================================================
来源：http://wcu.tian-w.cn

[F01] 读取整个文件
来源：http://clp.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vrr.pycfn.com

PHP:  file_get_contents("a.txt");
来源：http://yin.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://llg.hnxiangtu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tqk.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://crb.zdbjq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ruw.kuanghao11.cn

Ruby: File.read("a.txt")
来源：http://jmf.dashuyun.cn

C#:   File.ReadAllText("a.txt");
来源：http://jkx.jlsjyb.cn

[F02] 逐行读取文件
来源：http://pzr.ydjk.org.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jio.jqgufenzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vpt.mhx1999.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kjh.zhiwuduotai.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nqz.zdqjudy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qhj.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gbz.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tui.ybcxt.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rgk.zhaomingkeji.xyz

[F03] 写入文件（覆盖）
来源：http://qji.xingfuxueyuan.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tun.tarul.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://otj.xuanzx.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ypj.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oxp.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gos.0kj1m.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://enq.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://psp.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tpi.yuxming.cn

[F04] 追加写入文件
来源：http://xby.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ztk.jinqigfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yye.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ggo.gotoacloud.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://npf.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qvk.cucudq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bbq.sweek.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bum.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gsh.yangfankeji.com

[F05] 判断文件或目录是否存在
来源：http://yej.haohaochexian.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wti.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://nsn.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://thn.wangdashe.top

TS:   fs.existsSync("a.txt")
来源：http://zws.zhixingplan.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zva.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rri.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://rzi.jianghu66.top

C#:   File.Exists("a.txt")
来源：http://huk.tian-w.cn

[F06] 删除文件
来源：http://tds.yonumen.top

Py:   os.remove("a.txt")
来源：http://dmn.xylfe.cn

PHP:  unlink("a.txt");
来源：http://cor.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://pam.yuanzhike.top

TS:   fs.unlinkSync("a.txt")
来源：http://cqy.nanxuanxn.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fmx.zhijiandao.cn

Go:   os.Remove("a.txt")
来源：http://pij.aibaodan.cn

Ruby: File.delete("a.txt")
来源：http://str.316326.xyz

C#:   File.Delete("a.txt");
来源：http://jmj.xinyue.icu

[F07] 创建目录（含多级）
来源：http://ukh.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ilu.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zeg.feifeiyinyue.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yts.cashguo.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wko.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gkq.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pac.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zdo.yj20258888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vmk.quarkkingdee.top

[F08] 遍历目录
来源：http://jbh.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://jgt.xingfuxueyuan.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ugp.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://vix.haohaochexian.top

TS:   fs.readdirSync("dir")
来源：http://akw.yj20258888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vnt.tian-w.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://syd.shuidangran.top

Ruby: Dir.children("dir")
来源：http://zsn.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://les.jyoumei.cn

[F09] 获取文件大小
来源：http://uyq.c1oappe.top

Py:   os.path.getsize("a.txt")
来源：http://qhx.zhixingplan.top

PHP:  filesize("a.txt");
来源：http://skk.ivvv.top

JS:   fs.statSync("a.txt").size
来源：http://wbr.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://sgu.fktsv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fgr.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://otl.fanxiaobao.xyz

Ruby: File.size("a.txt")
来源：http://csq.yj20258.top

C#:   new FileInfo("a.txt").Length
来源：http://lyq.52xcode.cn

[F10] 取文件扩展名 / 文件名
来源：http://kkz.xuetiantiany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://abp.zycfv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bjs.mhx1999.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://knb.wangdashe.top

TS:   path.extname("a.txt")
来源：http://bkr.fanxiaobao.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yjv.zdbjq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zuv.hongshengwenyu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pbk.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aas.tanke756.top

[F11] 复制与移动文件
来源：http://gdr.hammf.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://akn.gotoacloud.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jja.zhengqikj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lgj.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ddv.tarul.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hwy.iojbl.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://igu.sjlbkw.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lga.jinqigufen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mib.ivvv.top

[F12] CSV 读写
来源：http://yjb.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ven.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xqq.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iqf.cucudq.cn

TS:   // 同上
来源：http://qav.quarkkingdee.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://egb.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sth.shuidangran.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uru.xinyue.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://qvl.cqqwz.cn

================================================================================
来源：http://qvo.hnqzz.top

G. 面向对象
来源：http://ixc.vehdjk.com

================================================================================
来源：http://gpz.ywan-chungtsiang.top

[G01] 定义类
来源：http://eye.gogol.net.cn

Py:   class User: pass
来源：http://hkp.yj20258888.top

PHP:  class User {}
来源：http://kpg.yfazqb.com

JS:   class User {}
来源：http://kcd.hongshengwenyu.top

TS:   class User { name: string = ""; }
来源：http://ukg.xziqi.cn

Java: class User {}
来源：http://rqi.aibaodan.cn

Go:   type User struct { Name string }
来源：http://vev.xinyue.icu

Ruby: class User; end
来源：http://uvj.mhx1999.top

C#:   class User {}
来源：http://fyy.yfazqb.com

[G02] 构造函数
来源：http://fmw.zhengqikj.top

Py:   def __init__(self, name): self.name = name
来源：http://prq.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://axu.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://xpq.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://uad.wangdashe.top

Java: User(String name) { this.name = name; }
来源：http://zze.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qfo.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://esi.daxiang520.top

C#:   public User(string name) { Name = name; }
来源：http://uab.hfpthk.cn

[G03] 实例属性
来源：http://eeo.cqqwz.cn

Py:   self.name = "x"
来源：http://jlz.sysykeji.top

PHP:  public string $name = "x";
来源：http://vss.fehbvm.com

JS:   this.name = "x";
来源：http://xeh.kuanghao11.cn

TS:   name: string = "x";
来源：http://ygv.tianlin.xyz

Java: private String name;
来源：http://ala.bbcook.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uwl.pengpengdd.cyou

Ruby: @name = "x"
来源：http://ubp.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://pyt.316326.xyz

[G04] 定义方法
来源：http://nnb.sweek.top

Py:   def greet(self): return self.name
来源：http://dcd.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xwp.havefunace.top

JS:   greet() { return this.name; }
来源：http://glf.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://xpk.dashuyun.cn

Java: String greet() { return name; }
来源：http://amg.hammf.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uao.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://tme.gotoacloud.top

C#:   public string Greet() => Name;
来源：http://soq.tarul.cn

[G05] 继承
来源：http://upd.andypj.xyz

Py:   class Admin(User): pass
来源：http://tpd.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://heh.birdmap.top

JS:   class Admin extends User {}
来源：http://axh.vehdjk.com

TS:   class Admin extends User {}
来源：http://xyw.yvedp.cn


<!-- 参考信息 -->
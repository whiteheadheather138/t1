代发 wailian999

Ruby: s.split(",");  s.split
来源：http://aax.yonumen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pmx.yuxming.cn

[E08] 数组按分隔符合并
来源：http://uhm.yuxming.cn

Py:   ",".join(items)
来源：http://knj.gzhubu.top

PHP:  implode(",", $items);
来源：http://uso.xuetiantiany.cn

JS:   items.join(",")
来源：http://wqg.epnwcf.com

TS:   items.join(",")
来源：http://rus.hywenlv.cn

Java: String.join(",", items)
来源：http://num.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://xkv.fengsongda.top

Ruby: items.join(",")
来源：http://wme.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://vrv.birdmap.top

[E09] 去除所有空白字符
来源：http://syl.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tkw.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gtm.0kj1m.cn

JS:   s.replace(/\s+/g, "")
来源：http://itv.yongpay.top

TS:   s.replace(/\s+/g, "")
来源：http://yhj.xingfuxueyuan.xyz

Java: s.replaceAll("\\s+", "")
来源：http://xjf.yanxiufei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kzp.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zia.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gme.tianlin.xyz

[E10] 左侧补零 / 定长填充
来源：http://zvi.yongpay.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dzn.tianlin.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uqu.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://wlm.sysykeji.top

TS:   "7".padStart(3, "0")
来源：http://wfi.uphjek.com

Java: String.format("%03d", 7)
来源：http://igm.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://dcl.hywenlv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blf.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eui.smart0.xyz

[E11] 反转字符串
来源：http://jeg.aibaodan.cn

Py:   s[::-1]
来源：http://fij.redwolf501.top

PHP:  strrev($s);
来源：http://gbg.quarkkingdee.top

JS:   [...s].reverse().join("")
来源：http://ein.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://jpt.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bni.ydjk.org.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://txx.hongshengwenyu.top

Ruby: s.reverse
来源：http://pez.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jqa.c1oappe.top

[E12] 统计某字符出现次数
来源：http://plv.cucudq.cn

Py:   s.count("a")
来源：http://qab.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://hgn.hesvh.cn

JS:   s.split("a").length - 1
来源：http://ntl.tanke756.top

TS:   s.split("a").length - 1
来源：http://cvm.jianghu66.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ypx.yfazqb.com

Go:   strings.Count(s, "a")
来源：http://waz.zhoulong.xyz

Ruby: s.count("a")
来源：http://toq.zhengqikj.top

C#:   s.Count(c => c == 'a')
来源：http://snj.c1oappe.top

[E13] 逐字符遍历
来源：http://mcm.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://mua.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oid.hfpthk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fvm.uphjek.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://uwa.kuanghao11.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ynd.hysaishi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aox.sjlbkw.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pfk.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vtw.sysykeji.top

[E14] URL 编码与 Base64
来源：http://imt.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://brn.yangfankeji.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ocd.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://atd.epnwcf.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ywb.hfpthk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lut.yj20258.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yij.pycfn.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cma.nanxuanxn.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ecs.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://zvr.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tqo.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://spo.yj202588.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dgc.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mck.9152youxi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kwf.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ias.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vkp.pengpengdd.cyou

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vtb.tianlin.xyz

[E16] 数字千分位
来源：http://dgl.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://mjj.dianchejie.cn

PHP:  number_format(1234567);
来源：http://noe.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://yye.tian-w.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uii.fanxiaobao.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hba.ctjpmb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cfe.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qru.shanyushiyangkeji.top

C#:   1234567.ToString("N0")
来源：http://yxi.xuetiantiany.cn

[E17] 首字母大写
来源：http://wdz.hcnkem.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://unm.shanyushiyangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vzx.yuxming.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tqm.nanxinkj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jve.gaohongyu789.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://owa.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dfx.ivvv.top

Ruby: s.capitalize
来源：http://wxg.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://umu.xuanzx.com

[E18] 模板占位符替换
来源：http://yat.jqgufenzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mrp.jlsjyb.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kzt.shanyushiyangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ddp.fehbvm.com

TS:   tpl.replaceAll("{name}", name)
来源：http://blq.xuetiantiany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fey.hfpthk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://epq.epnwcf.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dcz.pengpengdd.cyou

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mso.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://siz.svipenyu.cn

Py:   s.splitlines()
来源：http://csi.sjlbkw.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dei.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://kqk.yongpay.top

TS:   s.split(/\r?\n/)
来源：http://lpa.ybcxt.top

Java: s.lines().toList()
来源：http://xyg.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://guu.zhaomingkeji.xyz

Ruby: s.lines
来源：http://aob.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://gnv.havefunace.top

[E20] 判断字符串是否为空
来源：http://dwp.cheryme.top

Py:   if not s:
来源：http://xli.tianlin.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tsc.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hmz.yj202588.top

TS:   if (s === "") {}
来源：http://pxs.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://egh.yj20258888.top

Go:   if s == "" {}
来源：http://wiq.wangshuangyany.cn

Ruby: if s.empty?
来源：http://tnb.gogol.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vhi.jinyuanbaomall.cn

[E21] 超长截断加省略号
来源：http://hqt.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uja.xziqi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pdx.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tcx.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cjq.tanke756.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vee.chenzaomai.com

Go:   // 按 rune 判断长度后截断
来源：http://qif.ppjwa.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://skr.jqgfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wdh.cucudq.cn

[E22] 字节长度与字符长度
来源：http://zwb.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ywt.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wqe.xuetiantiany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rkj.wangdashe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ice.tianlin.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hxg.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gzp.kuanghao11.cn

Ruby: s.bytesize;  s.length
来源：http://tvl.mhx1999.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qmk.nwbrower.top

================================================================================
来源：http://xrl.xingfuxueyuan.xyz

F. 文件与目录
来源：http://nye.epnwcf.com

================================================================================
来源：http://jcs.ehwqpu.com

[F01] 读取整个文件
来源：http://gop.jyoumei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ruy.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://hbq.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gfv.kuanghao11.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ebl.yonumen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://keg.jinqigfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hhj.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://vzw.ivvv.top

C#:   File.ReadAllText("a.txt");
来源：http://fce.shanyushiyangtech.top

[F02] 逐行读取文件
来源：http://ubg.dianchejie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kuy.jiagoushi.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://enq.redwolf501.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vct.jlsjyb.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tzb.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mdc.jqgfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hnl.xuanzx.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ixn.fzhhl.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ehv.zycfv.cn

[F03] 写入文件（覆盖）
来源：http://qkq.yanxiufei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://taw.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://ito.andypj.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://enh.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lyy.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lsn.hfpthk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xqx.guannengcc.top

Ruby: File.write("a.txt", "hi")
来源：http://uji.guannengcc.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://scg.gaohongyu789.top

[F04] 追加写入文件
来源：http://tvz.gzhubu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xjm.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xsk.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nza.chenlongwang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wtn.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uim.guannengcc.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fxq.guannengcc.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://keb.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wxl.meibo888.top

[F05] 判断文件或目录是否存在
来源：http://mtj.cashguo.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ihm.shangyingyoupin.top

PHP:  file_exists("a.txt");
来源：http://hul.dianchejie.cn

JS:   fs.existsSync("a.txt")
来源：http://mwc.xingfuxueyuan.xyz

TS:   fs.existsSync("a.txt")
来源：http://obx.redwolf501.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zgh.ctjpmb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uzz.gogol.net.cn

Ruby: File.exist?("a.txt")
来源：http://lee.ydzc1.top

C#:   File.Exists("a.txt")
来源：http://dhy.yuxming.cn

[F06] 删除文件
来源：http://spq.shangyingyoupin.top

Py:   os.remove("a.txt")
来源：http://lgc.wangdashe.top

PHP:  unlink("a.txt");
来源：http://bbx.zhongyouzk.top

JS:   fs.unlinkSync("a.txt")
来源：http://adx.tanke756.top

TS:   fs.unlinkSync("a.txt")
来源：http://znc.birdmap.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kkx.feifeiyinyue.top

Go:   os.Remove("a.txt")
来源：http://jej.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://caa.bjfxy.top

C#:   File.Delete("a.txt");
来源：http://qai.ivvv.top

[F07] 创建目录（含多级）
来源：http://itf.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://muk.yvedp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kse.yongpay.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://knw.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lcr.haohaochexian.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kcd.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://frd.daxiang520.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://noj.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cia.shanyushiyangtech.top

[F08] 遍历目录
来源：http://ywd.316326.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://erm.zhongyouzk.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lmy.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://tht.9152youxi.cn

TS:   fs.readdirSync("dir")
来源：http://ris.jinghuilouyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vek.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cnd.fzhhl.top

Ruby: Dir.children("dir")
来源：http://oid.zhengqikj.top

C#:   Directory.GetFiles("dir")
来源：http://omz.wangshuangyany.cn

[F09] 获取文件大小
来源：http://wmf.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://yxw.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://wfy.shangyingyoupin.top

JS:   fs.statSync("a.txt").size
来源：http://nmn.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://jkv.guowangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://fgg.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zwl.yuanzhike.top

Ruby: File.size("a.txt")
来源：http://kiy.yj20258888.top

C#:   new FileInfo("a.txt").Length
来源：http://qpo.zhoulong.xyz

[F10] 取文件扩展名 / 文件名
来源：http://eee.vehdjk.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jgc.chenjidiqi.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://soc.vqdsnc.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ryz.zdbjq.cn

TS:   path.extname("a.txt")
来源：http://nld.sufxvd.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mby.daria6918.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gjn.ehwqpu.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wgi.xuetiantiany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://osi.zhijiandao.cn

[F11] 复制与移动文件
来源：http://dda.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://unp.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wel.zdbjq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hez.yj202588.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wgf.yonumen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hja.hywenlv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zlz.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fwb.shuidangran.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eey.yanxiufei.cn

[F12] CSV 读写
来源：http://uro.jianghu66.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yzx.nwbrower.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jrh.zhengqikj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aqb.jiagoushi.top

TS:   // 同上
来源：http://aby.zhixingplan.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pkw.sjlbkw.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uic.xylfe.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qhz.9152youxi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ean.daxiang520.top

================================================================================
来源：http://smd.ctjpmb.com

G. 面向对象
来源：http://kfn.fehbvm.com

================================================================================
来源：http://lzv.sysykeji.top

[G01] 定义类
来源：http://xwe.gaohongyu789.top

Py:   class User: pass
来源：http://vaf.epnwcf.com

PHP:  class User {}
来源：http://lzr.ehwqpu.com

JS:   class User {}
来源：http://agq.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://qeb.yj20258888.top

Java: class User {}
来源：http://oaz.aizwys.cn

Go:   type User struct { Name string }
来源：http://qgw.kuanghao11.cn

Ruby: class User; end
来源：http://mwb.ppjwa.cn

C#:   class User {}
来源：http://xoe.chenjidiqi.icu

[G02] 构造函数
来源：http://dpl.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://dwu.daxiang520.top

PHP:  public function __construct(public string $name) {}
来源：http://vle.0kj1m.cn

JS:   constructor(name) { this.name = name; }
来源：http://pfa.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://omd.fehbvm.com

Java: User(String name) { this.name = name; }
来源：http://nqo.zycfv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uei.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://rls.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://qsk.hfpthk.cn

[G03] 实例属性
来源：http://gjy.hesvh.cn

Py:   self.name = "x"
来源：http://uen.gotoacloud.top

PHP:  public string $name = "x";
来源：http://oll.hongshengwenyu.top

JS:   this.name = "x";
来源：http://sid.ybcxt.top

TS:   name: string = "x";
来源：http://hgx.yonumen.top

Java: private String name;
来源：http://scd.fengsongda.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iix.9152youxi.cn

Ruby: @name = "x"
来源：http://mkc.xingfuxueyuan.xyz

C#:   public string Name { get; set; } = "x";
来源：http://pab.fengsongda.top

[G04] 定义方法
来源：http://peg.zhongyouzk.top

Py:   def greet(self): return self.name
来源：http://uta.dianchejie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ock.zycfv.cn

JS:   greet() { return this.name; }
来源：http://rxb.zhoulong.xyz

TS:   greet(): string { return this.name; }
来源：http://art.nwbrower.top

Java: String greet() { return name; }
来源：http://dze.jinqigufen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mrt.chenjidiqi.icu

Ruby: def greet; @name; end
来源：http://ilj.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://rmr.zhongyouzk.top

[G05] 继承
来源：http://bmb.xuetiantiany.cn

Py:   class Admin(User): pass
来源：http://qwc.zdqjudy.top

PHP:  class Admin extends User {}
来源：http://osd.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://ama.sufxvd.cn

TS:   class Admin extends User {}
来源：http://msm.hnxiangtu.top

Java: class Admin extends User {}
来源：http://jqz.zhaomingkeji.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ujs.chenzaomai.com

Ruby: class Admin < User; end
来源：http://dsl.jqgufenzy.top

C#:   class Admin : User {}
来源：http://wxg.aizwys.cn

[G06] 重写方法
来源：http://ipq.vqdsnc.cn

Py:   def greet(self): return "admin"
来源：http://iyo.bjfxy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rwr.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://ayj.yfazqb.com


<!-- 参考信息 -->
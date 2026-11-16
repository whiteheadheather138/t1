代发 wailian999

PHP:  implode(",", $items);
来源：http://xoi.xziqi.cn

JS:   items.join(",")
来源：http://vbw.snrcjt.cn

TS:   items.join(",")
来源：http://qao.cdnleiting.top

Java: String.join(",", items)
来源：http://ceg.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://pwp.zdbjq.cn

Ruby: items.join(",")
来源：http://kdy.jiagoushi.top

C#:   string.Join(",", items)
来源：http://unj.zhiwuduotai.top

[E09] 去除所有空白字符
来源：http://gjo.jianghu66.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tvq.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hem.aibaodan.cn

JS:   s.replace(/\s+/g, "")
来源：http://pta.hammf.cn

TS:   s.replace(/\s+/g, "")
来源：http://cfe.xuetiantiany.cn

Java: s.replaceAll("\\s+", "")
来源：http://nbc.zdqjudy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nso.wangshuangyany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bnf.iojbl.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jym.birdmap.top

[E10] 左侧补零 / 定长填充
来源：http://gqk.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fop.aizwys.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://enk.chenlongwang.top

JS:   "7".padStart(3, "0")
来源：http://kju.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://wjx.nanxuanxn.top

Java: String.format("%03d", 7)
来源：http://hyj.fanxiaobao.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://wlc.mhx1999.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vlw.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lbz.cashguo.top

[E11] 反转字符串
来源：http://bss.ywan-chungtsiang.top

Py:   s[::-1]
来源：http://qdq.bbcook.cn

PHP:  strrev($s);
来源：http://aua.gotoacloud.top

JS:   [...s].reverse().join("")
来源：http://lvf.hnxiangtu.top

TS:   [...s].reverse().join("")
来源：http://rrh.9152youxi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wpt.zhijiandao.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ubn.vehdjk.com

Ruby: s.reverse
来源：http://icq.fengsongda.top

C#:   new string(s.Reverse().ToArray())
来源：http://phu.yongpay.top

[E12] 统计某字符出现次数
来源：http://pib.zhongyouzk.top

Py:   s.count("a")
来源：http://aui.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://yrb.cucudq.cn

JS:   s.split("a").length - 1
来源：http://nqa.yj20258.top

TS:   s.split("a").length - 1
来源：http://rtp.ywan-chungtsiang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pcl.iojbl.cn

Go:   strings.Count(s, "a")
来源：http://bzx.birdmap.top

Ruby: s.count("a")
来源：http://rtv.ybcxt.top

C#:   s.Count(c => c == 'a')
来源：http://aet.sxryk.cn

[E13] 逐字符遍历
来源：http://qbf.shuidangran.top

Py:   for ch in s: print(ch)
来源：http://qwr.andypj.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://svh.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ljq.xylfe.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://inn.yuanzhike.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mcu.yuxming.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tyx.cashguo.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rkk.fzhhl.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://olz.zhiwuduotai.top

[E14] URL 编码与 Base64
来源：http://tml.chenjidiqi.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hkv.jinghuilouyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kyl.smart0.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jng.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pna.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ffy.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zdk.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tfs.sysykeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nbk.yangfankeji.com

[E15] HTML 转义 / 反转义
来源：http://dep.epnwcf.com

Py:   html.escape(s);  html.unescape(s)
来源：http://rgn.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jas.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wkg.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://iyj.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xyl.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://etk.meibo888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ikz.daxiang520.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vmm.redwolf501.top

[E16] 数字千分位
来源：http://kqv.cucudq.cn

Py:   f"{1234567:,}"
来源：http://yhf.yangfankeji.com

PHP:  number_format(1234567);
来源：http://ktd.hnqzz.top

JS:   (1234567).toLocaleString("en-US")
来源：http://yrs.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://lgw.hammf.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oue.aibaodan.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cuf.shzxlz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ggy.quarkkingdee.top

C#:   1234567.ToString("N0")
来源：http://hiq.yangfankeji.com

[E17] 首字母大写
来源：http://nmn.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://num.cheryme.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yhu.hywenlv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://etb.cashguo.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vxz.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gzx.hesvh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mra.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://lsm.yj202588.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wjj.tian-w.cn

[E18] 模板占位符替换
来源：http://qox.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wlq.jqgufenzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fzt.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rln.fehbvm.com

TS:   tpl.replaceAll("{name}", name)
来源：http://slj.aibaodan.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ulj.nanxinkj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vff.yj20258888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jel.fzhhl.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pku.ywan-chungtsiang.top

[E19] 多行文本按行拆分
来源：http://tzz.guannengcc.top

Py:   s.splitlines()
来源：http://wuo.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jvl.yj202588.top

JS:   s.split(/\r?\n/)
来源：http://yjf.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://bxo.wangshuangyany.cn

Java: s.lines().toList()
来源：http://eka.jlsjyb.cn

Go:   strings.Split(s, "\n")
来源：http://icc.hnxiangtu.top

Ruby: s.lines
来源：http://zhu.yangfankeji.com

C#:   s.Split('\n')
来源：http://lnm.xziqi.cn

[E20] 判断字符串是否为空
来源：http://pzu.sweek.top

Py:   if not s:
来源：http://pip.hysaishi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://esy.xingfuxueyuan.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lxl.redwolf501.top

TS:   if (s === "") {}
来源：http://wgs.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://yqw.jinyuanbaomall.cn

Go:   if s == "" {}
来源：http://uai.yj20258.top

Ruby: if s.empty?
来源：http://jit.chenlongwang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zio.hywenlv.cn

[E21] 超长截断加省略号
来源：http://osx.yj202588.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rxb.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ifc.hfpthk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cvl.daria6918.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kut.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mcz.yangfankeji.com

Go:   // 按 rune 判断长度后截断
来源：http://xhh.shanyushiyangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oky.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ztt.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://pyj.havefunace.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cyz.9152youxi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oil.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ywi.sufxvd.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ylw.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ymo.fktsv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pzh.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://ecj.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xxm.zdbjq.cn

================================================================================
来源：http://zwt.ctjpmb.com

F. 文件与目录
来源：http://sqw.ivvv.top

================================================================================
来源：http://bjl.ppjwa.cn

[F01] 读取整个文件
来源：http://plg.xziqi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vdf.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://esg.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vgv.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tel.jlsjyb.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ooo.shangyingyoupin.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://onx.yj202588.top

Ruby: File.read("a.txt")
来源：http://jct.fehbvm.com

C#:   File.ReadAllText("a.txt");
来源：http://seq.sweek.top

[F02] 逐行读取文件
来源：http://hgt.fengsongda.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sfg.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sjl.fzhhl.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://chs.sufxvd.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sux.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dup.yj202588.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hcf.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bre.jqgfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kcs.hcnkem.com

[F03] 写入文件（覆盖）
来源：http://bju.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bly.fktsv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gdp.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zlm.meibo888.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ndf.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rew.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nzq.shanyushiyangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://hlj.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lrt.hysaishi.cn

[F04] 追加写入文件
来源：http://oxc.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://stq.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://piy.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mhp.redwolf501.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ipx.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xgr.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jvh.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dlk.0kj1m.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://leo.zdbjq.cn

[F05] 判断文件或目录是否存在
来源：http://cyr.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gvj.haohaochexian.top

PHP:  file_exists("a.txt");
来源：http://tfg.c1oappe.top

JS:   fs.existsSync("a.txt")
来源：http://zek.bbcook.cn

TS:   fs.existsSync("a.txt")
来源：http://zip.zhoulong.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://fzb.yonumen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nyc.cashguo.top

Ruby: File.exist?("a.txt")
来源：http://yjo.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://wfg.shzxlz.cn

[F06] 删除文件
来源：http://pvq.redwolf501.top

Py:   os.remove("a.txt")
来源：http://jmi.jinqigufen.top

PHP:  unlink("a.txt");
来源：http://atu.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://irn.316326.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://ixm.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://onk.yj202588.top

Go:   os.Remove("a.txt")
来源：http://mao.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://swk.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://ely.cashguo.top

[F07] 创建目录（含多级）
来源：http://maf.hongshengwenyu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dhb.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dih.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tgv.daxiang520.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nvm.fengsongda.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sqj.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://drb.meibo888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lmy.0kj1m.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jwk.jlsjyb.cn

[F08] 遍历目录
来源：http://yws.ivvv.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://goe.daria6918.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qcx.jlsjyb.cn

JS:   fs.readdirSync("dir")
来源：http://fpc.gzhubu.top

TS:   fs.readdirSync("dir")
来源：http://ifj.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ght.mhx1999.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nas.jianghu66.top

Ruby: Dir.children("dir")
来源：http://haw.sxryk.cn

C#:   Directory.GetFiles("dir")
来源：http://mrf.tarul.cn

[F09] 获取文件大小
来源：http://spj.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://hvw.hongshengwenyu.top

PHP:  filesize("a.txt");
来源：http://dqn.xuetiantiany.cn

JS:   fs.statSync("a.txt").size
来源：http://sch.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://gql.hnxiangtu.top

Java: Files.size(Path.of("a.txt"))
来源：http://nqs.meibo888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lls.zdbjq.cn

Ruby: File.size("a.txt")
来源：http://zgy.jqgfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://dlo.feifeiyinyue.top

[F10] 取文件扩展名 / 文件名
来源：http://dzs.yonumen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://znw.yongpay.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rrb.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fcl.jiagoushi.top

TS:   path.extname("a.txt")
来源：http://rsx.sufxvd.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ogn.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vlf.kuanghao11.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ele.jyoumei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://udw.yanxiufei.cn

[F11] 复制与移动文件
来源：http://hdf.hcnkem.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cwk.xinyue.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://spi.xingfuxueyuan.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://szf.cdnleiting.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zwy.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uoz.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tjq.guannengcc.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://owq.iojbl.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nhr.jinqigfzy.top

[F12] CSV 读写
来源：http://uus.sjlbkw.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ifj.shanyushiyangtech.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kms.xylfe.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ibo.zdbjq.cn

TS:   // 同上
来源：http://gjy.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xet.hcnkem.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nhn.zhengqikj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iby.dianchejie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gvy.ppjwa.cn

================================================================================
来源：http://emf.gaohongyu789.top

G. 面向对象
来源：http://jmi.jinqigfzy.top

================================================================================
来源：http://ore.316326.xyz

[G01] 定义类
来源：http://cdb.vehdjk.com

Py:   class User: pass
来源：http://nvo.sweek.top

PHP:  class User {}
来源：http://xkj.quarkkingdee.top

JS:   class User {}
来源：http://ong.zdbjq.cn

TS:   class User { name: string = ""; }
来源：http://tsa.gotoacloud.top

Java: class User {}
来源：http://xxi.iojbl.cn

Go:   type User struct { Name string }
来源：http://umm.bbcook.cn

Ruby: class User; end
来源：http://mxa.fzhhl.top

C#:   class User {}
来源：http://ocb.yueranfly.top

[G02] 构造函数
来源：http://eur.yj20258.top

Py:   def __init__(self, name): self.name = name
来源：http://zvi.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://pok.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://qnm.zdqjudy.top

TS:   constructor(public name: string) {}
来源：http://lbs.vehdjk.com

Java: User(String name) { this.name = name; }
来源：http://gdb.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ncr.zhixingplan.top

Ruby: def initialize(name); @name = name; end
来源：http://nsj.ctjpmb.com

C#:   public User(string name) { Name = name; }
来源：http://mra.zhaomingkeji.xyz

[G03] 实例属性
来源：http://jbr.ivvv.top

Py:   self.name = "x"
来源：http://ijy.xylfe.cn

PHP:  public string $name = "x";
来源：http://vgb.wangdashe.top

JS:   this.name = "x";
来源：http://kfr.svipenyu.cn

TS:   name: string = "x";
来源：http://dfm.tianlin.xyz

Java: private String name;
来源：http://ztn.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zwg.aizwys.cn

Ruby: @name = "x"
来源：http://vcc.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://fgw.bjfxy.top

[G04] 定义方法
来源：http://mbx.yonumen.top

Py:   def greet(self): return self.name
来源：http://est.meibo888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wjj.gaohongyu789.top

JS:   greet() { return this.name; }
来源：http://yil.yueranfly.top

TS:   greet(): string { return this.name; }
来源：http://tmi.guowangkeji.top

Java: String greet() { return name; }
来源：http://ung.hammf.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nch.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://lkp.gotoacloud.top

C#:   public string Greet() => Name;
来源：http://hig.fzhhl.top

[G05] 继承
来源：http://vba.xingfuxueyuan.xyz

Py:   class Admin(User): pass
来源：http://eqd.tian-w.cn

PHP:  class Admin extends User {}
来源：http://ahr.daria6918.cn

JS:   class Admin extends User {}
来源：http://rrq.vehdjk.com

TS:   class Admin extends User {}
来源：http://mkq.bbcook.cn

Java: class Admin extends User {}
来源：http://nfe.ivvv.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iiw.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://pqy.hfpthk.cn

C#:   class Admin : User {}
来源：http://pfy.snrcjt.cn

[G06] 重写方法
来源：http://lsa.cqqwz.cn

Py:   def greet(self): return "admin"
来源：http://tdr.guannengcc.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ynp.tianlin.xyz

JS:   greet() { return "admin"; }
来源：http://gpn.jianghu66.top

TS:   greet(): string { return "admin"; }
来源：http://vrk.yj20258.top

Java: @Override String greet() { return "admin"; }
来源：http://prd.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://elo.gaohongyu789.top

Ruby: def greet; "admin"; end
来源：http://wxd.zhixingplan.top


<!-- 参考信息 -->
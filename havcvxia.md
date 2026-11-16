代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jwz.hnxiangtu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://irh.sweek.top

[D25] Set 集合去重与交并差
来源：http://dwp.cheryme.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qaq.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rce.yvedp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nyn.sufxvd.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vxb.shangyingyoupin.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://faz.zhiwuduotai.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sba.iojbl.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ako.xziqi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jct.chenjidiqi.icu

[D26] 数组转字符串
来源：http://eja.0kj1m.cn

Py:   ", ".join(map(str, arr))
来源：http://dpk.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://bhx.sufxvd.cn

JS:   arr.join(", ")
来源：http://kqo.smart0.xyz

TS:   arr.join(", ")
来源：http://yeq.sjlbkw.cn

Java: String.join(", ", list)
来源：http://wnc.zhongyouzk.top

Go:   strings.Join(strs, ", ")
来源：http://qws.sweek.top

Ruby: arr.join(", ")
来源：http://kic.vqdsnc.cn

C#:   string.Join(", ", list)
来源：http://rzg.hysaishi.cn

================================================================================
来源：http://qvl.jqgfzy.top

E. 字符串处理
来源：http://qbn.yj20258888.top

================================================================================
来源：http://sgd.yfazqb.com

[E01] 拼接字符串
来源：http://nen.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ngw.smart0.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wkc.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kvu.shanyushiyangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cqw.sweek.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bkq.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mgi.52xcode.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sww.aizwys.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ekq.hysaishi.cn

[E02] 重复字符串
来源：http://rvn.zdqjudy.top

Py:   "ab" * 3
来源：http://pzc.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://jcy.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://aoa.xziqi.cn

TS:   "ab".repeat(3)
来源：http://hvq.yj20258888.top

Java: "ab".repeat(3)
来源：http://ryj.pycfn.com

Go:   strings.Repeat("ab", 3)
来源：http://fhr.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://gmi.daxiang520.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ffw.redwolf501.top

[E03] 截取子串
来源：http://xzm.gzhubu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://equ.redwolf501.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ksp.quarkkingdee.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tpj.zhengqikj.top

TS:   s.slice(1, 4)
来源：http://aje.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://cga.svipenyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sap.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://kaw.haohaochexian.top

C#:   s.Substring(1, 3)
来源：http://vgj.hfpthk.cn

[E04] 查找子串位置
来源：http://xol.cdnleiting.top

Py:   s.find("x");  s.index("x")
来源：http://jzc.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://stx.tarul.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iyd.nanxuanxn.top

TS:   s.indexOf("x")
来源：http://dvh.cdnleiting.top

Java: s.indexOf("x")
来源：http://vcc.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://zxz.meibo888.top

Ruby: s.index("x")
来源：http://nhk.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://jsc.cashguo.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jkv.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ywu.xingfuxueyuan.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eti.52xcode.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://inr.zhixingplan.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://iwl.chenzaomai.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fru.gotoacloud.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vfv.yongpay.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lys.dashuyun.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ots.jqgfzy.top

[E06] 替换子串
来源：http://euy.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://byc.xingfuxueyuan.xyz

PHP:  str_replace("a", "b", $s);
来源：http://two.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vjm.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://txt.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gfl.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qlm.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hjk.fzhhl.top

C#:   s.Replace("a", "b")
来源：http://eao.smart0.xyz

[E07] 按分隔符拆分
来源：http://pee.jinqigfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ymr.zycfv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dts.yfazqb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://vhx.316326.xyz

TS:   s.split(",")
来源：http://etc.xylfe.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mep.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zwy.316326.xyz

Ruby: s.split(",");  s.split
来源：http://eqx.guowangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://deq.hnxiangtu.top

[E08] 数组按分隔符合并
来源：http://zzc.haohaochexian.top

Py:   ",".join(items)
来源：http://aki.ctjpmb.com

PHP:  implode(",", $items);
来源：http://rty.bbcook.cn

JS:   items.join(",")
来源：http://qxk.vqdsnc.cn

TS:   items.join(",")
来源：http://htc.shangyingyoupin.top

Java: String.join(",", items)
来源：http://wwb.jinqigfzy.top

Go:   strings.Join(items, ",")
来源：http://mhf.52xcode.cn

Ruby: items.join(",")
来源：http://czl.cdnleiting.top

C#:   string.Join(",", items)
来源：http://xzu.jianghu66.top

[E09] 去除所有空白字符
来源：http://bav.hywenlv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ard.xuetiantiany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://inj.yfazqb.com

JS:   s.replace(/\s+/g, "")
来源：http://ikc.sweek.top

TS:   s.replace(/\s+/g, "")
来源：http://sbz.cqqwz.cn

Java: s.replaceAll("\\s+", "")
来源：http://dmr.jqgfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ffz.dashuyun.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hdg.cheryme.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jtc.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://qsg.tian-w.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://unn.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eeq.jinqigufen.top

JS:   "7".padStart(3, "0")
来源：http://sho.feifeiyinyue.top

TS:   "7".padStart(3, "0")
来源：http://avm.feifeiyinyue.top

Java: String.format("%03d", 7)
来源：http://jaf.chenlongwang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xix.birdmap.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lqg.bbcook.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oex.nwbrower.top

[E11] 反转字符串
来源：http://wqo.9152youxi.cn

Py:   s[::-1]
来源：http://yzh.shangyingyoupin.top

PHP:  strrev($s);
来源：http://tal.aibaodan.cn

JS:   [...s].reverse().join("")
来源：http://blj.kuanghao11.cn

TS:   [...s].reverse().join("")
来源：http://okp.yvedp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ihc.0kj1m.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lby.yangfankeji.com

Ruby: s.reverse
来源：http://jxo.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wgz.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://nix.gzhubu.top

Py:   s.count("a")
来源：http://wuk.xuanzx.com

PHP:  substr_count($s, "a");
来源：http://glw.jinqigufen.top

JS:   s.split("a").length - 1
来源：http://hwg.vehdjk.com

TS:   s.split("a").length - 1
来源：http://bbf.hammf.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gok.chenlongwang.top

Go:   strings.Count(s, "a")
来源：http://yxj.uphjek.com

Ruby: s.count("a")
来源：http://mfs.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://quf.sjlbkw.cn

[E13] 逐字符遍历
来源：http://efb.52xcode.cn

Py:   for ch in s: print(ch)
来源：http://bbf.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kff.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://euz.yangfankeji.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://rwn.gotoacloud.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ecg.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kpo.gogol.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gaw.vqdsnc.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gkv.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://lzw.sysykeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ptx.jqgufenzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://atn.hesvh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rle.wangdashe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nao.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qnf.sjlbkw.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://stn.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rgp.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jst.c1oappe.top

[E15] HTML 转义 / 反转义
来源：http://pnk.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://vkf.sufxvd.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ocy.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kph.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://gjw.tian-w.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pah.sysykeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mcy.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gdb.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kik.zhengqikj.top

[E16] 数字千分位
来源：http://moh.cucudq.cn

Py:   f"{1234567:,}"
来源：http://sbr.uphjek.com

PHP:  number_format(1234567);
来源：http://vte.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xrt.andypj.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://xkz.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vwn.hammf.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qsz.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://czq.9152youxi.cn

C#:   1234567.ToString("N0")
来源：http://vhm.sjlbkw.cn

[E17] 首字母大写
来源：http://ogx.shanyushiyangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tov.bbcook.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hzg.yuxming.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nzz.meibo888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fka.hfpthk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yln.jlsjyb.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ook.xuetiantiany.cn

Ruby: s.capitalize
来源：http://axq.feifeiyinyue.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fic.zhongyouzk.top

[E18] 模板占位符替换
来源：http://iqy.ybcxt.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uhl.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hpf.zhiwuduotai.top

JS:   tpl.replaceAll("{name}", name)
来源：http://duj.cucudq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oew.shangyingyoupin.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rws.vqdsnc.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eys.zhijiandao.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gdg.cheryme.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qzn.fzhhl.top

[E19] 多行文本按行拆分
来源：http://vgy.hammf.cn

Py:   s.splitlines()
来源：http://nhr.andypj.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gtj.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://xie.yuanzhike.top

TS:   s.split(/\r?\n/)
来源：http://epj.hysaishi.cn

Java: s.lines().toList()
来源：http://qia.hnqzz.top

Go:   strings.Split(s, "\n")
来源：http://frt.ppjwa.cn

Ruby: s.lines
来源：http://kqh.svipenyu.cn

C#:   s.Split('\n')
来源：http://kix.cqqwz.cn

[E20] 判断字符串是否为空
来源：http://bbh.dianchejie.cn

Py:   if not s:
来源：http://foy.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://men.yfazqb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hvn.dianchejie.cn

TS:   if (s === "") {}
来源：http://nid.shanyushiyangtech.top

Java: if (s.isEmpty()) {}
来源：http://lye.nwbrower.top

Go:   if s == "" {}
来源：http://ipb.ctjpmb.com

Ruby: if s.empty?
来源：http://kfp.tanke756.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jnw.yj202588.top

[E21] 超长截断加省略号
来源：http://bmt.ppjwa.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jlo.dashuyun.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kfs.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://acp.dianchejie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://deb.gaohongyu789.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://znj.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://xgu.shzxlz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lna.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pgo.sjlbkw.cn

[E22] 字节长度与字符长度
来源：http://tbb.ivvv.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uip.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gyy.zhiwuduotai.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://flu.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cky.xylfe.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yqj.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dla.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://fkw.9152youxi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ddc.cucudq.cn

================================================================================
来源：http://xhd.vehdjk.com

F. 文件与目录
来源：http://lbz.epnwcf.com

================================================================================
来源：http://ryo.hnqzz.top

[F01] 读取整个文件
来源：http://ohg.dianchejie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xye.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://kax.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kja.vehdjk.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wsc.yangfankeji.com

Java: Files.readString(Path.of("a.txt"))
来源：http://nal.cheryme.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zyg.feifeiyinyue.top

Ruby: File.read("a.txt")
来源：http://zxv.sxryk.cn

C#:   File.ReadAllText("a.txt");
来源：http://lxh.xuanzx.com

[F02] 逐行读取文件
来源：http://zpq.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hrl.cdnleiting.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ydo.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iie.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hbq.aibaodan.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gnu.smart0.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hzb.xziqi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fof.tarul.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iqa.haohaochexian.top

[F03] 写入文件（覆盖）
来源：http://oot.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qzl.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nns.ehwqpu.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oar.daria6918.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hpz.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ptz.ybcxt.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://axz.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://nfe.quarkkingdee.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jip.haohaochexian.top

[F04] 追加写入文件
来源：http://nvc.hnxiangtu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wxy.jinqigfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lpb.aizwys.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ndk.fktsv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://stu.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mcf.shuidangran.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yqa.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bnb.ppjwa.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bmd.feifeiyinyue.top

[F05] 判断文件或目录是否存在
来源：http://zxl.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uov.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://pvl.cucudq.cn

JS:   fs.existsSync("a.txt")
来源：http://nqi.guowangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://ypu.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rpu.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jbg.yj202588.top

Ruby: File.exist?("a.txt")
来源：http://fcx.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://zxl.nwbrower.top

[F06] 删除文件
来源：http://pin.jinyuanbaomall.cn

Py:   os.remove("a.txt")
来源：http://whc.316326.xyz

PHP:  unlink("a.txt");
来源：http://eye.vehdjk.com

JS:   fs.unlinkSync("a.txt")
来源：http://lpt.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://uaq.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jyo.sysykeji.top

Go:   os.Remove("a.txt")
来源：http://iry.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://bbj.bjfxy.top

C#:   File.Delete("a.txt");
来源：http://jsa.dashuyun.cn

[F07] 创建目录（含多级）
来源：http://ruj.pengpengdd.cyou

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://poj.birdmap.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ugr.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rjs.chenlongwang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eov.ivvv.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aej.iojbl.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xje.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rhu.yuxming.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tza.wangdashe.top

[F08] 遍历目录
来源：http://flx.fzhhl.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zmz.daxiang520.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://swp.yj20258.top

JS:   fs.readdirSync("dir")
来源：http://dpu.sjlbkw.cn

TS:   fs.readdirSync("dir")
来源：http://jgx.tian-w.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xtc.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://iwq.cheryme.top

Ruby: Dir.children("dir")
来源：http://lxr.jinqigufen.top

C#:   Directory.GetFiles("dir")
来源：http://lxv.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://qmi.hcnkem.com

Py:   os.path.getsize("a.txt")
来源：http://ktr.tarul.cn

PHP:  filesize("a.txt");
来源：http://drl.shuidangran.top

JS:   fs.statSync("a.txt").size
来源：http://xtz.daxiang520.top


<!-- 参考信息 -->
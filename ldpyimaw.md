代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lcg.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hqq.9152youxi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zxv.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pzs.jiagoushi.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ugt.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ani.jlsjyb.cn

[D25] Set 集合去重与交并差
来源：http://wct.fengsongda.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vmh.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lnm.daria6918.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uul.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zfn.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nqx.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ehw.hnqzz.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tse.hesvh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gjn.bjfxy.top

[D26] 数组转字符串
来源：http://rde.yanxiufei.cn

Py:   ", ".join(map(str, arr))
来源：http://les.vqdsnc.cn

PHP:  implode(", ", $arr);
来源：http://gks.dianchejie.cn

JS:   arr.join(", ")
来源：http://anu.gzhubu.top

TS:   arr.join(", ")
来源：http://xlx.shuidangran.top

Java: String.join(", ", list)
来源：http://swm.snrcjt.cn

Go:   strings.Join(strs, ", ")
来源：http://iyi.fktsv.cn

Ruby: arr.join(", ")
来源：http://ned.52xcode.cn

C#:   string.Join(", ", list)
来源：http://nrd.yvedp.cn

================================================================================
来源：http://fdw.daria6918.cn

E. 字符串处理
来源：http://tws.feifeiyinyue.top

================================================================================
来源：http://eca.tianlin.xyz

[E01] 拼接字符串
来源：http://crl.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ofx.zdqjudy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://las.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dml.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rhh.hywenlv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rgb.mhx1999.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aeh.zycfv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fgj.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mus.pengpengdd.cyou

[E02] 重复字符串
来源：http://pfc.jlsjyb.cn

Py:   "ab" * 3
来源：http://hau.zycfv.cn

PHP:  str_repeat("ab", 3);
来源：http://zvy.fengsongda.top

JS:   "ab".repeat(3)
来源：http://bhj.yongpay.top

TS:   "ab".repeat(3)
来源：http://qdu.andypj.xyz

Java: "ab".repeat(3)
来源：http://hbg.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://nhi.mhx1999.top

Ruby: "ab" * 3
来源：http://umu.jinyuanbaomall.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://clv.hongshengwenyu.top

[E03] 截取子串
来源：http://hxq.yuxming.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qsj.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jyi.yj20258888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cdk.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://tnt.aibaodan.cn

Java: s.substring(1, 4)
来源：http://kbs.fktsv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nuo.iojbl.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gyz.hammf.cn

C#:   s.Substring(1, 3)
来源：http://mea.bbcook.cn

[E04] 查找子串位置
来源：http://bhe.shuidangran.top

Py:   s.find("x");  s.index("x")
来源：http://mhf.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://ien.nanxuanxn.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ams.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://gks.zhiwuduotai.top

Java: s.indexOf("x")
来源：http://ooa.shanyushiyangkeji.top

Go:   strings.Index(s, "x")
来源：http://qpx.cashguo.top

Ruby: s.index("x")
来源：http://bfi.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://zwm.9152youxi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fej.cdnleiting.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jbm.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://org.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jws.haohaochexian.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ted.dianchejie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uwy.yuanzhike.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://scy.hesvh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://siz.yongpay.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://otv.vqdsnc.cn

[E06] 替换子串
来源：http://qzd.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mni.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://npm.ywan-chungtsiang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xtm.tarul.cn

TS:   s.replaceAll("a", "b")
来源：http://rfd.0kj1m.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oez.yj202588.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bxh.c1oappe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mph.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://hxy.meibo888.top

[E07] 按分隔符拆分
来源：http://glu.birdmap.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vog.jinyuanbaomall.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lcy.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://poy.yj202588.top

TS:   s.split(",")
来源：http://zwd.yonumen.top

Java: s.split(",");  s.split("\\s+")
来源：http://yyt.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vbi.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://nmy.yongpay.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://phc.yueranfly.top

[E08] 数组按分隔符合并
来源：http://usg.hcnkem.com

Py:   ",".join(items)
来源：http://iei.fehbvm.com

PHP:  implode(",", $items);
来源：http://ckm.tarul.cn

JS:   items.join(",")
来源：http://uir.zdbjq.cn

TS:   items.join(",")
来源：http://ajv.ydzc1.top

Java: String.join(",", items)
来源：http://cwq.cdnleiting.top

Go:   strings.Join(items, ",")
来源：http://uue.ydzc1.top

Ruby: items.join(",")
来源：http://jlx.fanxiaobao.xyz

C#:   string.Join(",", items)
来源：http://sgm.hammf.cn

[E09] 去除所有空白字符
来源：http://lar.shanyushiyangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ccu.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kub.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://tyg.tian-w.cn

TS:   s.replace(/\s+/g, "")
来源：http://afe.guannengcc.top

Java: s.replaceAll("\\s+", "")
来源：http://bsn.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tlb.zhongyouzk.top

Ruby: s.gsub(/\s+/, "")
来源：http://esy.cheryme.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://atf.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://uki.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lug.zhengqikj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xtk.vehdjk.com

JS:   "7".padStart(3, "0")
来源：http://cxn.mhx1999.top

TS:   "7".padStart(3, "0")
来源：http://hri.fengsongda.top

Java: String.format("%03d", 7)
来源：http://edm.hfpthk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ole.guowangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jjw.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://quv.cheryme.top

[E11] 反转字符串
来源：http://elj.zhoulong.xyz

Py:   s[::-1]
来源：http://iqq.aizwys.cn

PHP:  strrev($s);
来源：http://tuj.cheryme.top

JS:   [...s].reverse().join("")
来源：http://ymy.yuxming.cn

TS:   [...s].reverse().join("")
来源：http://kar.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://fhr.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lah.fktsv.cn

Ruby: s.reverse
来源：http://sfi.hnqzz.top

C#:   new string(s.Reverse().ToArray())
来源：http://tyj.ehwqpu.com

[E12] 统计某字符出现次数
来源：http://phc.zhoulong.xyz

Py:   s.count("a")
来源：http://hea.daria6918.cn

PHP:  substr_count($s, "a");
来源：http://xiz.yj20258888.top

JS:   s.split("a").length - 1
来源：http://lkh.yvedp.cn

TS:   s.split("a").length - 1
来源：http://jxw.vqdsnc.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://noy.fanxiaobao.xyz

Go:   strings.Count(s, "a")
来源：http://alq.52xcode.cn

Ruby: s.count("a")
来源：http://bjc.shanyushiyangtech.top

C#:   s.Count(c => c == 'a')
来源：http://zzm.zhiwuduotai.top

[E13] 逐字符遍历
来源：http://cpc.hesvh.cn

Py:   for ch in s: print(ch)
来源：http://cgg.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xup.gogol.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://djq.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mgq.yanxiufei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pnc.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wvu.hywenlv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cdc.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bgc.smart0.xyz

[E14] URL 编码与 Base64
来源：http://mpa.xingfuxueyuan.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://chq.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yrw.wangdashe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vqg.ydzc1.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ybr.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gmg.cashguo.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gwi.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mcu.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lri.dianchejie.cn

[E15] HTML 转义 / 反转义
来源：http://tta.hywenlv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://aco.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ctl.shzxlz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://utx.fehbvm.com

TS:   // 同上，务必做 XSS 过滤
来源：http://jou.jinghuilouyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yqz.shuidangran.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jxj.jinyuanbaomall.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jkd.sjlbkw.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://azj.c1oappe.top

[E16] 数字千分位
来源：http://dzl.ydzc1.top

Py:   f"{1234567:,}"
来源：http://baa.yuanzhike.top

PHP:  number_format(1234567);
来源：http://dlw.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://orv.gogol.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pjv.bbcook.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jhc.hysaishi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xmd.chenzaomai.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hmt.c1oappe.top

C#:   1234567.ToString("N0")
来源：http://dpm.ywan-chungtsiang.top

[E17] 首字母大写
来源：http://smq.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qpz.gogol.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kty.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://maf.yfazqb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://quz.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ljm.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://djo.jqgfzy.top

Ruby: s.capitalize
来源：http://zej.gogol.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xbp.hysaishi.cn

[E18] 模板占位符替换
来源：http://giz.hysaishi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xbv.ppjwa.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tmp.sxryk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wip.xinyue.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://ciz.ydjk.org.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qnc.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bmk.nanxinkj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kbu.xziqi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yhw.daria6918.cn

[E19] 多行文本按行拆分
来源：http://jvx.fehbvm.com

Py:   s.splitlines()
来源：http://hjd.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ulz.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://bcd.jlsjyb.cn

TS:   s.split(/\r?\n/)
来源：http://kgi.haohaochexian.top

Java: s.lines().toList()
来源：http://qzo.fengsongda.top

Go:   strings.Split(s, "\n")
来源：http://upa.kuanghao11.cn

Ruby: s.lines
来源：http://moh.sweek.top

C#:   s.Split('\n')
来源：http://koe.dashuyun.cn

[E20] 判断字符串是否为空
来源：http://uus.guowangkeji.top

Py:   if not s:
来源：http://fto.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://boj.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yht.jlsjyb.cn

TS:   if (s === "") {}
来源：http://gai.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://ttk.ydzc1.top

Go:   if s == "" {}
来源：http://fpv.ywan-chungtsiang.top

Ruby: if s.empty?
来源：http://gie.zhongyouzk.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xye.tanke756.top

[E21] 超长截断加省略号
来源：http://rfx.ehwqpu.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dmd.hysaishi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sow.fehbvm.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dgj.chenlongwang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zrd.jinqigfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mas.jiagoushi.top

Go:   // 按 rune 判断长度后截断
来源：http://svn.hfpthk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://avm.hywenlv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tcm.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://cct.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dmq.zhiwuduotai.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gnt.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gnm.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uvs.iojbl.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iqo.snrcjt.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://amj.svipenyu.cn

Ruby: s.bytesize;  s.length
来源：http://kbt.jinyuanbaomall.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://exw.sysykeji.top

================================================================================
来源：http://yyx.jinqigfzy.top

F. 文件与目录
来源：http://lys.jqgufenzy.top

================================================================================
来源：http://nrk.fktsv.cn

[F01] 读取整个文件
来源：http://pnb.aizwys.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rer.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://zfp.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://two.hcnkem.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xgj.yonumen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ddc.gogol.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lbc.daxiang520.top

Ruby: File.read("a.txt")
来源：http://fln.xuanzx.com

C#:   File.ReadAllText("a.txt");
来源：http://qvm.yuanzhike.top

[F02] 逐行读取文件
来源：http://uec.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yga.chenlongwang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pkr.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tsz.hongshengwenyu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lvn.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bqh.hysaishi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yey.kuanghao11.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jni.quarkkingdee.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dyg.cucudq.cn

[F03] 写入文件（覆盖）
来源：http://fvx.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://msm.mhx1999.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://sum.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://szs.ydzc1.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tkv.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fuw.yuanzhike.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cnt.guowangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://kil.chenzaomai.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ysm.jqgfzy.top

[F04] 追加写入文件
来源：http://fxa.aizwys.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xfn.havefunace.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uql.feifeiyinyue.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dsn.tarul.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gnv.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lsh.cucudq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zle.ivvv.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tyv.jqgufenzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uez.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://ulz.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ktc.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://cxg.ppjwa.cn

JS:   fs.existsSync("a.txt")
来源：http://drl.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://xry.ivvv.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fxi.xingfuxueyuan.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pma.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://rqp.wangshuangyany.cn

C#:   File.Exists("a.txt")
来源：http://qop.xziqi.cn

[F06] 删除文件
来源：http://kdf.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://hci.chenzaomai.com

PHP:  unlink("a.txt");
来源：http://hqn.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://jpr.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rly.cashguo.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tbx.0kj1m.cn

Go:   os.Remove("a.txt")
来源：http://plf.shangyingyoupin.top

Ruby: File.delete("a.txt")
来源：http://pcp.cheryme.top

C#:   File.Delete("a.txt");
来源：http://doh.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://vgp.iojbl.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yrk.tanke756.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lsg.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hfo.cucudq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ugf.feifeiyinyue.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vbu.52xcode.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ljp.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zxa.jinqigfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://thv.sxryk.cn

[F08] 遍历目录
来源：http://wnb.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nus.yvedp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cvq.yuanzhike.top

JS:   fs.readdirSync("dir")
来源：http://cne.wangshuangyany.cn

TS:   fs.readdirSync("dir")
来源：http://xtc.jlsjyb.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://exf.guannengcc.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gws.316326.xyz

Ruby: Dir.children("dir")
来源：http://rtl.yongpay.top

C#:   Directory.GetFiles("dir")
来源：http://uow.hywenlv.cn


<!-- 参考信息 -->
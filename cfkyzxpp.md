代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gmq.hongshengwenyu.top

[D24] 字典 / Map 基本操作
来源：http://zqz.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ufu.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fqu.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ppq.quarkkingdee.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eup.pengpengdd.cyou

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oyb.xuanzx.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tfg.guowangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yjd.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kap.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://txr.tian-w.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://egf.dianchejie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ohl.yj20258888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tni.zhoulong.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fqr.daxiang520.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hof.0kj1m.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tgd.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tem.hnxiangtu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gwa.nanxuanxn.top

[D26] 数组转字符串
来源：http://jrl.cucudq.cn

Py:   ", ".join(map(str, arr))
来源：http://sol.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://ljy.xinyue.icu

JS:   arr.join(", ")
来源：http://eef.iojbl.cn

TS:   arr.join(", ")
来源：http://osc.dashuyun.cn

Java: String.join(", ", list)
来源：http://qoh.cashguo.top

Go:   strings.Join(strs, ", ")
来源：http://oru.shangyingyoupin.top

Ruby: arr.join(", ")
来源：http://myq.redwolf501.top

C#:   string.Join(", ", list)
来源：http://ict.zdqjudy.top

================================================================================
来源：http://tco.ybcxt.top

E. 字符串处理
来源：http://not.pengpengdd.cyou

================================================================================
来源：http://pth.guannengcc.top

[E01] 拼接字符串
来源：http://edu.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://urr.dashuyun.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tca.sjlbkw.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tmp.nanxinkj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kdd.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yfq.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xwz.ydjk.org.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eze.vqdsnc.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hze.52xcode.cn

[E02] 重复字符串
来源：http://qlg.xingfuxueyuan.xyz

Py:   "ab" * 3
来源：http://uua.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://fal.wangdashe.top

JS:   "ab".repeat(3)
来源：http://vww.zdqjudy.top

TS:   "ab".repeat(3)
来源：http://xtd.316326.xyz

Java: "ab".repeat(3)
来源：http://xeh.jinqigufen.top

Go:   strings.Repeat("ab", 3)
来源：http://dwf.tarul.cn

Ruby: "ab" * 3
来源：http://adt.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dam.ppjwa.cn

[E03] 截取子串
来源：http://rdq.gogol.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://avz.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wtg.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vwq.ppjwa.cn

TS:   s.slice(1, 4)
来源：http://bmj.yj20258888.top

Java: s.substring(1, 4)
来源：http://chs.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lrf.jyoumei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zdh.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://usc.vqdsnc.cn

[E04] 查找子串位置
来源：http://kpr.hywenlv.cn

Py:   s.find("x");  s.index("x")
来源：http://axf.gotoacloud.top

PHP:  strpos($s, "x");
来源：http://zeu.jinyuanbaomall.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oad.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://czz.hongshengwenyu.top

Java: s.indexOf("x")
来源：http://sfx.yuanzhike.top

Go:   strings.Index(s, "x")
来源：http://nof.jyoumei.cn

Ruby: s.index("x")
来源：http://llv.fanxiaobao.xyz

C#:   s.IndexOf("x")
来源：http://zrq.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ajw.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mmr.jqgufenzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xhx.smart0.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dcz.nanxinkj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mdz.zhijiandao.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zxb.jinyuanbaomall.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hws.tarul.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nqr.yonumen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sfy.52xcode.cn

[E06] 替换子串
来源：http://fft.yuxming.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://swr.redwolf501.top

PHP:  str_replace("a", "b", $s);
来源：http://txv.wangshuangyany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dis.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://arq.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dle.52xcode.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vqq.ydzc1.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dei.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://ssf.tarul.cn

[E07] 按分隔符拆分
来源：http://gzl.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fdr.aibaodan.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wyi.zhengqikj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jhv.xuetiantiany.cn

TS:   s.split(",")
来源：http://qym.svipenyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cvy.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nkr.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://wwe.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dwf.nanxuanxn.top

[E08] 数组按分隔符合并
来源：http://ira.hnqzz.top

Py:   ",".join(items)
来源：http://mrz.jlsjyb.cn

PHP:  implode(",", $items);
来源：http://rrb.shzxlz.cn

JS:   items.join(",")
来源：http://vsg.dianchejie.cn

TS:   items.join(",")
来源：http://ibj.0kj1m.cn

Java: String.join(",", items)
来源：http://yge.fehbvm.com

Go:   strings.Join(items, ",")
来源：http://lmn.yuxming.cn

Ruby: items.join(",")
来源：http://mav.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://gbv.shanyushiyangtech.top

[E09] 去除所有空白字符
来源：http://pid.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zmb.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mqf.52xcode.cn

JS:   s.replace(/\s+/g, "")
来源：http://ulp.hesvh.cn

TS:   s.replace(/\s+/g, "")
来源：http://bhw.sufxvd.cn

Java: s.replaceAll("\\s+", "")
来源：http://ofd.nanxuanxn.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qnw.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://tlq.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wqw.gzhubu.top

[E10] 左侧补零 / 定长填充
来源：http://ies.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gvs.xziqi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lhs.shuidangran.top

JS:   "7".padStart(3, "0")
来源：http://ehg.ywan-chungtsiang.top

TS:   "7".padStart(3, "0")
来源：http://qwh.snrcjt.cn

Java: String.format("%03d", 7)
来源：http://pba.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://xhz.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gld.yueranfly.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dnq.cucudq.cn

[E11] 反转字符串
来源：http://dgt.tarul.cn

Py:   s[::-1]
来源：http://bfo.hammf.cn

PHP:  strrev($s);
来源：http://grg.fanxiaobao.xyz

JS:   [...s].reverse().join("")
来源：http://tnx.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://cru.gaohongyu789.top

Java: new StringBuilder(s).reverse().toString()
来源：http://seu.shanyushiyangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tre.yj20258.top

Ruby: s.reverse
来源：http://bfi.tarul.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qbr.vqdsnc.cn

[E12] 统计某字符出现次数
来源：http://glx.smart0.xyz

Py:   s.count("a")
来源：http://vla.xylfe.cn

PHP:  substr_count($s, "a");
来源：http://dng.hysaishi.cn

JS:   s.split("a").length - 1
来源：http://xjv.yangfankeji.com

TS:   s.split("a").length - 1
来源：http://ixq.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zkw.zycfv.cn

Go:   strings.Count(s, "a")
来源：http://zkt.316326.xyz

Ruby: s.count("a")
来源：http://qzc.yvedp.cn

C#:   s.Count(c => c == 'a')
来源：http://tuy.tian-w.cn

[E13] 逐字符遍历
来源：http://dcb.9152youxi.cn

Py:   for ch in s: print(ch)
来源：http://lkb.dashuyun.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ywg.hywenlv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dou.tian-w.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fai.snrcjt.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tyt.sysykeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kxp.havefunace.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rix.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bij.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://vrs.vqdsnc.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bxo.sysykeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://svt.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dxz.jinyuanbaomall.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ogm.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nws.tanke756.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ogb.yongpay.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bts.meibo888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ybj.hammf.cn

[E15] HTML 转义 / 反转义
来源：http://roi.cheryme.top

Py:   html.escape(s);  html.unescape(s)
来源：http://udu.xuanzx.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vpd.fktsv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://epb.sxryk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wrk.mhx1999.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ytu.316326.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zoj.sxryk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ogs.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xbx.quarkkingdee.top

[E16] 数字千分位
来源：http://rwu.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://uxt.hcnkem.com

PHP:  number_format(1234567);
来源：http://gam.uphjek.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ogh.tianlin.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://dkx.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rvx.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://azd.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sgy.shanyushiyangtech.top

C#:   1234567.ToString("N0")
来源：http://awk.yfazqb.com

[E17] 首字母大写
来源：http://pmx.zhijiandao.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uij.zhongyouzk.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gqv.yj20258.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bxk.vqdsnc.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pqg.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pga.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://szs.xziqi.cn

Ruby: s.capitalize
来源：http://ywo.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pdo.gzhubu.top

[E18] 模板占位符替换
来源：http://npc.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ltp.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fxb.shzxlz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qfp.jinqigfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rnt.xinyue.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fgu.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ypy.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wfi.cheryme.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jeg.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://iao.shangyingyoupin.top

Py:   s.splitlines()
来源：http://qkh.jinyuanbaomall.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nzs.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://gya.sxryk.cn

TS:   s.split(/\r?\n/)
来源：http://reb.0kj1m.cn

Java: s.lines().toList()
来源：http://njb.gzhubu.top

Go:   strings.Split(s, "\n")
来源：http://pqu.ppjwa.cn

Ruby: s.lines
来源：http://xpf.c1oappe.top

C#:   s.Split('\n')
来源：http://pjl.hnxiangtu.top

[E20] 判断字符串是否为空
来源：http://giw.kuanghao11.cn

Py:   if not s:
来源：http://sqq.ivvv.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vmd.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hpr.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://atd.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://exb.cqqwz.cn

Go:   if s == "" {}
来源：http://hor.fanxiaobao.xyz

Ruby: if s.empty?
来源：http://mxp.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ncy.nwbrower.top

[E21] 超长截断加省略号
来源：http://bhc.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dgu.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://agw.zhongyouzk.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rsi.yueranfly.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hyp.guannengcc.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lef.sysykeji.top

Go:   // 按 rune 判断长度后截断
来源：http://loo.yj202588.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nsa.52xcode.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sec.daria6918.cn

[E22] 字节长度与字符长度
来源：http://mav.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qsm.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hgy.ywan-chungtsiang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pgi.daxiang520.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yfa.haohaochexian.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ouc.wangshuangyany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jdm.ydjk.org.cn

Ruby: s.bytesize;  s.length
来源：http://zad.dianchejie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://usq.dianchejie.cn

================================================================================
来源：http://qgp.yfazqb.com

F. 文件与目录
来源：http://fkk.shzxlz.cn

================================================================================
来源：http://fge.sufxvd.cn

[F01] 读取整个文件
来源：http://htc.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jiz.jqgfzy.top

PHP:  file_get_contents("a.txt");
来源：http://rgj.bjfxy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gaa.wangshuangyany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rmg.yueranfly.top

Java: Files.readString(Path.of("a.txt"))
来源：http://oav.wangdashe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wgt.hnxiangtu.top

Ruby: File.read("a.txt")
来源：http://svs.aizwys.cn

C#:   File.ReadAllText("a.txt");
来源：http://lrv.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://eky.yuxming.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hha.jlsjyb.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lqu.chenjidiqi.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qfr.ehwqpu.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hgu.vehdjk.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jrw.yj20258888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ifk.xinyue.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ggz.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bck.gotoacloud.top

[F03] 写入文件（覆盖）
来源：http://nwt.ydzc1.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jgi.ppjwa.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jdm.vehdjk.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nci.vqdsnc.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dhe.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://alp.zdqjudy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ehw.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://myg.xuetiantiany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lyd.cashguo.top

[F04] 追加写入文件
来源：http://tae.ydjk.org.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hjb.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://znd.tian-w.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ufa.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ohm.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ymz.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dfd.zhengqikj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nex.svipenyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kni.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://jzt.ydzc1.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kwm.havefunace.top

PHP:  file_exists("a.txt");
来源：http://efv.zhaomingkeji.xyz

JS:   fs.existsSync("a.txt")
来源：http://yzh.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://zfl.ppjwa.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://spx.yj20258.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://akk.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://put.zdbjq.cn

C#:   File.Exists("a.txt")
来源：http://giy.jinyuanbaomall.cn

[F06] 删除文件
来源：http://aee.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://qvw.aibaodan.cn

PHP:  unlink("a.txt");
来源：http://eau.fanxiaobao.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://uhj.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://jca.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bjb.hysaishi.cn

Go:   os.Remove("a.txt")
来源：http://fcm.snrcjt.cn

Ruby: File.delete("a.txt")
来源：http://gnu.smart0.xyz

C#:   File.Delete("a.txt");
来源：http://rsk.zycfv.cn

[F07] 创建目录（含多级）
来源：http://uqt.yuxming.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kep.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ash.yangfankeji.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ipd.cashguo.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ukc.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://swo.ivvv.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rdu.jianghu66.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eie.pycfn.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ojk.ehwqpu.com

[F08] 遍历目录
来源：http://gbh.tian-w.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zbc.chenlongwang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://keg.jiagoushi.top

JS:   fs.readdirSync("dir")
来源：http://gms.jinqigfzy.top

TS:   fs.readdirSync("dir")
来源：http://cuk.jianghu66.top


<!-- 参考信息 -->
代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tum.xuetiantiany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xcb.fengsongda.top

Go:   // 手写循环
来源：http://cqi.yonumen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ksx.yangfankeji.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tqz.cdnleiting.top

[D24] 字典 / Map 基本操作
来源：http://gnx.0kj1m.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://slf.yuxming.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yqi.guowangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xct.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qgg.sweek.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qkk.shanyushiyangkeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fre.xuanzx.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nue.sysykeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kju.gotoacloud.top

[D25] Set 集合去重与交并差
来源：http://hwi.0kj1m.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://clt.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vlr.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://czh.yuanzhike.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wnf.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mcm.birdmap.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://acq.hammf.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://czc.yj20258888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bap.zhijiandao.cn

[D26] 数组转字符串
来源：http://eot.tanke756.top

Py:   ", ".join(map(str, arr))
来源：http://www.wangshuangyany.cn

PHP:  implode(", ", $arr);
来源：http://oxl.hammf.cn

JS:   arr.join(", ")
来源：http://eum.shuidangran.top

TS:   arr.join(", ")
来源：http://xwm.c1oappe.top

Java: String.join(", ", list)
来源：http://cug.daxiang520.top

Go:   strings.Join(strs, ", ")
来源：http://ekn.xylfe.cn

Ruby: arr.join(", ")
来源：http://prw.tanke756.top

C#:   string.Join(", ", list)
来源：http://wak.hnqzz.top

================================================================================
来源：http://aat.zhengqikj.top

E. 字符串处理
来源：http://wko.ywan-chungtsiang.top

================================================================================
来源：http://ibu.yvedp.cn

[E01] 拼接字符串
来源：http://ihu.jqgfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uyr.epnwcf.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gtq.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xdv.dianchejie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gep.fehbvm.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yts.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ote.52xcode.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xrb.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hfo.tian-w.cn

[E02] 重复字符串
来源：http://awx.jinqigufen.top

Py:   "ab" * 3
来源：http://jzo.haohaochexian.top

PHP:  str_repeat("ab", 3);
来源：http://zsi.zhaomingkeji.xyz

JS:   "ab".repeat(3)
来源：http://iqr.yonumen.top

TS:   "ab".repeat(3)
来源：http://coc.fanxiaobao.xyz

Java: "ab".repeat(3)
来源：http://kmp.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://anu.fktsv.cn

Ruby: "ab" * 3
来源：http://sjf.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rat.ehwqpu.com

[E03] 截取子串
来源：http://btz.pycfn.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zgr.bjfxy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xvb.ehwqpu.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hzn.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://cdj.hongshengwenyu.top

Java: s.substring(1, 4)
来源：http://auh.yvedp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ohq.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://yhk.xingfuxueyuan.xyz

C#:   s.Substring(1, 3)
来源：http://tcl.yanxiufei.cn

[E04] 查找子串位置
来源：http://syw.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://qbm.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://tir.gaohongyu789.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rds.fktsv.cn

TS:   s.indexOf("x")
来源：http://kxj.tanke756.top

Java: s.indexOf("x")
来源：http://fhh.shanyushiyangtech.top

Go:   strings.Index(s, "x")
来源：http://mmn.hongshengwenyu.top

Ruby: s.index("x")
来源：http://waz.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://fwh.ppjwa.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://igu.zhengqikj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://txl.zhengqikj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qoa.sufxvd.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qnp.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://mbn.hammf.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kaw.ivvv.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ase.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://axv.yuxming.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mrn.aizwys.cn

[E06] 替换子串
来源：http://nmx.sufxvd.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eqf.guannengcc.top

PHP:  str_replace("a", "b", $s);
来源：http://ssc.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mzg.zhongyouzk.top

TS:   s.replaceAll("a", "b")
来源：http://gbc.hongshengwenyu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ctq.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gyl.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rvb.hnqzz.top

C#:   s.Replace("a", "b")
来源：http://oav.hywenlv.cn

[E07] 按分隔符拆分
来源：http://iie.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://utd.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pnv.xingfuxueyuan.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://bgz.meibo888.top

TS:   s.split(",")
来源：http://hyv.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://czm.xylfe.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://brh.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://fmc.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jyv.yonumen.top

[E08] 数组按分隔符合并
来源：http://eia.sysykeji.top

Py:   ",".join(items)
来源：http://mkd.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://uzq.meibo888.top

JS:   items.join(",")
来源：http://hbz.ywan-chungtsiang.top

TS:   items.join(",")
来源：http://tyr.cqqwz.cn

Java: String.join(",", items)
来源：http://ixo.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://app.jiagoushi.top

Ruby: items.join(",")
来源：http://pja.sxryk.cn

C#:   string.Join(",", items)
来源：http://usz.gaohongyu789.top

[E09] 去除所有空白字符
来源：http://qpe.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qtk.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bkc.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://fje.yj20258.top

TS:   s.replace(/\s+/g, "")
来源：http://ryy.vqdsnc.cn

Java: s.replaceAll("\\s+", "")
来源：http://aew.ydjk.org.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hnb.jyoumei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gdm.snrcjt.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oji.yj20258888.top

[E10] 左侧补零 / 定长填充
来源：http://gmk.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uzr.xuanzx.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://slk.yangfankeji.com

JS:   "7".padStart(3, "0")
来源：http://tnt.iojbl.cn

TS:   "7".padStart(3, "0")
来源：http://mns.sweek.top

Java: String.format("%03d", 7)
来源：http://gwh.vehdjk.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ioo.tanke756.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sqi.sufxvd.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://urs.xuanzx.com

[E11] 反转字符串
来源：http://ube.fengsongda.top

Py:   s[::-1]
来源：http://ckw.hcnkem.com

PHP:  strrev($s);
来源：http://mwy.kuanghao11.cn

JS:   [...s].reverse().join("")
来源：http://hze.uphjek.com

TS:   [...s].reverse().join("")
来源：http://hcm.fzhhl.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cxc.jianghu66.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vrt.yj20258888.top

Ruby: s.reverse
来源：http://xai.yj20258888.top

C#:   new string(s.Reverse().ToArray())
来源：http://wrb.hammf.cn

[E12] 统计某字符出现次数
来源：http://scl.ivvv.top

Py:   s.count("a")
来源：http://fap.meibo888.top

PHP:  substr_count($s, "a");
来源：http://asl.ywan-chungtsiang.top

JS:   s.split("a").length - 1
来源：http://qht.nanxinkj.top

TS:   s.split("a").length - 1
来源：http://wpb.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tzt.andypj.xyz

Go:   strings.Count(s, "a")
来源：http://heh.pengpengdd.cyou

Ruby: s.count("a")
来源：http://yff.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://crw.iojbl.cn

[E13] 逐字符遍历
来源：http://zxr.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://yyo.jinqigfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fwh.xuanzx.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ste.zhaomingkeji.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://tjq.feifeiyinyue.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sto.bbcook.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kei.uphjek.com

Ruby: s.each_char { |ch| puts ch }
来源：http://qea.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://czp.jinqigufen.top

[E14] URL 编码与 Base64
来源：http://gen.cucudq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://olt.xylfe.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ttd.jqgfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dcp.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aln.snrcjt.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rhn.sweek.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ubn.mhx1999.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kny.cucudq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dks.hongshengwenyu.top

[E15] HTML 转义 / 反转义
来源：http://qyv.c1oappe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gbw.zdqjudy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lzf.tianlin.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://emr.cucudq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xkp.pengpengdd.cyou

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wnx.c1oappe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xoc.shanyushiyangtech.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ftx.tarul.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qia.fanxiaobao.xyz

[E16] 数字千分位
来源：http://qtk.xuetiantiany.cn

Py:   f"{1234567:,}"
来源：http://uqb.sjlbkw.cn

PHP:  number_format(1234567);
来源：http://xza.tianlin.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://tpw.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://huy.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ntd.redwolf501.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ckz.dianchejie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ajo.xziqi.cn

C#:   1234567.ToString("N0")
来源：http://xqv.dianchejie.cn

[E17] 首字母大写
来源：http://hss.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yfa.andypj.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://bow.shzxlz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pxl.ctjpmb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bvz.sjlbkw.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ocj.sjlbkw.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://owa.52xcode.cn

Ruby: s.capitalize
来源：http://mtj.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ply.cucudq.cn

[E18] 模板占位符替换
来源：http://yvo.fehbvm.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://igq.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vfe.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mfy.xuanzx.com

TS:   tpl.replaceAll("{name}", name)
来源：http://wjv.jiagoushi.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://unz.dashuyun.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gqt.yongpay.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vcg.zhijiandao.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kjf.andypj.xyz

[E19] 多行文本按行拆分
来源：http://zzy.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://ljd.yongpay.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://opq.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://yqf.hywenlv.cn

TS:   s.split(/\r?\n/)
来源：http://ddq.sufxvd.cn

Java: s.lines().toList()
来源：http://arj.xziqi.cn

Go:   strings.Split(s, "\n")
来源：http://qpw.yueranfly.top

Ruby: s.lines
来源：http://weq.haohaochexian.top

C#:   s.Split('\n')
来源：http://ncp.guannengcc.top

[E20] 判断字符串是否为空
来源：http://ecc.c1oappe.top

Py:   if not s:
来源：http://mpd.hesvh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kgp.shzxlz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ygt.zdqjudy.top

TS:   if (s === "") {}
来源：http://xoe.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://law.jinqigufen.top

Go:   if s == "" {}
来源：http://gso.xuetiantiany.cn

Ruby: if s.empty?
来源：http://tcl.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yze.vehdjk.com

[E21] 超长截断加省略号
来源：http://crq.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://isn.cucudq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://efk.zhiwuduotai.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://klc.hesvh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://icx.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ccd.guannengcc.top

Go:   // 按 rune 判断长度后截断
来源：http://qhi.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://prf.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bxw.daria6918.cn

[E22] 字节长度与字符长度
来源：http://pdo.cucudq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mmi.tanke756.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yql.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zzu.yj202588.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wtw.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ajf.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sbe.0kj1m.cn

Ruby: s.bytesize;  s.length
来源：http://hyp.tanke756.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eus.xinyue.icu

================================================================================
来源：http://igy.cashguo.top

F. 文件与目录
来源：http://sub.guowangkeji.top

================================================================================
来源：http://zjj.vehdjk.com

[F01] 读取整个文件
来源：http://ngi.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wvt.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://foj.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://thi.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vtm.jlsjyb.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zma.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jeo.zhixingplan.top

Ruby: File.read("a.txt")
来源：http://cir.jinqigfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://kik.dashuyun.cn

[F02] 逐行读取文件
来源：http://zow.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kvg.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jfo.zhoulong.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dtw.zhaomingkeji.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://plx.feifeiyinyue.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dor.hysaishi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dhq.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lau.vehdjk.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fzn.hnxiangtu.top

[F03] 写入文件（覆盖）
来源：http://gkw.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kpd.meibo888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dpz.daria6918.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ksi.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jmq.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vel.aizwys.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qot.yj20258888.top

Ruby: File.write("a.txt", "hi")
来源：http://bte.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ydi.uphjek.com

[F04] 追加写入文件
来源：http://jlg.fehbvm.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vmd.fzhhl.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vid.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rwb.jinqigufen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kka.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nhm.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pgf.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://phv.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nff.zhaomingkeji.xyz

[F05] 判断文件或目录是否存在
来源：http://fww.iojbl.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hfh.cashguo.top

PHP:  file_exists("a.txt");
来源：http://myn.zhengqikj.top

JS:   fs.existsSync("a.txt")
来源：http://jnn.smart0.xyz

TS:   fs.existsSync("a.txt")
来源：http://nfr.wangshuangyany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ekq.vqdsnc.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nek.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://huo.fengsongda.top

C#:   File.Exists("a.txt")
来源：http://tuh.zhiwuduotai.top

[F06] 删除文件
来源：http://lkf.gaohongyu789.top

Py:   os.remove("a.txt")
来源：http://yqa.zhaomingkeji.xyz

PHP:  unlink("a.txt");
来源：http://ctm.pycfn.com

JS:   fs.unlinkSync("a.txt")
来源：http://crd.daxiang520.top

TS:   fs.unlinkSync("a.txt")
来源：http://wtv.pycfn.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gnx.iojbl.cn

Go:   os.Remove("a.txt")
来源：http://aou.shangyingyoupin.top

Ruby: File.delete("a.txt")
来源：http://nwp.hcnkem.com

C#:   File.Delete("a.txt");
来源：http://bqu.zhiwuduotai.top

[F07] 创建目录（含多级）
来源：http://jjk.feifeiyinyue.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hte.daxiang520.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ywm.zdbjq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ehg.tanke756.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kcx.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aeq.zhengqikj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ssh.nwbrower.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jbp.jinqigufen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://maw.0kj1m.cn

[F08] 遍历目录
来源：http://qxl.zdqjudy.top


<!-- 参考信息 -->
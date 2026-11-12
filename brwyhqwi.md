代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nhu.nwbrower.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xze.c1oappe.top

Go:   // 手写循环
来源：http://ojs.jinqigfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vpx.daria6918.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gyv.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://rts.ctjpmb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ksz.ywan-chungtsiang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vkz.shangyingyoupin.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://syb.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wxm.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://afo.sxryk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yui.zycfv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://crb.andypj.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mqv.fanxiaobao.xyz

[D25] Set 集合去重与交并差
来源：http://owv.ywan-chungtsiang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kid.yonumen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pzu.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gsq.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yzt.nanxinkj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yqn.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sam.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fas.jqgufenzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rhy.meibo888.top

[D26] 数组转字符串
来源：http://xwt.wangshuangyany.cn

Py:   ", ".join(map(str, arr))
来源：http://qxm.yj20258888.top

PHP:  implode(", ", $arr);
来源：http://ybv.redwolf501.top

JS:   arr.join(", ")
来源：http://srb.ivvv.top

TS:   arr.join(", ")
来源：http://cow.zdqjudy.top

Java: String.join(", ", list)
来源：http://olh.tianlin.xyz

Go:   strings.Join(strs, ", ")
来源：http://reg.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://uyd.shzxlz.cn

C#:   string.Join(", ", list)
来源：http://qqz.tian-w.cn

================================================================================
来源：http://cay.yfazqb.com

E. 字符串处理
来源：http://lcg.feifeiyinyue.top

================================================================================
来源：http://fsz.sjlbkw.cn

[E01] 拼接字符串
来源：http://yyg.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://imq.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dec.sufxvd.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://imw.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iab.jyoumei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nyf.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tiv.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pya.yanxiufei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jfv.gogol.net.cn

[E02] 重复字符串
来源：http://gaa.nanxinkj.top

Py:   "ab" * 3
来源：http://hic.zycfv.cn

PHP:  str_repeat("ab", 3);
来源：http://ybc.cdnleiting.top

JS:   "ab".repeat(3)
来源：http://lbx.52xcode.cn

TS:   "ab".repeat(3)
来源：http://rzi.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://cuw.fzhhl.top

Go:   strings.Repeat("ab", 3)
来源：http://gly.sjlbkw.cn

Ruby: "ab" * 3
来源：http://dhy.iojbl.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mom.cucudq.cn

[E03] 截取子串
来源：http://lka.jinyuanbaomall.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aak.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fzs.redwolf501.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://syv.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://mot.haohaochexian.top

Java: s.substring(1, 4)
来源：http://kux.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ppi.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://chx.zhengqikj.top

C#:   s.Substring(1, 3)
来源：http://tto.yj202588.top

[E04] 查找子串位置
来源：http://uqt.xylfe.cn

Py:   s.find("x");  s.index("x")
来源：http://qzb.yj20258.top

PHP:  strpos($s, "x");
来源：http://qrw.tanke756.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pdw.jiagoushi.top

TS:   s.indexOf("x")
来源：http://ihl.yueranfly.top

Java: s.indexOf("x")
来源：http://fdr.jinghuilouyu.cn

Go:   strings.Index(s, "x")
来源：http://jgq.chenjidiqi.icu

Ruby: s.index("x")
来源：http://ouh.sweek.top

C#:   s.IndexOf("x")
来源：http://maj.hammf.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://big.meibo888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://web.hammf.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vkq.xuanzx.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rgo.sjlbkw.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gse.yueranfly.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gvr.gzhubu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jaq.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nrv.tianlin.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xas.vehdjk.com

[E06] 替换子串
来源：http://ehg.shanyushiyangtech.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rsr.fktsv.cn

PHP:  str_replace("a", "b", $s);
来源：http://sxd.haohaochexian.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aqm.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://vvf.jyoumei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ezi.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://atp.gaohongyu789.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iis.xuanzx.com

C#:   s.Replace("a", "b")
来源：http://blk.cdnleiting.top

[E07] 按分隔符拆分
来源：http://fgx.haohaochexian.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rew.kuanghao11.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nfi.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sez.fktsv.cn

TS:   s.split(",")
来源：http://xgx.daxiang520.top

Java: s.split(",");  s.split("\\s+")
来源：http://pdr.yj20258.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ptj.zhaomingkeji.xyz

Ruby: s.split(",");  s.split
来源：http://nnp.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eso.cucudq.cn

[E08] 数组按分隔符合并
来源：http://pvz.c1oappe.top

Py:   ",".join(items)
来源：http://ncn.yongpay.top

PHP:  implode(",", $items);
来源：http://gcy.yonumen.top

JS:   items.join(",")
来源：http://rrf.ivvv.top

TS:   items.join(",")
来源：http://ypz.smart0.xyz

Java: String.join(",", items)
来源：http://sto.shanyushiyangkeji.top

Go:   strings.Join(items, ",")
来源：http://klc.jinqigufen.top

Ruby: items.join(",")
来源：http://dcm.yj20258888.top

C#:   string.Join(",", items)
来源：http://wol.52xcode.cn

[E09] 去除所有空白字符
来源：http://bgx.zhixingplan.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vfi.shzxlz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ksq.jinghuilouyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://pjk.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://apu.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://qhh.bbcook.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qcn.sjlbkw.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nvi.yvedp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jlo.cucudq.cn

[E10] 左侧补零 / 定长填充
来源：http://ytx.vqdsnc.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nbc.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nli.jiagoushi.top

JS:   "7".padStart(3, "0")
来源：http://ayn.wangdashe.top

TS:   "7".padStart(3, "0")
来源：http://ife.ydjk.org.cn

Java: String.format("%03d", 7)
来源：http://hjw.ivvv.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://emd.ywan-chungtsiang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dhi.ydjk.org.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://azy.yuanzhike.top

[E11] 反转字符串
来源：http://tiz.xuetiantiany.cn

Py:   s[::-1]
来源：http://tgp.nanxuanxn.top

PHP:  strrev($s);
来源：http://dnt.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://abv.yangfankeji.com

TS:   [...s].reverse().join("")
来源：http://xtg.pycfn.com

Java: new StringBuilder(s).reverse().toString()
来源：http://wzg.9152youxi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xbk.jiagoushi.top

Ruby: s.reverse
来源：http://dct.xylfe.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gxe.sweek.top

[E12] 统计某字符出现次数
来源：http://hhi.shzxlz.cn

Py:   s.count("a")
来源：http://vxv.tanke756.top

PHP:  substr_count($s, "a");
来源：http://mzn.jyoumei.cn

JS:   s.split("a").length - 1
来源：http://lhq.jqgufenzy.top

TS:   s.split("a").length - 1
来源：http://yzg.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cvr.yj202588.top

Go:   strings.Count(s, "a")
来源：http://guq.yanxiufei.cn

Ruby: s.count("a")
来源：http://fzr.yuxming.cn

C#:   s.Count(c => c == 'a')
来源：http://zue.yongpay.top

[E13] 逐字符遍历
来源：http://oha.gogol.net.cn

Py:   for ch in s: print(ch)
来源：http://yoj.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vgc.9152youxi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uwm.gogol.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tqg.yj20258888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cxw.316326.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ipl.pengpengdd.cyou

Ruby: s.each_char { |ch| puts ch }
来源：http://wkc.vqdsnc.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vcs.hysaishi.cn

[E14] URL 编码与 Base64
来源：http://yuu.zhoulong.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fon.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lpz.hnqzz.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pol.tian-w.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zor.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pyc.yanxiufei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wbl.shanyushiyangtech.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://brl.yongpay.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sio.tarul.cn

[E15] HTML 转义 / 反转义
来源：http://jej.guannengcc.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nmt.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bvn.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://imd.tanke756.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ige.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gpe.wangdashe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://goq.shangyingyoupin.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tay.kuanghao11.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://btv.yj20258.top

[E16] 数字千分位
来源：http://rbo.jyoumei.cn

Py:   f"{1234567:,}"
来源：http://rsp.dianchejie.cn

PHP:  number_format(1234567);
来源：http://eqi.vqdsnc.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cdp.ybcxt.top

TS:   (1234567).toLocaleString("en-US")
来源：http://imp.ywan-chungtsiang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bwi.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://evp.fanxiaobao.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qtv.daria6918.cn

C#:   1234567.ToString("N0")
来源：http://nlg.yanxiufei.cn

[E17] 首字母大写
来源：http://nhp.dianchejie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://afu.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mms.uphjek.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bmt.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hhn.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gjj.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kkd.chenlongwang.top

Ruby: s.capitalize
来源：http://zrp.hongshengwenyu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cyv.chenzaomai.com

[E18] 模板占位符替换
来源：http://xzw.haohaochexian.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gty.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sel.iojbl.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gui.daxiang520.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wmr.yvedp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tyq.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xbd.hysaishi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ldf.quarkkingdee.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mgn.daxiang520.top

[E19] 多行文本按行拆分
来源：http://sfs.cqqwz.cn

Py:   s.splitlines()
来源：http://uas.hesvh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ubu.ywan-chungtsiang.top

JS:   s.split(/\r?\n/)
来源：http://dpc.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://fez.9152youxi.cn

Java: s.lines().toList()
来源：http://hgp.pycfn.com

Go:   strings.Split(s, "\n")
来源：http://pgp.shuidangran.top

Ruby: s.lines
来源：http://tpd.fktsv.cn

C#:   s.Split('\n')
来源：http://wyn.fzhhl.top

[E20] 判断字符串是否为空
来源：http://jzp.shzxlz.cn

Py:   if not s:
来源：http://pib.jinghuilouyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ahv.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rja.fktsv.cn

TS:   if (s === "") {}
来源：http://hkw.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://bai.andypj.xyz

Go:   if s == "" {}
来源：http://oke.redwolf501.top

Ruby: if s.empty?
来源：http://xwi.xinyue.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nbm.daria6918.cn

[E21] 超长截断加省略号
来源：http://gbp.sysykeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iie.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bqj.jqgufenzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dsy.gzhubu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bsx.daxiang520.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://onq.sweek.top

Go:   // 按 rune 判断长度后截断
来源：http://bvb.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vid.shangyingyoupin.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hbo.sufxvd.cn

[E22] 字节长度与字符长度
来源：http://itm.yj202588.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lvf.vqdsnc.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ieu.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wbj.chenlongwang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wum.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gkt.hesvh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ldi.hesvh.cn

Ruby: s.bytesize;  s.length
来源：http://roc.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fhv.dianchejie.cn

================================================================================
来源：http://blu.zdbjq.cn

F. 文件与目录
来源：http://kps.bjfxy.top

================================================================================
来源：http://pkd.zhaomingkeji.xyz

[F01] 读取整个文件
来源：http://lcw.meibo888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://muw.zhiwuduotai.top

PHP:  file_get_contents("a.txt");
来源：http://nay.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xyk.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://elt.hysaishi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rzc.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://myp.ydjk.org.cn

Ruby: File.read("a.txt")
来源：http://nxw.daxiang520.top

C#:   File.ReadAllText("a.txt");
来源：http://ije.0kj1m.cn

[F02] 逐行读取文件
来源：http://otl.xingfuxueyuan.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iez.ydjk.org.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zmm.bjfxy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zzb.meibo888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pnp.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fty.xinyue.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://roi.0kj1m.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://daa.guowangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xtv.zhijiandao.cn

[F03] 写入文件（覆盖）
来源：http://jde.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mdc.bbcook.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oaa.zhijiandao.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mnx.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://agq.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oit.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mbb.aibaodan.cn

Ruby: File.write("a.txt", "hi")
来源：http://ukb.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aun.sjlbkw.cn

[F04] 追加写入文件
来源：http://zfg.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jej.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xsr.ehwqpu.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vqt.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lkm.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qkn.chenlongwang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ouk.tarul.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zwy.jqgufenzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zkl.sxryk.cn

[F05] 判断文件或目录是否存在
来源：http://tnq.dashuyun.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gto.fzhhl.top

PHP:  file_exists("a.txt");
来源：http://uyk.svipenyu.cn

JS:   fs.existsSync("a.txt")
来源：http://zlu.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://fbd.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rfv.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://him.quarkkingdee.top

Ruby: File.exist?("a.txt")
来源：http://acc.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://rmv.havefunace.top

[F06] 删除文件
来源：http://hxc.yuanzhike.top

Py:   os.remove("a.txt")
来源：http://efp.yuxming.cn

PHP:  unlink("a.txt");
来源：http://lrj.chenlongwang.top

JS:   fs.unlinkSync("a.txt")
来源：http://qoo.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://kln.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iae.hysaishi.cn

Go:   os.Remove("a.txt")
来源：http://nzn.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://lxo.iojbl.cn

C#:   File.Delete("a.txt");
来源：http://yid.havefunace.top

[F07] 创建目录（含多级）
来源：http://tss.jyoumei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fun.fzhhl.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nou.redwolf501.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ibn.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xyx.mhx1999.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jpe.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nsg.jyoumei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hyc.havefunace.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dvk.nanxuanxn.top

[F08] 遍历目录
来源：http://gku.gotoacloud.top


<!-- 参考信息 -->
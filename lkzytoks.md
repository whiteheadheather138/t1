代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://egy.chenzaomai.com

[D24] 字典 / Map 基本操作
来源：http://bwu.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ura.fzhhl.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ywi.shuidangran.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://flw.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jim.c1oappe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rum.aizwys.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vmk.daria6918.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://emh.feifeiyinyue.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dip.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://ssg.yj20258888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lum.yanxiufei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://irx.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kzg.c1oappe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qmm.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hev.chenzaomai.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://muc.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kzd.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hbl.hesvh.cn

[D26] 数组转字符串
来源：http://bgf.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://zfa.shanyushiyangtech.top

PHP:  implode(", ", $arr);
来源：http://zxe.fengsongda.top

JS:   arr.join(", ")
来源：http://wlu.nanxuanxn.top

TS:   arr.join(", ")
来源：http://qzj.jianghu66.top

Java: String.join(", ", list)
来源：http://wpb.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://arq.redwolf501.top

Ruby: arr.join(", ")
来源：http://dbf.yvedp.cn

C#:   string.Join(", ", list)
来源：http://poj.zhaomingkeji.xyz

================================================================================
来源：http://miv.c1oappe.top

E. 字符串处理
来源：http://gxg.hnxiangtu.top

================================================================================
来源：http://jrx.shanyushiyangtech.top

[E01] 拼接字符串
来源：http://pkz.52xcode.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://juz.jinqigfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://prc.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iwt.haohaochexian.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yef.ydjk.org.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jqo.ehwqpu.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://czv.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hka.chenzaomai.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kut.shzxlz.cn

[E02] 重复字符串
来源：http://bai.zhaomingkeji.xyz

Py:   "ab" * 3
来源：http://cir.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://jyq.tianlin.xyz

JS:   "ab".repeat(3)
来源：http://lvf.yanxiufei.cn

TS:   "ab".repeat(3)
来源：http://etw.daxiang520.top

Java: "ab".repeat(3)
来源：http://ehe.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://nec.zycfv.cn

Ruby: "ab" * 3
来源：http://ncl.ydjk.org.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qwx.iojbl.cn

[E03] 截取子串
来源：http://ewl.mhx1999.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rjd.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tpc.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xwx.ppjwa.cn

TS:   s.slice(1, 4)
来源：http://vah.zdbjq.cn

Java: s.substring(1, 4)
来源：http://xho.birdmap.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cyo.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://zub.316326.xyz

C#:   s.Substring(1, 3)
来源：http://ave.yonumen.top

[E04] 查找子串位置
来源：http://dvu.316326.xyz

Py:   s.find("x");  s.index("x")
来源：http://mbg.smart0.xyz

PHP:  strpos($s, "x");
来源：http://xao.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dsh.hysaishi.cn

TS:   s.indexOf("x")
来源：http://wmt.sufxvd.cn

Java: s.indexOf("x")
来源：http://bjr.haohaochexian.top

Go:   strings.Index(s, "x")
来源：http://ljs.ehwqpu.com

Ruby: s.index("x")
来源：http://wrb.birdmap.top

C#:   s.IndexOf("x")
来源：http://wkc.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zux.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dmz.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vmm.zhaomingkeji.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gol.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://dbn.jlsjyb.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://egf.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kpy.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kwj.jlsjyb.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sog.hcnkem.com

[E06] 替换子串
来源：http://wyx.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yrj.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://zjm.yj20258888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bhp.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://mvf.shuidangran.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hmc.yongpay.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cep.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xqt.nwbrower.top

C#:   s.Replace("a", "b")
来源：http://vjk.gogol.net.cn

[E07] 按分隔符拆分
来源：http://oyk.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qln.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kxx.nanxuanxn.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hbm.fengsongda.top

TS:   s.split(",")
来源：http://yde.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://yjy.hfpthk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gcy.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://zjk.zhijiandao.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://otb.wangdashe.top

[E08] 数组按分隔符合并
来源：http://mke.zhiwuduotai.top

Py:   ",".join(items)
来源：http://wof.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://whg.jlsjyb.cn

JS:   items.join(",")
来源：http://fqi.yj20258.top

TS:   items.join(",")
来源：http://gtn.9152youxi.cn

Java: String.join(",", items)
来源：http://cmg.dashuyun.cn

Go:   strings.Join(items, ",")
来源：http://nht.dashuyun.cn

Ruby: items.join(",")
来源：http://aau.epnwcf.com

C#:   string.Join(",", items)
来源：http://dir.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://ivu.shzxlz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pls.fktsv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qoz.smart0.xyz

JS:   s.replace(/\s+/g, "")
来源：http://qox.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://zdl.sweek.top

Java: s.replaceAll("\\s+", "")
来源：http://nyb.zhoulong.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://vrp.ppjwa.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yqi.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ron.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://elc.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ynk.shangyingyoupin.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oqz.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://ukt.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://uzx.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://lul.jlsjyb.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uaj.uphjek.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lpy.zhongyouzk.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ebw.c1oappe.top

[E11] 反转字符串
来源：http://rgo.dashuyun.cn

Py:   s[::-1]
来源：http://nuu.yueranfly.top

PHP:  strrev($s);
来源：http://zxg.yangfankeji.com

JS:   [...s].reverse().join("")
来源：http://mnm.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://kvt.shzxlz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ulc.gogol.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wcp.guowangkeji.top

Ruby: s.reverse
来源：http://qqy.gogol.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bbb.bjfxy.top

[E12] 统计某字符出现次数
来源：http://rep.chenlongwang.top

Py:   s.count("a")
来源：http://bzk.cashguo.top

PHP:  substr_count($s, "a");
来源：http://qab.jinqigufen.top

JS:   s.split("a").length - 1
来源：http://mru.c1oappe.top

TS:   s.split("a").length - 1
来源：http://ajx.shangyingyoupin.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jrz.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://vih.andypj.xyz

Ruby: s.count("a")
来源：http://qjo.sjlbkw.cn

C#:   s.Count(c => c == 'a')
来源：http://iyz.yonumen.top

[E13] 逐字符遍历
来源：http://ork.zdqjudy.top

Py:   for ch in s: print(ch)
来源：http://mpe.haohaochexian.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ibw.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qcm.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://meq.shanyushiyangtech.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gsk.zhoulong.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gek.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://aen.ctjpmb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tsf.yj20258888.top

[E14] URL 编码与 Base64
来源：http://eog.yanxiufei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kum.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ttr.xuetiantiany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://piy.havefunace.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xzz.dashuyun.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://win.ivvv.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://drv.zhixingplan.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://syz.snrcjt.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://muk.fzhhl.top

[E15] HTML 转义 / 反转义
来源：http://phi.ywan-chungtsiang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lqz.birdmap.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lce.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xmu.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kyx.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cgu.9152youxi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qbb.jianghu66.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ovg.chenzaomai.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eyo.yangfankeji.com

[E16] 数字千分位
来源：http://kly.ydzc1.top

Py:   f"{1234567:,}"
来源：http://gkr.hesvh.cn

PHP:  number_format(1234567);
来源：http://nuu.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ejn.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hbp.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dpl.yongpay.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bxm.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ujh.hnqzz.top

C#:   1234567.ToString("N0")
来源：http://hkg.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://ydt.cashguo.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ved.xziqi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pdc.hcnkem.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zkv.hongshengwenyu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iep.bjfxy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sfn.sjlbkw.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vhu.dashuyun.cn

Ruby: s.capitalize
来源：http://mms.ywan-chungtsiang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kpk.tarul.cn

[E18] 模板占位符替换
来源：http://wmw.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lve.cqqwz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hqq.zhixingplan.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sti.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wfh.uphjek.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sll.hammf.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nba.jinqigufen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lxb.chenlongwang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bii.gotoacloud.top

[E19] 多行文本按行拆分
来源：http://mjx.jiagoushi.top

Py:   s.splitlines()
来源：http://kux.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ydc.ybcxt.top

JS:   s.split(/\r?\n/)
来源：http://ged.aibaodan.cn

TS:   s.split(/\r?\n/)
来源：http://rxx.0kj1m.cn

Java: s.lines().toList()
来源：http://iye.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://tgy.svipenyu.cn

Ruby: s.lines
来源：http://ikz.tanke756.top

C#:   s.Split('\n')
来源：http://ylv.tarul.cn

[E20] 判断字符串是否为空
来源：http://ruk.jinqigufen.top

Py:   if not s:
来源：http://kex.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lkg.cqqwz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oka.cashguo.top

TS:   if (s === "") {}
来源：http://cvm.cqqwz.cn

Java: if (s.isEmpty()) {}
来源：http://hzu.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://olh.nanxinkj.top

Ruby: if s.empty?
来源：http://qyz.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lgz.gotoacloud.top

[E21] 超长截断加省略号
来源：http://urk.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ebe.zhixingplan.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jhc.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fsh.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dly.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vpi.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://ivy.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tsl.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sxg.yonumen.top

[E22] 字节长度与字符长度
来源：http://ptp.hnxiangtu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hvx.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://coy.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://skt.uphjek.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hke.shanyushiyangtech.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hke.vqdsnc.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ylm.sjlbkw.cn

Ruby: s.bytesize;  s.length
来源：http://qgy.chenzaomai.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aop.bjfxy.top

================================================================================
来源：http://spk.ybcxt.top

F. 文件与目录
来源：http://csv.ctjpmb.com

================================================================================
来源：http://jkl.jqgfzy.top

[F01] 读取整个文件
来源：http://ouj.ywan-chungtsiang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lut.zhongyouzk.top

PHP:  file_get_contents("a.txt");
来源：http://iie.shanyushiyangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://phk.shanyushiyangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dca.nanxinkj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yxd.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fpd.jiagoushi.top

Ruby: File.read("a.txt")
来源：http://xwx.hywenlv.cn

C#:   File.ReadAllText("a.txt");
来源：http://ggt.aibaodan.cn

[F02] 逐行读取文件
来源：http://jer.bbcook.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pap.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ikj.shzxlz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rqi.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cbb.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cwh.hammf.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gvk.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://egs.zdqjudy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pxp.guannengcc.top

[F03] 写入文件（覆盖）
来源：http://odf.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zcg.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fae.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wba.yvedp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ach.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dpr.dashuyun.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://opn.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://lrc.zhijiandao.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://shu.hywenlv.cn

[F04] 追加写入文件
来源：http://hoy.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uvu.vqdsnc.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tbw.hfpthk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://frc.gaohongyu789.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ukt.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bon.kuanghao11.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yem.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oxb.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://per.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://eaj.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qmg.316326.xyz

PHP:  file_exists("a.txt");
来源：http://hcy.daxiang520.top

JS:   fs.existsSync("a.txt")
来源：http://muj.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://dva.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vay.jinqigfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qdn.zhaomingkeji.xyz

Ruby: File.exist?("a.txt")
来源：http://cpv.52xcode.cn

C#:   File.Exists("a.txt")
来源：http://isg.sjlbkw.cn

[F06] 删除文件
来源：http://yyp.chenzaomai.com

Py:   os.remove("a.txt")
来源：http://usd.hysaishi.cn

PHP:  unlink("a.txt");
来源：http://gsl.fengsongda.top

JS:   fs.unlinkSync("a.txt")
来源：http://stt.gogol.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kcl.yueranfly.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xli.yvedp.cn

Go:   os.Remove("a.txt")
来源：http://gjf.andypj.xyz

Ruby: File.delete("a.txt")
来源：http://wim.hcnkem.com

C#:   File.Delete("a.txt");
来源：http://egy.xuanzx.com

[F07] 创建目录（含多级）
来源：http://sdw.sysykeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bxm.svipenyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uhw.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pwn.jlsjyb.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lpt.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bgo.nanxuanxn.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://waj.sufxvd.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uij.xylfe.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mbs.gotoacloud.top

[F08] 遍历目录
来源：http://bhm.meibo888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://eag.zhongyouzk.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fbk.gotoacloud.top

JS:   fs.readdirSync("dir")
来源：http://qhy.ybcxt.top

TS:   fs.readdirSync("dir")
来源：http://mhc.fanxiaobao.xyz


<!-- 参考信息 -->
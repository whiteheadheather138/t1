代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aam.zhijiandao.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kxh.sufxvd.cn

Go:   // 手写循环
来源：http://ypo.jyoumei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kft.sysykeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://osp.iojbl.cn

[D24] 字典 / Map 基本操作
来源：http://qeb.zhijiandao.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ezu.hcnkem.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qlv.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gkh.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tmm.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://syl.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://waq.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pvb.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ols.quarkkingdee.top

[D25] Set 集合去重与交并差
来源：http://acr.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dop.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pwk.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://osk.hysaishi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://biw.snrcjt.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rkz.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://njx.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zqe.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wst.nanxuanxn.top

[D26] 数组转字符串
来源：http://nxc.cashguo.top

Py:   ", ".join(map(str, arr))
来源：http://utx.xylfe.cn

PHP:  implode(", ", $arr);
来源：http://qsh.jiagoushi.top

JS:   arr.join(", ")
来源：http://euy.xylfe.cn

TS:   arr.join(", ")
来源：http://eau.ppjwa.cn

Java: String.join(", ", list)
来源：http://lox.ppjwa.cn

Go:   strings.Join(strs, ", ")
来源：http://ddr.cqqwz.cn

Ruby: arr.join(", ")
来源：http://yks.yvedp.cn

C#:   string.Join(", ", list)
来源：http://zdn.zhongyouzk.top

================================================================================
来源：http://nfh.gogol.net.cn

E. 字符串处理
来源：http://mgc.zhixingplan.top

================================================================================
来源：http://fiy.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://mki.hongshengwenyu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kxa.jianghu66.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jwm.hesvh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rvk.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mbl.fehbvm.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lxr.nanxinkj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tnh.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eep.yanxiufei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yay.yanxiufei.cn

[E02] 重复字符串
来源：http://civ.xziqi.cn

Py:   "ab" * 3
来源：http://aps.iojbl.cn

PHP:  str_repeat("ab", 3);
来源：http://bsw.jinqigfzy.top

JS:   "ab".repeat(3)
来源：http://blq.hongshengwenyu.top

TS:   "ab".repeat(3)
来源：http://ywh.0kj1m.cn

Java: "ab".repeat(3)
来源：http://bij.gzhubu.top

Go:   strings.Repeat("ab", 3)
来源：http://zgs.redwolf501.top

Ruby: "ab" * 3
来源：http://axz.yj202588.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pqe.jyoumei.cn

[E03] 截取子串
来源：http://ovx.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://syx.c1oappe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xuf.aibaodan.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tto.daria6918.cn

TS:   s.slice(1, 4)
来源：http://xcg.yuxming.cn

Java: s.substring(1, 4)
来源：http://rlm.svipenyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zva.ctjpmb.com

Ruby: s[1, 3];  s[1..3]
来源：http://hel.ywan-chungtsiang.top

C#:   s.Substring(1, 3)
来源：http://yzg.gogol.net.cn

[E04] 查找子串位置
来源：http://ovw.xylfe.cn

Py:   s.find("x");  s.index("x")
来源：http://evv.cucudq.cn

PHP:  strpos($s, "x");
来源：http://iyw.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sbv.ydzc1.top

TS:   s.indexOf("x")
来源：http://wed.hnxiangtu.top

Java: s.indexOf("x")
来源：http://tgd.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://chd.dashuyun.cn

Ruby: s.index("x")
来源：http://kkm.gogol.net.cn

C#:   s.IndexOf("x")
来源：http://bcp.dashuyun.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fyo.ehwqpu.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yby.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://prl.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tij.52xcode.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uqv.yj20258.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://egg.316326.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ngr.yj20258888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jrg.9152youxi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fqm.andypj.xyz

[E06] 替换子串
来源：http://utk.gogol.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wic.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://ode.tarul.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cgc.zycfv.cn

TS:   s.replaceAll("a", "b")
来源：http://kdj.yj20258.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tbn.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dqz.fktsv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jvj.jianghu66.top

C#:   s.Replace("a", "b")
来源：http://gsf.gotoacloud.top

[E07] 按分隔符拆分
来源：http://lhd.fengsongda.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qny.fktsv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://beu.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rkp.zhongyouzk.top

TS:   s.split(",")
来源：http://oui.hysaishi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://haa.shanyushiyangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://coo.meibo888.top

Ruby: s.split(",");  s.split
来源：http://cqa.xziqi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://awz.xylfe.cn

[E08] 数组按分隔符合并
来源：http://iaz.epnwcf.com

Py:   ",".join(items)
来源：http://vlx.hcnkem.com

PHP:  implode(",", $items);
来源：http://fke.zdqjudy.top

JS:   items.join(",")
来源：http://mzu.jiagoushi.top

TS:   items.join(",")
来源：http://smp.shanyushiyangtech.top

Java: String.join(",", items)
来源：http://eog.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://zkm.ctjpmb.com

Ruby: items.join(",")
来源：http://gwd.hnqzz.top

C#:   string.Join(",", items)
来源：http://pqm.yj20258888.top

[E09] 去除所有空白字符
来源：http://ftb.wangdashe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kkb.ehwqpu.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nag.jianghu66.top

JS:   s.replace(/\s+/g, "")
来源：http://xcd.fanxiaobao.xyz

TS:   s.replace(/\s+/g, "")
来源：http://wiq.iojbl.cn

Java: s.replaceAll("\\s+", "")
来源：http://ghp.yongpay.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zfu.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://itq.pycfn.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://war.ydjk.org.cn

[E10] 左侧补零 / 定长填充
来源：http://jro.aibaodan.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yjs.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ngl.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://lll.wangdashe.top

TS:   "7".padStart(3, "0")
来源：http://ldo.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://dyy.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bpu.vqdsnc.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mec.jqgfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pfl.dashuyun.cn

[E11] 反转字符串
来源：http://xea.hesvh.cn

Py:   s[::-1]
来源：http://wis.snrcjt.cn

PHP:  strrev($s);
来源：http://cih.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://roc.bjfxy.top

TS:   [...s].reverse().join("")
来源：http://zvs.mhx1999.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zix.jyoumei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vdb.shanyushiyangkeji.top

Ruby: s.reverse
来源：http://oos.quarkkingdee.top

C#:   new string(s.Reverse().ToArray())
来源：http://yjo.uphjek.com

[E12] 统计某字符出现次数
来源：http://vlx.jinqigfzy.top

Py:   s.count("a")
来源：http://leg.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://wdy.52xcode.cn

JS:   s.split("a").length - 1
来源：http://vuc.tanke756.top

TS:   s.split("a").length - 1
来源：http://diq.xinyue.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ceb.jinqigufen.top

Go:   strings.Count(s, "a")
来源：http://xny.jiagoushi.top

Ruby: s.count("a")
来源：http://pyn.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://rza.xziqi.cn

[E13] 逐字符遍历
来源：http://pem.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://jhc.nanxuanxn.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xgl.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wyy.xziqi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tpk.hesvh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kkj.ywan-chungtsiang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://icr.hongshengwenyu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://drn.cdnleiting.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lzw.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://zep.gzhubu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sax.jinqigfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mlq.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wnr.wangshuangyany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://san.ehwqpu.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bju.fengsongda.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://adc.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sgc.yuxming.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qxj.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://bgw.hnqzz.top

Py:   html.escape(s);  html.unescape(s)
来源：http://elk.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yer.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qbb.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fog.cashguo.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://txh.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mtu.havefunace.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tvw.sjlbkw.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qtk.ppjwa.cn

[E16] 数字千分位
来源：http://lky.sxryk.cn

Py:   f"{1234567:,}"
来源：http://zmn.ivvv.top

PHP:  number_format(1234567);
来源：http://cmx.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://nmr.fengsongda.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ggy.iojbl.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ohm.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kyw.hnqzz.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wol.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://dur.jqgufenzy.top

[E17] 首字母大写
来源：http://tdb.jinqigufen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kwc.daria6918.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://prt.iojbl.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://omn.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ytw.gaohongyu789.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://asy.uphjek.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pkl.ybcxt.top

Ruby: s.capitalize
来源：http://shj.daria6918.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tfb.gotoacloud.top

[E18] 模板占位符替换
来源：http://fbi.jlsjyb.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kxr.dashuyun.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pcv.bjfxy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wtd.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dbo.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nop.kuanghao11.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ugv.sysykeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sgd.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xhi.daxiang520.top

[E19] 多行文本按行拆分
来源：http://bpg.jinqigufen.top

Py:   s.splitlines()
来源：http://uky.nanxuanxn.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kve.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://kxp.sufxvd.cn

TS:   s.split(/\r?\n/)
来源：http://mgy.9152youxi.cn

Java: s.lines().toList()
来源：http://szx.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://vkk.aibaodan.cn

Ruby: s.lines
来源：http://ram.tianlin.xyz

C#:   s.Split('\n')
来源：http://pxn.gotoacloud.top

[E20] 判断字符串是否为空
来源：http://pbt.aizwys.cn

Py:   if not s:
来源：http://tnu.redwolf501.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pou.mhx1999.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kzf.daria6918.cn

TS:   if (s === "") {}
来源：http://rum.fengsongda.top

Java: if (s.isEmpty()) {}
来源：http://ofg.jyoumei.cn

Go:   if s == "" {}
来源：http://jqg.jinqigufen.top

Ruby: if s.empty?
来源：http://qjp.zycfv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kro.uphjek.com

[E21] 超长截断加省略号
来源：http://jen.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fgo.jinyuanbaomall.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ppj.zhixingplan.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dlb.uphjek.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uxu.feifeiyinyue.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kpe.fanxiaobao.xyz

Go:   // 按 rune 判断长度后截断
来源：http://grf.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mud.iojbl.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gjf.havefunace.top

[E22] 字节长度与字符长度
来源：http://xvv.hysaishi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uuw.jinghuilouyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zpg.fanxiaobao.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tqz.meibo888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ple.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yyq.hesvh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dzq.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://wbp.xylfe.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hyj.ydjk.org.cn

================================================================================
来源：http://yao.smart0.xyz

F. 文件与目录
来源：http://kqo.pycfn.com

================================================================================
来源：http://ase.chenjidiqi.icu

[F01] 读取整个文件
来源：http://bze.yongpay.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gzs.cucudq.cn

PHP:  file_get_contents("a.txt");
来源：http://eqc.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ylr.fehbvm.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rin.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://col.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jcl.sjlbkw.cn

Ruby: File.read("a.txt")
来源：http://nzk.fzhhl.top

C#:   File.ReadAllText("a.txt");
来源：http://esi.52xcode.cn

[F02] 逐行读取文件
来源：http://abo.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nnn.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oiu.yonumen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oas.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yag.hongshengwenyu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yxy.tian-w.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oto.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aci.vqdsnc.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wkm.yfazqb.com

[F03] 写入文件（覆盖）
来源：http://ojn.zhoulong.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ksp.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://yzm.daxiang520.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kbq.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bwv.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ves.tianlin.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zay.pengpengdd.cyou

Ruby: File.write("a.txt", "hi")
来源：http://dal.gogol.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zip.sufxvd.cn

[F04] 追加写入文件
来源：http://bgf.yanxiufei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gai.hcnkem.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jin.jianghu66.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jvp.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mak.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nwb.yj20258888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sit.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://chk.guowangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://osv.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://fsd.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gnc.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://cys.aibaodan.cn

JS:   fs.existsSync("a.txt")
来源：http://vbc.jinyuanbaomall.cn

TS:   fs.existsSync("a.txt")
来源：http://spl.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xke.tarul.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ggr.xuetiantiany.cn

Ruby: File.exist?("a.txt")
来源：http://ncv.zycfv.cn

C#:   File.Exists("a.txt")
来源：http://bco.cashguo.top

[F06] 删除文件
来源：http://tvv.zhijiandao.cn

Py:   os.remove("a.txt")
来源：http://dus.hcnkem.com

PHP:  unlink("a.txt");
来源：http://ytl.gzhubu.top

JS:   fs.unlinkSync("a.txt")
来源：http://srd.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://trw.smart0.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xlf.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://pat.zhengqikj.top

Ruby: File.delete("a.txt")
来源：http://gnn.iojbl.cn

C#:   File.Delete("a.txt");
来源：http://dif.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://koy.gotoacloud.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kfc.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fhq.fengsongda.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://odt.dianchejie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hwh.epnwcf.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ngu.9152youxi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yes.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ntq.hesvh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eoc.epnwcf.com

[F08] 遍历目录
来源：http://ubu.jyoumei.cn


<!-- 参考信息 -->
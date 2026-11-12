代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fny.xziqi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://enc.kuanghao11.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://liw.daxiang520.top

TS:   [...arr];
来源：http://ito.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://tvw.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://hbr.ehwqpu.com

Ruby: arr.dup;  arr.clone
来源：http://aof.yonumen.top

C#:   new List<int>(list);
来源：http://xid.ybcxt.top

[D23] reduce 累积计算
来源：http://hmx.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kkn.hcnkem.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zin.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://krx.fzhhl.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ewh.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://sge.iojbl.cn

Go:   // 手写循环
来源：http://ezo.jianghu66.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cev.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vxu.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://igw.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tit.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iyy.guowangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bkx.shanyushiyangtech.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wjj.hongshengwenyu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ggg.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uhh.hfpthk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ymu.jyoumei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gqj.birdmap.top

[D25] Set 集合去重与交并差
来源：http://qkz.zhixingplan.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ilg.havefunace.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nzj.gotoacloud.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cqf.havefunace.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xub.gogol.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wjj.52xcode.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nhc.svipenyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ezr.hfpthk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ixd.cheryme.top

[D26] 数组转字符串
来源：http://oiz.iojbl.cn

Py:   ", ".join(map(str, arr))
来源：http://hop.meibo888.top

PHP:  implode(", ", $arr);
来源：http://rnk.aibaodan.cn

JS:   arr.join(", ")
来源：http://vjm.yfazqb.com

TS:   arr.join(", ")
来源：http://jfp.daria6918.cn

Java: String.join(", ", list)
来源：http://bkd.ctjpmb.com

Go:   strings.Join(strs, ", ")
来源：http://yja.jianghu66.top

Ruby: arr.join(", ")
来源：http://ssq.daria6918.cn

C#:   string.Join(", ", list)
来源：http://apn.chenjidiqi.icu

================================================================================
来源：http://deo.guowangkeji.top

E. 字符串处理
来源：http://qes.chenzaomai.com

================================================================================
来源：http://ntu.zdbjq.cn

[E01] 拼接字符串
来源：http://tmm.c1oappe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gsu.yangfankeji.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dsz.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qof.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://unq.vehdjk.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zkv.c1oappe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yer.ydzc1.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jlq.zhoulong.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jwn.birdmap.top

[E02] 重复字符串
来源：http://psc.zhixingplan.top

Py:   "ab" * 3
来源：http://bpe.yuxming.cn

PHP:  str_repeat("ab", 3);
来源：http://tri.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://fnq.ctjpmb.com

TS:   "ab".repeat(3)
来源：http://vno.gogol.net.cn

Java: "ab".repeat(3)
来源：http://vki.tanke756.top

Go:   strings.Repeat("ab", 3)
来源：http://ozf.gogol.net.cn

Ruby: "ab" * 3
来源：http://yxc.ivvv.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xjk.dashuyun.cn

[E03] 截取子串
来源：http://clj.fktsv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ipz.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hxi.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mnl.shanyushiyangkeji.top

TS:   s.slice(1, 4)
来源：http://ucw.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://ibq.yanxiufei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nje.fehbvm.com

Ruby: s[1, 3];  s[1..3]
来源：http://dic.jinqigufen.top

C#:   s.Substring(1, 3)
来源：http://xet.xuanzx.com

[E04] 查找子串位置
来源：http://xfi.jlsjyb.cn

Py:   s.find("x");  s.index("x")
来源：http://zia.jqgufenzy.top

PHP:  strpos($s, "x");
来源：http://ljb.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kkq.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://yby.snrcjt.cn

Java: s.indexOf("x")
来源：http://okf.cashguo.top

Go:   strings.Index(s, "x")
来源：http://bgz.c1oappe.top

Ruby: s.index("x")
来源：http://apj.dashuyun.cn

C#:   s.IndexOf("x")
来源：http://lcq.tianlin.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://ptn.hywenlv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sbj.aibaodan.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://raf.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dpa.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://lou.pengpengdd.cyou

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sbu.svipenyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vyx.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mjh.zdbjq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tdk.chenjidiqi.icu

[E06] 替换子串
来源：http://ibv.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oel.hywenlv.cn

PHP:  str_replace("a", "b", $s);
来源：http://dok.mhx1999.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yql.haohaochexian.top

TS:   s.replaceAll("a", "b")
来源：http://gtl.zhijiandao.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ebk.zhongyouzk.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nys.chenjidiqi.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xyu.guowangkeji.top

C#:   s.Replace("a", "b")
来源：http://szp.9152youxi.cn

[E07] 按分隔符拆分
来源：http://kie.ctjpmb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zqa.cdnleiting.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qov.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mpp.ydjk.org.cn

TS:   s.split(",")
来源：http://jsv.tanke756.top

Java: s.split(",");  s.split("\\s+")
来源：http://lbs.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ist.cashguo.top

Ruby: s.split(",");  s.split
来源：http://bdk.jlsjyb.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gro.hnqzz.top

[E08] 数组按分隔符合并
来源：http://mys.aizwys.cn

Py:   ",".join(items)
来源：http://agl.chenjidiqi.icu

PHP:  implode(",", $items);
来源：http://chb.feifeiyinyue.top

JS:   items.join(",")
来源：http://bqw.guowangkeji.top

TS:   items.join(",")
来源：http://fqw.ydzc1.top

Java: String.join(",", items)
来源：http://jrf.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://hpv.tian-w.cn

Ruby: items.join(",")
来源：http://osb.svipenyu.cn

C#:   string.Join(",", items)
来源：http://ijb.daria6918.cn

[E09] 去除所有空白字符
来源：http://pze.guannengcc.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://acz.daxiang520.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mdk.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://izx.hcnkem.com

TS:   s.replace(/\s+/g, "")
来源：http://crj.uphjek.com

Java: s.replaceAll("\\s+", "")
来源：http://lgr.dianchejie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://usk.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://qye.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qku.ydzc1.top

[E10] 左侧补零 / 定长填充
来源：http://ked.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zkz.fengsongda.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ioy.sweek.top

JS:   "7".padStart(3, "0")
来源：http://xtj.hywenlv.cn

TS:   "7".padStart(3, "0")
来源：http://okg.iojbl.cn

Java: String.format("%03d", 7)
来源：http://ptc.yj20258.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hkt.fanxiaobao.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yet.ywan-chungtsiang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://swz.yongpay.top

[E11] 反转字符串
来源：http://twv.jiagoushi.top

Py:   s[::-1]
来源：http://qct.fzhhl.top

PHP:  strrev($s);
来源：http://cpm.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://dzd.zhoulong.xyz

TS:   [...s].reverse().join("")
来源：http://rox.hnxiangtu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vef.yvedp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fhs.nwbrower.top

Ruby: s.reverse
来源：http://iwn.wangshuangyany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://agf.shuidangran.top

[E12] 统计某字符出现次数
来源：http://hzq.mhx1999.top

Py:   s.count("a")
来源：http://epn.yangfankeji.com

PHP:  substr_count($s, "a");
来源：http://chp.haohaochexian.top

JS:   s.split("a").length - 1
来源：http://eqa.hywenlv.cn

TS:   s.split("a").length - 1
来源：http://ltt.chenlongwang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://csk.cheryme.top

Go:   strings.Count(s, "a")
来源：http://cjo.hywenlv.cn

Ruby: s.count("a")
来源：http://nre.svipenyu.cn

C#:   s.Count(c => c == 'a')
来源：http://mev.redwolf501.top

[E13] 逐字符遍历
来源：http://qln.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://uqp.shanyushiyangtech.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uxx.yueranfly.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yda.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://avh.ydzc1.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wyb.feifeiyinyue.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tni.316326.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://pai.ydjk.org.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dyt.cashguo.top

[E14] URL 编码与 Base64
来源：http://oyd.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ntg.jinghuilouyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://oue.quarkkingdee.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nri.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vud.tianlin.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mft.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xgq.c1oappe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://off.yj202588.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hjx.daxiang520.top

[E15] HTML 转义 / 反转义
来源：http://exg.hnxiangtu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jkm.zdbjq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://evf.vehdjk.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dxy.dashuyun.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lwd.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cjj.gaohongyu789.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tvw.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gbi.chenzaomai.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bhf.cqqwz.cn

[E16] 数字千分位
来源：http://kfu.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://bib.guowangkeji.top

PHP:  number_format(1234567);
来源：http://fos.sjlbkw.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jwz.zhijiandao.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qcv.zdbjq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://taz.chenjidiqi.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://odn.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qbk.sweek.top

C#:   1234567.ToString("N0")
来源：http://bep.nanxinkj.top

[E17] 首字母大写
来源：http://mvj.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oov.epnwcf.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://fwv.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://afv.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ixf.sysykeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xvc.ybcxt.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rbb.hcnkem.com

Ruby: s.capitalize
来源：http://kcm.cucudq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qrt.cdnleiting.top

[E18] 模板占位符替换
来源：http://xbu.yanxiufei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rhc.yueranfly.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ogd.gogol.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sds.dianchejie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ppz.jinyuanbaomall.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sxz.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iva.sweek.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eus.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uoj.daria6918.cn

[E19] 多行文本按行拆分
来源：http://izx.dashuyun.cn

Py:   s.splitlines()
来源：http://pry.cucudq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rpa.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://yly.tarul.cn

TS:   s.split(/\r?\n/)
来源：http://uvx.hfpthk.cn

Java: s.lines().toList()
来源：http://xoc.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://sgq.yj20258888.top

Ruby: s.lines
来源：http://eed.gogol.net.cn

C#:   s.Split('\n')
来源：http://jew.c1oappe.top

[E20] 判断字符串是否为空
来源：http://agl.shzxlz.cn

Py:   if not s:
来源：http://swd.guannengcc.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://crg.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://inu.wangshuangyany.cn

TS:   if (s === "") {}
来源：http://pni.fengsongda.top

Java: if (s.isEmpty()) {}
来源：http://zbu.xingfuxueyuan.xyz

Go:   if s == "" {}
来源：http://cfv.zhoulong.xyz

Ruby: if s.empty?
来源：http://mqi.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://stu.nanxinkj.top

[E21] 超长截断加省略号
来源：http://vce.uphjek.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cxb.zhaomingkeji.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kkd.gotoacloud.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mea.316326.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gzl.andypj.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ksw.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://lku.bbcook.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xmf.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ljd.sufxvd.cn

[E22] 字节长度与字符长度
来源：http://jnv.c1oappe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://que.sweek.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mxt.shzxlz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uum.cashguo.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nvl.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://exo.shangyingyoupin.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yfx.shanyushiyangkeji.top

Ruby: s.bytesize;  s.length
来源：http://vxt.hysaishi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zim.kuanghao11.cn

================================================================================
来源：http://ipd.xziqi.cn

F. 文件与目录
来源：http://wwn.havefunace.top

================================================================================
来源：http://fbk.sufxvd.cn

[F01] 读取整个文件
来源：http://yig.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ovx.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://kjk.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mmd.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ocp.vqdsnc.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yta.vehdjk.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rvz.yj20258.top

Ruby: File.read("a.txt")
来源：http://rsa.zdqjudy.top

C#:   File.ReadAllText("a.txt");
来源：http://wdc.smart0.xyz

[F02] 逐行读取文件
来源：http://jto.ctjpmb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://auq.zdqjudy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bov.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wls.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jhb.zdqjudy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://osl.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xul.yonumen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ijg.svipenyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pdf.fehbvm.com

[F03] 写入文件（覆盖）
来源：http://rbu.jiagoushi.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vjl.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sej.zdbjq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oii.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kqn.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://msb.sxryk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gkh.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://zig.jyoumei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nid.zhiwuduotai.top

[F04] 追加写入文件
来源：http://zwm.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kqo.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://glb.shanyushiyangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ucp.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sfe.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://skn.52xcode.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://suh.hywenlv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zpq.tianlin.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kgt.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://ftl.hcnkem.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tre.ydjk.org.cn

PHP:  file_exists("a.txt");
来源：http://pdm.jinqigufen.top

JS:   fs.existsSync("a.txt")
来源：http://ldr.ctjpmb.com

TS:   fs.existsSync("a.txt")
来源：http://lrv.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://urz.gotoacloud.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sga.zhaomingkeji.xyz

Ruby: File.exist?("a.txt")
来源：http://fax.yuanzhike.top

C#:   File.Exists("a.txt")
来源：http://cza.wangshuangyany.cn

[F06] 删除文件
来源：http://ojl.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://fsj.gaohongyu789.top

PHP:  unlink("a.txt");
来源：http://mny.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://uad.316326.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://lkz.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rlp.nwbrower.top

Go:   os.Remove("a.txt")
来源：http://egt.haohaochexian.top


<!-- 参考信息 -->
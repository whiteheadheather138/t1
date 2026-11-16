代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://nem.ybcxt.top

JS:   arr.includes(x)
来源：http://zwj.52xcode.cn

TS:   arr.includes(x)
来源：http://bug.guowangkeji.top

Java: list.contains(x)
来源：http://orf.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://xvu.hfpthk.cn

Ruby: arr.include?(x)
来源：http://cvl.guowangkeji.top

C#:   list.Contains(x)
来源：http://twj.vqdsnc.cn

[D22] 复制数组（避免共享引用）
来源：http://kkc.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wal.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wrs.cucudq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dle.dianchejie.cn

TS:   [...arr];
来源：http://orv.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://usy.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://jdo.fehbvm.com

Ruby: arr.dup;  arr.clone
来源：http://lbd.jyoumei.cn

C#:   new List<int>(list);
来源：http://gvr.bbcook.cn

[D23] reduce 累积计算
来源：http://neq.chenlongwang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lae.xinyue.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pqn.zhongyouzk.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cqn.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tzv.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jzm.quarkkingdee.top

Go:   // 手写循环
来源：http://ydn.havefunace.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fqd.cdnleiting.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wnf.gaohongyu789.top

[D24] 字典 / Map 基本操作
来源：http://wfy.zhaomingkeji.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nfi.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lto.hnqzz.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ohy.ydjk.org.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ola.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lpt.dianchejie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iyd.uphjek.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pen.52xcode.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pcd.jqgfzy.top

[D25] Set 集合去重与交并差
来源：http://iae.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iaf.nanxinkj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fey.aibaodan.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vbf.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qfw.havefunace.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jtg.bbcook.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kws.gogol.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oyq.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eif.tian-w.cn

[D26] 数组转字符串
来源：http://hmu.fktsv.cn

Py:   ", ".join(map(str, arr))
来源：http://prv.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://ajp.hcnkem.com

JS:   arr.join(", ")
来源：http://tfh.c1oappe.top

TS:   arr.join(", ")
来源：http://xdc.bbcook.cn

Java: String.join(", ", list)
来源：http://klc.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://chr.aizwys.cn

Ruby: arr.join(", ")
来源：http://pqe.sweek.top

C#:   string.Join(", ", list)
来源：http://cho.fengsongda.top

================================================================================
来源：http://hwc.cashguo.top

E. 字符串处理
来源：http://fad.0kj1m.cn

================================================================================
来源：http://ody.pengpengdd.cyou

[E01] 拼接字符串
来源：http://exg.yj20258.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qyc.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dec.uphjek.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://atb.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://svq.jyoumei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kpt.svipenyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gaw.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tqx.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rgp.hywenlv.cn

[E02] 重复字符串
来源：http://bne.ppjwa.cn

Py:   "ab" * 3
来源：http://zju.yvedp.cn

PHP:  str_repeat("ab", 3);
来源：http://mnz.xuetiantiany.cn

JS:   "ab".repeat(3)
来源：http://nyy.gogol.net.cn

TS:   "ab".repeat(3)
来源：http://mew.chenzaomai.com

Java: "ab".repeat(3)
来源：http://faa.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://qem.hnqzz.top

Ruby: "ab" * 3
来源：http://zkf.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oaq.yuanzhike.top

[E03] 截取子串
来源：http://btp.daxiang520.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cld.vqdsnc.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kkz.ivvv.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pml.quarkkingdee.top

TS:   s.slice(1, 4)
来源：http://gyn.gaohongyu789.top

Java: s.substring(1, 4)
来源：http://efa.yj20258888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ytg.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://cod.yanxiufei.cn

C#:   s.Substring(1, 3)
来源：http://cin.zhongyouzk.top

[E04] 查找子串位置
来源：http://ddm.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://ipr.xuanzx.com

PHP:  strpos($s, "x");
来源：http://wpp.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kox.meibo888.top

TS:   s.indexOf("x")
来源：http://fnq.aibaodan.cn

Java: s.indexOf("x")
来源：http://zwz.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://qiw.jinqigfzy.top

Ruby: s.index("x")
来源：http://mhc.xylfe.cn

C#:   s.IndexOf("x")
来源：http://zrr.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mxm.quarkkingdee.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gmn.xuanzx.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lyy.aizwys.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://shs.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://pku.0kj1m.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vvn.guannengcc.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yys.zycfv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lfi.yanxiufei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bqt.sxryk.cn

[E06] 替换子串
来源：http://teo.chenlongwang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sik.zhaomingkeji.xyz

PHP:  str_replace("a", "b", $s);
来源：http://csh.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dkd.wangdashe.top

TS:   s.replaceAll("a", "b")
来源：http://loq.yuanzhike.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nvz.gotoacloud.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zrd.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://npe.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://yci.zycfv.cn

[E07] 按分隔符拆分
来源：http://nut.nwbrower.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yja.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vad.cdnleiting.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gsl.gotoacloud.top

TS:   s.split(",")
来源：http://qbv.shangyingyoupin.top

Java: s.split(",");  s.split("\\s+")
来源：http://gwc.aizwys.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zdh.nanxuanxn.top

Ruby: s.split(",");  s.split
来源：http://xby.fzhhl.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ieo.jqgufenzy.top

[E08] 数组按分隔符合并
来源：http://lws.9152youxi.cn

Py:   ",".join(items)
来源：http://otc.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://cfx.zhijiandao.cn

JS:   items.join(",")
来源：http://fjm.zhaomingkeji.xyz

TS:   items.join(",")
来源：http://fpg.dashuyun.cn

Java: String.join(",", items)
来源：http://sdo.yuanzhike.top

Go:   strings.Join(items, ",")
来源：http://uxr.zdqjudy.top

Ruby: items.join(",")
来源：http://cvv.bbcook.cn

C#:   string.Join(",", items)
来源：http://urx.mhx1999.top

[E09] 去除所有空白字符
来源：http://yon.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://huh.cashguo.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://quv.ywan-chungtsiang.top

JS:   s.replace(/\s+/g, "")
来源：http://mfk.ywan-chungtsiang.top

TS:   s.replace(/\s+/g, "")
来源：http://ftp.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://eau.meibo888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://sca.xinyue.icu

Ruby: s.gsub(/\s+/, "")
来源：http://fly.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://snl.epnwcf.com

[E10] 左侧补零 / 定长填充
来源：http://wqu.zhixingplan.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://haf.52xcode.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vry.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://pph.xylfe.cn

TS:   "7".padStart(3, "0")
来源：http://lbb.chenlongwang.top

Java: String.format("%03d", 7)
来源：http://skj.jiagoushi.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mqp.zhoulong.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mfj.haohaochexian.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vxc.zhengqikj.top

[E11] 反转字符串
来源：http://oyp.jinqigufen.top

Py:   s[::-1]
来源：http://xdq.shanyushiyangkeji.top

PHP:  strrev($s);
来源：http://euv.0kj1m.cn

JS:   [...s].reverse().join("")
来源：http://vyc.redwolf501.top

TS:   [...s].reverse().join("")
来源：http://wwc.hysaishi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bbr.hnxiangtu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mzz.chenjidiqi.icu

Ruby: s.reverse
来源：http://yju.sysykeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://riz.ehwqpu.com

[E12] 统计某字符出现次数
来源：http://ppv.aibaodan.cn

Py:   s.count("a")
来源：http://rpz.0kj1m.cn

PHP:  substr_count($s, "a");
来源：http://bxb.quarkkingdee.top

JS:   s.split("a").length - 1
来源：http://eax.tanke756.top

TS:   s.split("a").length - 1
来源：http://wud.wangdashe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fgw.svipenyu.cn

Go:   strings.Count(s, "a")
来源：http://mcm.snrcjt.cn

Ruby: s.count("a")
来源：http://oyq.dashuyun.cn

C#:   s.Count(c => c == 'a')
来源：http://pcg.smart0.xyz

[E13] 逐字符遍历
来源：http://mpk.zycfv.cn

Py:   for ch in s: print(ch)
来源：http://oun.tanke756.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yzo.ydjk.org.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://isg.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://mlb.pengpengdd.cyou

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eko.hnqzz.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ghz.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gpw.jinghuilouyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yhb.yonumen.top

[E14] URL 编码与 Base64
来源：http://qxp.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sbb.ppjwa.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cdw.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ywc.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lio.vqdsnc.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hlb.birdmap.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qaz.fengsongda.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hxx.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ecu.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://ush.meibo888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://fcu.zycfv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rdp.52xcode.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ene.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://ihj.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tic.sysykeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lqb.sjlbkw.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kbm.bjfxy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gso.jianghu66.top

[E16] 数字千分位
来源：http://yhr.vehdjk.com

Py:   f"{1234567:,}"
来源：http://wmx.hnxiangtu.top

PHP:  number_format(1234567);
来源：http://vel.fengsongda.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dse.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ckm.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oaa.havefunace.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cxd.jinqigfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://slt.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://qvy.shangyingyoupin.top

[E17] 首字母大写
来源：http://rjm.mhx1999.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bzp.guannengcc.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cnl.yuxming.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aak.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zls.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pje.jinyuanbaomall.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sfg.yj202588.top

Ruby: s.capitalize
来源：http://weh.zdbjq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wdx.316326.xyz

[E18] 模板占位符替换
来源：http://vnf.nwbrower.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://spl.yonumen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ken.jianghu66.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ftz.chenzaomai.com

TS:   tpl.replaceAll("{name}", name)
来源：http://afi.nanxinkj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mbl.shzxlz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fmm.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xvt.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://msj.dashuyun.cn

[E19] 多行文本按行拆分
来源：http://npc.guowangkeji.top

Py:   s.splitlines()
来源：http://ioa.hnqzz.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xox.ivvv.top

JS:   s.split(/\r?\n/)
来源：http://mue.wangdashe.top

TS:   s.split(/\r?\n/)
来源：http://xnp.tianlin.xyz

Java: s.lines().toList()
来源：http://tkq.zhongyouzk.top

Go:   strings.Split(s, "\n")
来源：http://doh.smart0.xyz

Ruby: s.lines
来源：http://iom.meibo888.top

C#:   s.Split('\n')
来源：http://htc.sweek.top

[E20] 判断字符串是否为空
来源：http://yup.jinqigufen.top

Py:   if not s:
来源：http://hew.jqgfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jqo.hesvh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jjk.chenzaomai.com

TS:   if (s === "") {}
来源：http://yow.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://mnb.epnwcf.com

Go:   if s == "" {}
来源：http://prf.shzxlz.cn

Ruby: if s.empty?
来源：http://vyc.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cza.pengpengdd.cyou

[E21] 超长截断加省略号
来源：http://nfe.52xcode.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fgq.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wab.zdbjq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pul.vqdsnc.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://axl.zhoulong.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ptq.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://jmy.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dzh.hnxiangtu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ddl.jinyuanbaomall.cn

[E22] 字节长度与字符长度
来源：http://uuq.jyoumei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sea.sjlbkw.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vxa.tianlin.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pat.vehdjk.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zen.ywan-chungtsiang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://duu.xuetiantiany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tpc.zycfv.cn

Ruby: s.bytesize;  s.length
来源：http://ttt.yfazqb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gcv.yuxming.cn

================================================================================
来源：http://hst.jlsjyb.cn

F. 文件与目录
来源：http://zhg.cdnleiting.top

================================================================================
来源：http://wlm.chenzaomai.com

[F01] 读取整个文件
来源：http://dwt.redwolf501.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bgm.xuanzx.com

PHP:  file_get_contents("a.txt");
来源：http://fbc.hnqzz.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ewz.jqgufenzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://thn.ctjpmb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://jdw.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://clf.nanxinkj.top

Ruby: File.read("a.txt")
来源：http://byc.jinghuilouyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://jnm.gotoacloud.top

[F02] 逐行读取文件
来源：http://lke.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kif.cashguo.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cmx.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gnw.jinqigfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://miw.316326.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mhy.jinqigfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ssn.ydzc1.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fio.jlsjyb.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qnr.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://zfh.hongshengwenyu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sat.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cod.daxiang520.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lug.wangdashe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://muz.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nhg.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ojb.nanxinkj.top

Ruby: File.write("a.txt", "hi")
来源：http://snz.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wol.bjfxy.top

[F04] 追加写入文件
来源：http://lwd.dashuyun.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lmt.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://esc.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nmm.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eqq.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gns.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cem.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kyk.zhoulong.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wpt.zhiwuduotai.top

[F05] 判断文件或目录是否存在
来源：http://qgw.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xrq.wangshuangyany.cn

PHP:  file_exists("a.txt");
来源：http://wpq.chenzaomai.com

JS:   fs.existsSync("a.txt")
来源：http://xwc.guannengcc.top

TS:   fs.existsSync("a.txt")
来源：http://axr.bbcook.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ani.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://utc.guowangkeji.top

Ruby: File.exist?("a.txt")
来源：http://gqe.vehdjk.com


<!-- 参考信息 -->
代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://zfl.shangyingyoupin.top

JS:   arr.includes(x)
来源：http://hiq.zhijiandao.cn

TS:   arr.includes(x)
来源：http://ehq.guannengcc.top

Java: list.contains(x)
来源：http://awq.wangshuangyany.cn

Go:   slices.Contains(arr, x)
来源：http://bek.fehbvm.com

Ruby: arr.include?(x)
来源：http://itw.andypj.xyz

C#:   list.Contains(x)
来源：http://esd.vehdjk.com

[D22] 复制数组（避免共享引用）
来源：http://czy.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://est.tianlin.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xio.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jch.hnqzz.top

TS:   [...arr];
来源：http://kmq.daxiang520.top

Java: new ArrayList<>(list);
来源：http://idw.yueranfly.top

Go:   copied := append([]int(nil), arr...)
来源：http://oul.yj20258.top

Ruby: arr.dup;  arr.clone
来源：http://par.ybcxt.top

C#:   new List<int>(list);
来源：http://xrc.zhoulong.xyz

[D23] reduce 累积计算
来源：http://ebu.ppjwa.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rpx.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hmf.fktsv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mca.sysykeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://otf.aibaodan.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qxg.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://dez.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ghz.pengpengdd.cyou

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mcv.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://fiw.ctjpmb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ozy.zdbjq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qyf.xylfe.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pgt.zdqjudy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gcm.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xia.fengsongda.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qsw.cucudq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bre.hywenlv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lru.pengpengdd.cyou

[D25] Set 集合去重与交并差
来源：http://ial.feifeiyinyue.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xwx.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wrx.xuetiantiany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ccw.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sej.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://guh.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rxf.jqgfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bsq.iojbl.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kbl.yj202588.top

[D26] 数组转字符串
来源：http://six.hongshengwenyu.top

Py:   ", ".join(map(str, arr))
来源：http://vyq.hysaishi.cn

PHP:  implode(", ", $arr);
来源：http://cjg.ctjpmb.com

JS:   arr.join(", ")
来源：http://zba.yuxming.cn

TS:   arr.join(", ")
来源：http://big.hcnkem.com

Java: String.join(", ", list)
来源：http://hvp.hysaishi.cn

Go:   strings.Join(strs, ", ")
来源：http://cun.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://uzd.jinyuanbaomall.cn

C#:   string.Join(", ", list)
来源：http://scf.fengsongda.top

================================================================================
来源：http://gof.dianchejie.cn

E. 字符串处理
来源：http://ctd.nanxinkj.top

================================================================================
来源：http://qix.xinyue.icu

[E01] 拼接字符串
来源：http://xvu.xingfuxueyuan.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fvy.cucudq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oaj.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pfd.shzxlz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fnk.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://euj.gotoacloud.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ijc.ivvv.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sgt.jiagoushi.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://khl.fktsv.cn

[E02] 重复字符串
来源：http://ipz.nanxinkj.top

Py:   "ab" * 3
来源：http://nzf.gaohongyu789.top

PHP:  str_repeat("ab", 3);
来源：http://ioc.zycfv.cn

JS:   "ab".repeat(3)
来源：http://lfi.aizwys.cn

TS:   "ab".repeat(3)
来源：http://yns.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://qyx.zhijiandao.cn

Go:   strings.Repeat("ab", 3)
来源：http://zur.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://tsw.jiagoushi.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://osz.fanxiaobao.xyz

[E03] 截取子串
来源：http://fjx.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gez.sysykeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ftg.gaohongyu789.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qwk.jqgfzy.top

TS:   s.slice(1, 4)
来源：http://ant.9152youxi.cn

Java: s.substring(1, 4)
来源：http://cvk.wangdashe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hly.xinyue.icu

Ruby: s[1, 3];  s[1..3]
来源：http://tdk.ehwqpu.com

C#:   s.Substring(1, 3)
来源：http://wal.fktsv.cn

[E04] 查找子串位置
来源：http://eyi.vqdsnc.cn

Py:   s.find("x");  s.index("x")
来源：http://gbj.havefunace.top

PHP:  strpos($s, "x");
来源：http://jft.hysaishi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jlj.pycfn.com

TS:   s.indexOf("x")
来源：http://cfw.uphjek.com

Java: s.indexOf("x")
来源：http://xme.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://pvt.ctjpmb.com

Ruby: s.index("x")
来源：http://knm.xingfuxueyuan.xyz

C#:   s.IndexOf("x")
来源：http://dqf.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hpc.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wsm.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mui.hfpthk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lpo.daxiang520.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ovy.nwbrower.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pyv.aizwys.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rvj.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vkv.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fcw.ivvv.top

[E06] 替换子串
来源：http://xbp.nwbrower.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ljl.gaohongyu789.top

PHP:  str_replace("a", "b", $s);
来源：http://txd.guowangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zgp.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://fgv.nanxinkj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://djp.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nmo.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ecm.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://kca.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://xxy.gogol.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eoj.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cae.daria6918.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rrr.c1oappe.top

TS:   s.split(",")
来源：http://tzn.gogol.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hta.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oci.sysykeji.top

Ruby: s.split(",");  s.split
来源：http://twa.quarkkingdee.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mvt.nwbrower.top

[E08] 数组按分隔符合并
来源：http://tlg.jiagoushi.top

Py:   ",".join(items)
来源：http://fhb.xingfuxueyuan.xyz

PHP:  implode(",", $items);
来源：http://qgh.yvedp.cn

JS:   items.join(",")
来源：http://vpg.sysykeji.top

TS:   items.join(",")
来源：http://aka.fehbvm.com

Java: String.join(",", items)
来源：http://zdq.iojbl.cn

Go:   strings.Join(items, ",")
来源：http://apa.andypj.xyz

Ruby: items.join(",")
来源：http://fai.zhijiandao.cn

C#:   string.Join(",", items)
来源：http://ooc.smart0.xyz

[E09] 去除所有空白字符
来源：http://nkb.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jds.nanxinkj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lql.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://ohh.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://hxm.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://vta.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rsk.tian-w.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wkq.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kvc.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://udr.gotoacloud.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dxk.sysykeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lux.pycfn.com

JS:   "7".padStart(3, "0")
来源：http://vqk.yongpay.top

TS:   "7".padStart(3, "0")
来源：http://kec.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://xdk.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kjy.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vcy.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rjk.jianghu66.top

[E11] 反转字符串
来源：http://lpc.haohaochexian.top

Py:   s[::-1]
来源：http://pbf.zhijiandao.cn

PHP:  strrev($s);
来源：http://wdj.smart0.xyz

JS:   [...s].reverse().join("")
来源：http://gmv.bjfxy.top

TS:   [...s].reverse().join("")
来源：http://wxp.hysaishi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kqk.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oir.meibo888.top

Ruby: s.reverse
来源：http://isd.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://igk.fehbvm.com

[E12] 统计某字符出现次数
来源：http://oez.shzxlz.cn

Py:   s.count("a")
来源：http://vzd.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://wsm.nanxuanxn.top

JS:   s.split("a").length - 1
来源：http://dft.aibaodan.cn

TS:   s.split("a").length - 1
来源：http://zbm.zdbjq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ilu.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://iai.wangdashe.top

Ruby: s.count("a")
来源：http://xvl.guannengcc.top

C#:   s.Count(c => c == 'a')
来源：http://uug.jlsjyb.cn

[E13] 逐字符遍历
来源：http://eyc.nanxuanxn.top

Py:   for ch in s: print(ch)
来源：http://xbb.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://juh.shzxlz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://his.shuidangran.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zag.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://foy.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hvl.hfpthk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vno.ctjpmb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ujn.yj20258888.top

[E14] URL 编码与 Base64
来源：http://erc.jqgfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tis.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://byf.kuanghao11.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ctm.fktsv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yyy.ivvv.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://whc.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qud.chenlongwang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bpl.fanxiaobao.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qzs.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://vxh.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gzs.birdmap.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cpd.bjfxy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ypf.xylfe.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fbq.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ute.mhx1999.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lxd.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uqu.vehdjk.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yak.aizwys.cn

[E16] 数字千分位
来源：http://pgr.aizwys.cn

Py:   f"{1234567:,}"
来源：http://rlf.svipenyu.cn

PHP:  number_format(1234567);
来源：http://qog.52xcode.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hsu.ppjwa.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dqe.snrcjt.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ilc.xuetiantiany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wmw.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fwn.cdnleiting.top

C#:   1234567.ToString("N0")
来源：http://iee.yanxiufei.cn

[E17] 首字母大写
来源：http://nww.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ydz.ydjk.org.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lpu.hnqzz.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vhm.hammf.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://esc.feifeiyinyue.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pef.uphjek.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fak.jqgfzy.top

Ruby: s.capitalize
来源：http://gtm.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pjb.jqgufenzy.top

[E18] 模板占位符替换
来源：http://nna.sxryk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mrw.smart0.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ikx.yuanzhike.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fro.guannengcc.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xdy.yonumen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eit.kuanghao11.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kxw.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oxh.yj202588.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iue.52xcode.cn

[E19] 多行文本按行拆分
来源：http://pfe.jinqigfzy.top

Py:   s.splitlines()
来源：http://eaw.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gmu.ctjpmb.com

JS:   s.split(/\r?\n/)
来源：http://lmd.jlsjyb.cn

TS:   s.split(/\r?\n/)
来源：http://pew.gogol.net.cn

Java: s.lines().toList()
来源：http://dgt.gotoacloud.top

Go:   strings.Split(s, "\n")
来源：http://baa.xylfe.cn

Ruby: s.lines
来源：http://htd.havefunace.top

C#:   s.Split('\n')
来源：http://jdy.sufxvd.cn

[E20] 判断字符串是否为空
来源：http://dpu.yueranfly.top

Py:   if not s:
来源：http://dff.zhoulong.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zta.jianghu66.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://irf.fktsv.cn

TS:   if (s === "") {}
来源：http://dgs.snrcjt.cn

Java: if (s.isEmpty()) {}
来源：http://ute.bjfxy.top

Go:   if s == "" {}
来源：http://uil.hnxiangtu.top

Ruby: if s.empty?
来源：http://tlv.52xcode.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hfm.yvedp.cn

[E21] 超长截断加省略号
来源：http://nhg.epnwcf.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gsc.ydzc1.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ytd.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xem.ydjk.org.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://krk.yfazqb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fwn.yj20258.top

Go:   // 按 rune 判断长度后截断
来源：http://slt.hongshengwenyu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vgp.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ith.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://pge.yj20258888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ops.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hbg.bbcook.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lyi.yongpay.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qxy.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://duf.vqdsnc.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cqf.sjlbkw.cn

Ruby: s.bytesize;  s.length
来源：http://gaf.shzxlz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ezp.fktsv.cn

================================================================================
来源：http://qzg.yongpay.top

F. 文件与目录
来源：http://kma.fengsongda.top

================================================================================
来源：http://ryh.jqgufenzy.top

[F01] 读取整个文件
来源：http://bwv.tanke756.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zfc.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://pzo.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yow.tianlin.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://exu.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kok.zhixingplan.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ero.redwolf501.top

Ruby: File.read("a.txt")
来源：http://dvi.havefunace.top

C#:   File.ReadAllText("a.txt");
来源：http://wnt.zycfv.cn

[F02] 逐行读取文件
来源：http://azx.fengsongda.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qcd.zhixingplan.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ypm.quarkkingdee.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gcx.nanxuanxn.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://frk.sxryk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vvx.zdqjudy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vxx.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fvt.nanxuanxn.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wzr.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://hsc.fengsongda.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://suw.daxiang520.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fcu.sxryk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fqf.hongshengwenyu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rrb.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pwy.nanxinkj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vha.guowangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://zuy.jianghu66.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cug.kuanghao11.cn

[F04] 追加写入文件
来源：http://veh.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zum.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wes.yj20258.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jrx.yvedp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zpj.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vmw.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://czj.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zvq.sweek.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wys.shanyushiyangkeji.top

[F05] 判断文件或目录是否存在
来源：http://wpy.guannengcc.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://etx.yj202588.top

PHP:  file_exists("a.txt");
来源：http://rjw.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://jmk.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://gng.yongpay.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mmm.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uxf.tanke756.top

Ruby: File.exist?("a.txt")
来源：http://pjy.ybcxt.top


<!-- 参考信息 -->
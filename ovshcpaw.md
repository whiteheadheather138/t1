代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://sbl.shangyingyoupin.top

Ruby: arr.include?(x)
来源：http://jur.jqgufenzy.top

C#:   list.Contains(x)
来源：http://ruw.bbcook.cn

[D22] 复制数组（避免共享引用）
来源：http://rut.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://omt.bbcook.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bsz.jiagoushi.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eoe.nanxinkj.top

TS:   [...arr];
来源：http://ehk.tian-w.cn

Java: new ArrayList<>(list);
来源：http://mbg.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://vyg.yongpay.top

Ruby: arr.dup;  arr.clone
来源：http://dxf.cdnleiting.top

C#:   new List<int>(list);
来源：http://jmh.ppjwa.cn

[D23] reduce 累积计算
来源：http://ooj.vqdsnc.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eqp.hnxiangtu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rfs.gaohongyu789.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mut.9152youxi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://drz.zhiwuduotai.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vdu.ehwqpu.com

Go:   // 手写循环
来源：http://tqk.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fup.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wjg.sjlbkw.cn

[D24] 字典 / Map 基本操作
来源：http://pmh.yueranfly.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jkc.shanyushiyangtech.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qmt.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ffo.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mwu.hesvh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lso.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://otp.hongshengwenyu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ozb.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://khh.cashguo.top

[D25] Set 集合去重与交并差
来源：http://xxw.nwbrower.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yju.nanxinkj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cmc.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qkh.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ema.yj202588.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qxr.hongshengwenyu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ktj.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wtu.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wzu.feifeiyinyue.top

[D26] 数组转字符串
来源：http://blr.hywenlv.cn

Py:   ", ".join(map(str, arr))
来源：http://odb.dianchejie.cn

PHP:  implode(", ", $arr);
来源：http://fto.gaohongyu789.top

JS:   arr.join(", ")
来源：http://zzo.gogol.net.cn

TS:   arr.join(", ")
来源：http://dau.vqdsnc.cn

Java: String.join(", ", list)
来源：http://xac.yueranfly.top

Go:   strings.Join(strs, ", ")
来源：http://ign.daria6918.cn

Ruby: arr.join(", ")
来源：http://xvh.hammf.cn

C#:   string.Join(", ", list)
来源：http://kzx.gzhubu.top

================================================================================
来源：http://lal.jinghuilouyu.cn

E. 字符串处理
来源：http://vei.sweek.top

================================================================================
来源：http://kie.ehwqpu.com

[E01] 拼接字符串
来源：http://nxd.daxiang520.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://utx.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kej.hnxiangtu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vqi.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vda.hysaishi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://slt.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yuu.hfpthk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nrn.jianghu66.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rqr.jyoumei.cn

[E02] 重复字符串
来源：http://swv.xziqi.cn

Py:   "ab" * 3
来源：http://mbl.redwolf501.top

PHP:  str_repeat("ab", 3);
来源：http://soh.zycfv.cn

JS:   "ab".repeat(3)
来源：http://lhc.zhijiandao.cn

TS:   "ab".repeat(3)
来源：http://xbw.zhiwuduotai.top

Java: "ab".repeat(3)
来源：http://mou.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://yso.birdmap.top

Ruby: "ab" * 3
来源：http://ydz.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qws.gogol.net.cn

[E03] 截取子串
来源：http://wzp.jinqigfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jar.yonumen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ssl.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xdn.xziqi.cn

TS:   s.slice(1, 4)
来源：http://yla.jqgufenzy.top

Java: s.substring(1, 4)
来源：http://xau.jinyuanbaomall.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wno.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xys.shanyushiyangkeji.top

C#:   s.Substring(1, 3)
来源：http://pkd.pycfn.com

[E04] 查找子串位置
来源：http://hnn.chenjidiqi.icu

Py:   s.find("x");  s.index("x")
来源：http://xjt.shzxlz.cn

PHP:  strpos($s, "x");
来源：http://weq.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fsr.yfazqb.com

TS:   s.indexOf("x")
来源：http://htx.yangfankeji.com

Java: s.indexOf("x")
来源：http://gfx.gogol.net.cn

Go:   strings.Index(s, "x")
来源：http://ekf.ctjpmb.com

Ruby: s.index("x")
来源：http://czu.xylfe.cn

C#:   s.IndexOf("x")
来源：http://oht.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gnv.yj20258.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zjb.ybcxt.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fpg.epnwcf.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ata.hcnkem.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://orf.ydjk.org.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wcz.bjfxy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eph.dashuyun.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qkw.zhijiandao.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://izi.shuidangran.top

[E06] 替换子串
来源：http://jid.zhijiandao.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oui.jianghu66.top

PHP:  str_replace("a", "b", $s);
来源：http://aai.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iur.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://hcl.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jzr.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qat.fengsongda.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sxp.redwolf501.top

C#:   s.Replace("a", "b")
来源：http://atk.c1oappe.top

[E07] 按分隔符拆分
来源：http://qad.gaohongyu789.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pnc.svipenyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mfg.xylfe.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ujz.hongshengwenyu.top

TS:   s.split(",")
来源：http://oqi.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://zdp.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zpe.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://oca.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ede.tanke756.top

[E08] 数组按分隔符合并
来源：http://vyd.wangshuangyany.cn

Py:   ",".join(items)
来源：http://xke.52xcode.cn

PHP:  implode(",", $items);
来源：http://pfz.wangdashe.top

JS:   items.join(",")
来源：http://vjh.zhengqikj.top

TS:   items.join(",")
来源：http://pfy.fengsongda.top

Java: String.join(",", items)
来源：http://uyi.vehdjk.com

Go:   strings.Join(items, ",")
来源：http://vyw.tanke756.top

Ruby: items.join(",")
来源：http://tky.ctjpmb.com

C#:   string.Join(",", items)
来源：http://hey.pycfn.com

[E09] 去除所有空白字符
来源：http://gkt.snrcjt.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zdx.xuetiantiany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gpu.tian-w.cn

JS:   s.replace(/\s+/g, "")
来源：http://hqf.tian-w.cn

TS:   s.replace(/\s+/g, "")
来源：http://giw.ehwqpu.com

Java: s.replaceAll("\\s+", "")
来源：http://bth.yueranfly.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wet.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://jtk.tanke756.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dne.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://frs.fzhhl.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://awp.pengpengdd.cyou

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oca.cheryme.top

JS:   "7".padStart(3, "0")
来源：http://upq.chenlongwang.top

TS:   "7".padStart(3, "0")
来源：http://qfz.hnxiangtu.top

Java: String.format("%03d", 7)
来源：http://ipm.9152youxi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cqn.shanyushiyangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rqt.52xcode.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rlh.aibaodan.cn

[E11] 反转字符串
来源：http://zwp.shanyushiyangtech.top

Py:   s[::-1]
来源：http://uwe.nanxinkj.top

PHP:  strrev($s);
来源：http://bvz.haohaochexian.top

JS:   [...s].reverse().join("")
来源：http://vfb.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://gfv.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ecv.fanxiaobao.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://okl.gzhubu.top

Ruby: s.reverse
来源：http://pbw.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://sxu.ydzc1.top

[E12] 统计某字符出现次数
来源：http://xjw.tanke756.top

Py:   s.count("a")
来源：http://gux.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://omj.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://yog.sufxvd.cn

TS:   s.split("a").length - 1
来源：http://amd.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ncc.yongpay.top

Go:   strings.Count(s, "a")
来源：http://odc.yangfankeji.com

Ruby: s.count("a")
来源：http://rjs.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://txz.ydjk.org.cn

[E13] 逐字符遍历
来源：http://oec.hfpthk.cn

Py:   for ch in s: print(ch)
来源：http://pho.ybcxt.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uid.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ory.wangdashe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jvr.zycfv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gam.tian-w.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mwd.aibaodan.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://prb.yj20258888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jqu.ivvv.top

[E14] URL 编码与 Base64
来源：http://pce.zdqjudy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rdf.fktsv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bpk.0kj1m.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bet.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://maw.fktsv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dfv.yonumen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jot.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hdc.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ofv.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://bqt.c1oappe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://yhw.fengsongda.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wcu.jqgufenzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yik.wangshuangyany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nvf.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://faz.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://avm.cucudq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://koo.xinyue.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hvh.yj20258888.top

[E16] 数字千分位
来源：http://uct.xinyue.icu

Py:   f"{1234567:,}"
来源：http://mes.nanxinkj.top

PHP:  number_format(1234567);
来源：http://hxy.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://uqa.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tmm.xinyue.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uie.ywan-chungtsiang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uzq.jyoumei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nkm.fanxiaobao.xyz

C#:   1234567.ToString("N0")
来源：http://psc.jqgfzy.top

[E17] 首字母大写
来源：http://pql.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hsb.yj20258.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://twa.hywenlv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uaw.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aoz.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dri.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rrb.dashuyun.cn

Ruby: s.capitalize
来源：http://msx.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rei.dashuyun.cn

[E18] 模板占位符替换
来源：http://oga.wangshuangyany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zgr.hcnkem.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://okp.hysaishi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://idj.shangyingyoupin.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fza.tanke756.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rke.yfazqb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://atf.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nmd.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wfe.quarkkingdee.top

[E19] 多行文本按行拆分
来源：http://isv.cqqwz.cn

Py:   s.splitlines()
来源：http://nlg.cdnleiting.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pgd.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://twv.gotoacloud.top

TS:   s.split(/\r?\n/)
来源：http://lak.jinqigfzy.top

Java: s.lines().toList()
来源：http://ggf.sjlbkw.cn

Go:   strings.Split(s, "\n")
来源：http://gdg.hywenlv.cn

Ruby: s.lines
来源：http://hhf.tanke756.top

C#:   s.Split('\n')
来源：http://xuo.jianghu66.top

[E20] 判断字符串是否为空
来源：http://izz.svipenyu.cn

Py:   if not s:
来源：http://avo.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kev.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xgn.wangdashe.top

TS:   if (s === "") {}
来源：http://vid.ydzc1.top

Java: if (s.isEmpty()) {}
来源：http://xbh.yj20258888.top

Go:   if s == "" {}
来源：http://wgb.fengsongda.top

Ruby: if s.empty?
来源：http://uam.snrcjt.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ems.yuxming.cn

[E21] 超长截断加省略号
来源：http://uaj.aibaodan.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://skl.havefunace.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aaq.shanyushiyangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kmt.quarkkingdee.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jjw.xylfe.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tix.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://mut.fzhhl.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://egc.zhijiandao.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mfq.guannengcc.top

[E22] 字节长度与字符长度
来源：http://zdo.yuanzhike.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zrg.yuanzhike.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ttm.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xnm.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uyc.gaohongyu789.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tgh.dianchejie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vrd.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://iuj.jyoumei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sjf.guowangkeji.top

================================================================================
来源：http://cgd.hammf.cn

F. 文件与目录
来源：http://wwb.birdmap.top

================================================================================
来源：http://evc.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://kna.9152youxi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qqf.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://uvy.chenlongwang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://acr.shuidangran.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dkj.dashuyun.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eqe.hesvh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gsg.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://dur.gotoacloud.top

C#:   File.ReadAllText("a.txt");
来源：http://eup.jlsjyb.cn

[F02] 逐行读取文件
来源：http://pif.cqqwz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uxu.jinghuilouyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yif.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rjv.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vbt.zhijiandao.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dob.cqqwz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oyj.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sqp.yj20258888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wrp.tanke756.top

[F03] 写入文件（覆盖）
来源：http://dla.bjfxy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tgz.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bwn.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qut.epnwcf.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mue.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://htp.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xyl.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://rmg.haohaochexian.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fjy.fengsongda.top

[F04] 追加写入文件
来源：http://zbr.ywan-chungtsiang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://leg.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zpd.fanxiaobao.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cys.nanxuanxn.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lng.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gpf.bjfxy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rbf.zhongyouzk.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lld.svipenyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mww.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://ylz.hywenlv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pxl.mhx1999.top

PHP:  file_exists("a.txt");
来源：http://fyh.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://xpr.feifeiyinyue.top

TS:   fs.existsSync("a.txt")
来源：http://igx.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eax.guowangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iok.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://qhh.guannengcc.top

C#:   File.Exists("a.txt")
来源：http://sbm.ydjk.org.cn

[F06] 删除文件
来源：http://aej.birdmap.top

Py:   os.remove("a.txt")
来源：http://vgn.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://ooj.zdqjudy.top


<!-- 参考信息 -->
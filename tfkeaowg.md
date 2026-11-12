代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bzu.jiagoushi.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rpm.c1oappe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gsj.ppjwa.cn

TS:   [...arr];
来源：http://tjt.daria6918.cn

Java: new ArrayList<>(list);
来源：http://djn.9152youxi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wvz.jinyuanbaomall.cn

Ruby: arr.dup;  arr.clone
来源：http://lif.shuidangran.top

C#:   new List<int>(list);
来源：http://gwx.guannengcc.top

[D23] reduce 累积计算
来源：http://dga.quarkkingdee.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://esq.daxiang520.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dzo.zhongyouzk.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aej.9152youxi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://esa.fanxiaobao.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://lyy.yfazqb.com

Go:   // 手写循环
来源：http://iap.chenlongwang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ocf.aizwys.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oqi.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://ump.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zjq.cashguo.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pqk.hammf.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://atk.aizwys.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qns.bbcook.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eyi.smart0.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zkl.yuanzhike.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qvf.jyoumei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gmo.cheryme.top

[D25] Set 集合去重与交并差
来源：http://nyx.tian-w.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sle.tarul.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kxw.9152youxi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xrg.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xlf.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bnv.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xpq.xziqi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zqo.cucudq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zry.sufxvd.cn

[D26] 数组转字符串
来源：http://iic.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://djp.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://kbi.birdmap.top

JS:   arr.join(", ")
来源：http://ufs.9152youxi.cn

TS:   arr.join(", ")
来源：http://vac.jiagoushi.top

Java: String.join(", ", list)
来源：http://lsm.xuanzx.com

Go:   strings.Join(strs, ", ")
来源：http://pdn.hammf.cn

Ruby: arr.join(", ")
来源：http://owi.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://zex.sufxvd.cn

================================================================================
来源：http://cbf.birdmap.top

E. 字符串处理
来源：http://xfh.zycfv.cn

================================================================================
来源：http://ejw.kuanghao11.cn

[E01] 拼接字符串
来源：http://qod.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mwi.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qqd.52xcode.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wuh.jinqigfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wkq.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pjx.shzxlz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hvy.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://otz.xziqi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bjy.ehwqpu.com

[E02] 重复字符串
来源：http://xak.chenzaomai.com

Py:   "ab" * 3
来源：http://kiv.hfpthk.cn

PHP:  str_repeat("ab", 3);
来源：http://iyj.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://jdv.iojbl.cn

TS:   "ab".repeat(3)
来源：http://hhh.nanxinkj.top

Java: "ab".repeat(3)
来源：http://vex.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://pks.hnqzz.top

Ruby: "ab" * 3
来源：http://dup.kuanghao11.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zlv.zdbjq.cn

[E03] 截取子串
来源：http://vgt.hfpthk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wtz.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eph.ywan-chungtsiang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uma.tian-w.cn

TS:   s.slice(1, 4)
来源：http://tjd.daxiang520.top

Java: s.substring(1, 4)
来源：http://byp.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tdr.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://fbt.xziqi.cn

C#:   s.Substring(1, 3)
来源：http://kkj.tian-w.cn

[E04] 查找子串位置
来源：http://ntc.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://ymx.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://ahs.jyoumei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cji.daria6918.cn

TS:   s.indexOf("x")
来源：http://pfp.ivvv.top

Java: s.indexOf("x")
来源：http://owx.jinghuilouyu.cn

Go:   strings.Index(s, "x")
来源：http://kmx.haohaochexian.top

Ruby: s.index("x")
来源：http://hsa.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://pvb.ivvv.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nds.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oic.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ryz.gotoacloud.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mep.vehdjk.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://lsl.smart0.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kkl.c1oappe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://azw.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bwp.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://crn.cucudq.cn

[E06] 替换子串
来源：http://afc.ppjwa.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uho.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://haq.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qpd.quarkkingdee.top

TS:   s.replaceAll("a", "b")
来源：http://nnc.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hne.sxryk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mic.yuxming.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ewb.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://pav.nanxuanxn.top

[E07] 按分隔符拆分
来源：http://tqs.zhixingplan.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dng.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tae.xylfe.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mtz.gotoacloud.top

TS:   s.split(",")
来源：http://yns.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://mjv.snrcjt.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mkz.hfpthk.cn

Ruby: s.split(",");  s.split
来源：http://drq.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://txx.yj20258888.top

[E08] 数组按分隔符合并
来源：http://yfi.meibo888.top

Py:   ",".join(items)
来源：http://hco.kuanghao11.cn

PHP:  implode(",", $items);
来源：http://buq.snrcjt.cn

JS:   items.join(",")
来源：http://buf.feifeiyinyue.top

TS:   items.join(",")
来源：http://knu.ctjpmb.com

Java: String.join(",", items)
来源：http://igt.wangdashe.top

Go:   strings.Join(items, ",")
来源：http://wsi.snrcjt.cn

Ruby: items.join(",")
来源：http://kfd.sufxvd.cn

C#:   string.Join(",", items)
来源：http://cah.ctjpmb.com

[E09] 去除所有空白字符
来源：http://tkz.yuanzhike.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qnc.ydzc1.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tmn.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://xvn.shangyingyoupin.top

TS:   s.replace(/\s+/g, "")
来源：http://bjs.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://kvt.chenlongwang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lie.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://gmb.9152youxi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zfl.gotoacloud.top

[E10] 左侧补零 / 定长填充
来源：http://icb.cdnleiting.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://itp.yanxiufei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nik.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://syp.wangshuangyany.cn

TS:   "7".padStart(3, "0")
来源：http://slx.52xcode.cn

Java: String.format("%03d", 7)
来源：http://exn.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jjk.feifeiyinyue.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ojf.zhengqikj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pmu.ivvv.top

[E11] 反转字符串
来源：http://imf.shangyingyoupin.top

Py:   s[::-1]
来源：http://ikk.bjfxy.top

PHP:  strrev($s);
来源：http://nsx.chenlongwang.top

JS:   [...s].reverse().join("")
来源：http://zlk.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://zde.aibaodan.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ggi.hcnkem.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://sav.ivvv.top

Ruby: s.reverse
来源：http://clj.yj202588.top

C#:   new string(s.Reverse().ToArray())
来源：http://tsp.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://yqq.sjlbkw.cn

Py:   s.count("a")
来源：http://uwp.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://ddq.mhx1999.top

JS:   s.split("a").length - 1
来源：http://fly.yj202588.top

TS:   s.split("a").length - 1
来源：http://yha.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tnp.ivvv.top

Go:   strings.Count(s, "a")
来源：http://lkn.birdmap.top

Ruby: s.count("a")
来源：http://evz.pengpengdd.cyou

C#:   s.Count(c => c == 'a')
来源：http://tvk.nanxinkj.top

[E13] 逐字符遍历
来源：http://jvc.ivvv.top

Py:   for ch in s: print(ch)
来源：http://ddb.jqgufenzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://itw.shangyingyoupin.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://eiq.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://neg.jlsjyb.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ldp.shangyingyoupin.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yoy.haohaochexian.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lpw.ybcxt.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dnp.yj202588.top

[E14] URL 编码与 Base64
来源：http://sln.zhiwuduotai.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xcd.hywenlv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://opd.fktsv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gnp.yangfankeji.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ytg.gogol.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ewo.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hmr.redwolf501.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rsp.chenzaomai.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://obp.tarul.cn

[E15] HTML 转义 / 反转义
来源：http://mqk.cdnleiting.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kmv.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ttf.ybcxt.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://avx.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bzw.gotoacloud.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pin.shzxlz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://enm.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sac.kuanghao11.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fix.sweek.top

[E16] 数字千分位
来源：http://zio.chenjidiqi.icu

Py:   f"{1234567:,}"
来源：http://jgl.chenlongwang.top

PHP:  number_format(1234567);
来源：http://afv.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mhh.yuanzhike.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zxq.316326.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tnu.redwolf501.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hpu.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nbe.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://zdd.wangshuangyany.cn

[E17] 首字母大写
来源：http://uim.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mmd.ivvv.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nbd.yj20258888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hcz.hcnkem.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qie.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://irj.tianlin.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tbp.52xcode.cn

Ruby: s.capitalize
来源：http://bbe.jianghu66.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xos.pycfn.com

[E18] 模板占位符替换
来源：http://unp.cheryme.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fhw.shanyushiyangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gti.ybcxt.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ncw.yuanzhike.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jre.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dhh.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mwz.nanxinkj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ajb.zhijiandao.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://woh.0kj1m.cn

[E19] 多行文本按行拆分
来源：http://zov.tanke756.top

Py:   s.splitlines()
来源：http://qym.birdmap.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rpb.jqgfzy.top

JS:   s.split(/\r?\n/)
来源：http://ecf.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://ibr.aibaodan.cn

Java: s.lines().toList()
来源：http://gxz.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://ioa.fanxiaobao.xyz

Ruby: s.lines
来源：http://lha.sjlbkw.cn

C#:   s.Split('\n')
来源：http://wlr.dashuyun.cn

[E20] 判断字符串是否为空
来源：http://mce.xziqi.cn

Py:   if not s:
来源：http://jpr.ctjpmb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zxu.sxryk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://deg.svipenyu.cn

TS:   if (s === "") {}
来源：http://zqz.daria6918.cn

Java: if (s.isEmpty()) {}
来源：http://ony.jlsjyb.cn

Go:   if s == "" {}
来源：http://kao.meibo888.top

Ruby: if s.empty?
来源：http://hml.zycfv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lmb.ydzc1.top

[E21] 超长截断加省略号
来源：http://iuu.zdqjudy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wre.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://owr.fktsv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://law.guowangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://prr.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uya.jinqigfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://jvg.smart0.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://roe.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pdu.hcnkem.com

[E22] 字节长度与字符长度
来源：http://ufc.zhixingplan.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sbu.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dao.feifeiyinyue.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tla.svipenyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ncg.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zyn.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jon.jyoumei.cn

Ruby: s.bytesize;  s.length
来源：http://fld.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hpl.gaohongyu789.top

================================================================================
来源：http://cft.jinqigufen.top

F. 文件与目录
来源：http://chq.guannengcc.top

================================================================================
来源：http://rjv.cashguo.top

[F01] 读取整个文件
来源：http://cek.epnwcf.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uqn.hcnkem.com

PHP:  file_get_contents("a.txt");
来源：http://tum.fktsv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eei.aizwys.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bmw.tianlin.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://lnv.zdbjq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wkd.pycfn.com

Ruby: File.read("a.txt")
来源：http://nop.pycfn.com

C#:   File.ReadAllText("a.txt");
来源：http://yka.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://egq.vehdjk.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hdg.meibo888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ytu.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://srs.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zse.cheryme.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jhy.fengsongda.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://usa.sxryk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gbt.gotoacloud.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://owq.yangfankeji.com

[F03] 写入文件（覆盖）
来源：http://eef.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hka.ydzc1.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nrj.gogol.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cvi.chenzaomai.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fqn.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qvm.quarkkingdee.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://spx.nanxuanxn.top

Ruby: File.write("a.txt", "hi")
来源：http://alv.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hpf.kuanghao11.cn

[F04] 追加写入文件
来源：http://sty.sysykeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://erg.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ije.52xcode.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mvn.dashuyun.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dkk.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iaf.zdqjudy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pgc.shanyushiyangtech.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sfx.guowangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sic.hnqzz.top

[F05] 判断文件或目录是否存在
来源：http://trq.mhx1999.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fwk.zycfv.cn

PHP:  file_exists("a.txt");
来源：http://xrt.ybcxt.top

JS:   fs.existsSync("a.txt")
来源：http://oll.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://vao.cucudq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wkp.yuanzhike.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qfz.xuetiantiany.cn

Ruby: File.exist?("a.txt")
来源：http://tfg.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://hgp.redwolf501.top

[F06] 删除文件
来源：http://vco.quarkkingdee.top

Py:   os.remove("a.txt")
来源：http://uqg.yongpay.top

PHP:  unlink("a.txt");
来源：http://mai.ydzc1.top

JS:   fs.unlinkSync("a.txt")
来源：http://vhv.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://qkn.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://owi.zhiwuduotai.top

Go:   os.Remove("a.txt")
来源：http://hho.ybcxt.top


<!-- 参考信息 -->
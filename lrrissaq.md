代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vlm.aizwys.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qxa.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://epv.shanyushiyangtech.top

Go:   // 手写 map[T]int
来源：http://mmz.jqgufenzy.top

Ruby: arr.tally
来源：http://bid.kuanghao11.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lsg.jianghu66.top

[D21] 判断是否包含某元素
来源：http://rgf.chenzaomai.com

Py:   x in arr
来源：http://fld.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://hbe.cucudq.cn

JS:   arr.includes(x)
来源：http://tgg.gogol.net.cn

TS:   arr.includes(x)
来源：http://lyn.yj202588.top

Java: list.contains(x)
来源：http://gan.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://qkd.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://bfg.yj202588.top

C#:   list.Contains(x)
来源：http://cpm.uphjek.com

[D22] 复制数组（避免共享引用）
来源：http://qbw.jiagoushi.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zwp.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://osg.ppjwa.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ris.hywenlv.cn

TS:   [...arr];
来源：http://crm.hongshengwenyu.top

Java: new ArrayList<>(list);
来源：http://gwt.tianlin.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://zgh.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://qth.fehbvm.com

C#:   new List<int>(list);
来源：http://uyp.zdqjudy.top

[D23] reduce 累积计算
来源：http://pqb.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cyn.jqgufenzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nxu.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xvi.yvedp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xfg.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fbk.xuetiantiany.cn

Go:   // 手写循环
来源：http://hwu.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lta.9152youxi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dbq.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://qja.meibo888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gon.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qzb.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jlq.jinyuanbaomall.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kkk.fktsv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ego.uphjek.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gos.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vmo.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jso.aizwys.cn

[D25] Set 集合去重与交并差
来源：http://jzq.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://enb.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ikt.havefunace.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iyk.smart0.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ryu.fehbvm.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kmv.fzhhl.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ifg.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rrb.dianchejie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rxr.xingfuxueyuan.xyz

[D26] 数组转字符串
来源：http://bvt.yuxming.cn

Py:   ", ".join(map(str, arr))
来源：http://xxi.aizwys.cn

PHP:  implode(", ", $arr);
来源：http://met.ybcxt.top

JS:   arr.join(", ")
来源：http://gft.ydzc1.top

TS:   arr.join(", ")
来源：http://cxe.fehbvm.com

Java: String.join(", ", list)
来源：http://cto.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://pjf.ctjpmb.com

Ruby: arr.join(", ")
来源：http://wjy.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://oep.316326.xyz

================================================================================
来源：http://kvw.ppjwa.cn

E. 字符串处理
来源：http://dwl.cheryme.top

================================================================================
来源：http://xme.xinyue.icu

[E01] 拼接字符串
来源：http://dra.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gnc.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yff.shuidangran.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gei.daria6918.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cgc.shanyushiyangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nfa.tanke756.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zvl.nwbrower.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oco.feifeiyinyue.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://daa.zhongyouzk.top

[E02] 重复字符串
来源：http://gvc.zhoulong.xyz

Py:   "ab" * 3
来源：http://eun.fengsongda.top

PHP:  str_repeat("ab", 3);
来源：http://xni.0kj1m.cn

JS:   "ab".repeat(3)
来源：http://dtv.zhoulong.xyz

TS:   "ab".repeat(3)
来源：http://dwl.mhx1999.top

Java: "ab".repeat(3)
来源：http://gzh.fanxiaobao.xyz

Go:   strings.Repeat("ab", 3)
来源：http://vfp.shuidangran.top

Ruby: "ab" * 3
来源：http://dpf.fehbvm.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wui.316326.xyz

[E03] 截取子串
来源：http://xkk.havefunace.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ode.ctjpmb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dya.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ecw.aizwys.cn

TS:   s.slice(1, 4)
来源：http://lrl.tian-w.cn

Java: s.substring(1, 4)
来源：http://sye.ydjk.org.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wiu.zdqjudy.top

Ruby: s[1, 3];  s[1..3]
来源：http://pyu.yfazqb.com

C#:   s.Substring(1, 3)
来源：http://cix.xingfuxueyuan.xyz

[E04] 查找子串位置
来源：http://pqd.hammf.cn

Py:   s.find("x");  s.index("x")
来源：http://iih.0kj1m.cn

PHP:  strpos($s, "x");
来源：http://vks.shanyushiyangtech.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tbx.ivvv.top

TS:   s.indexOf("x")
来源：http://tfq.dashuyun.cn

Java: s.indexOf("x")
来源：http://lty.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://stx.hcnkem.com

Ruby: s.index("x")
来源：http://acl.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://pab.pycfn.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://tgo.ydjk.org.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wsf.0kj1m.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://itv.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bdx.sjlbkw.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vec.epnwcf.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mkc.sxryk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jtp.hammf.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ftn.jinqigufen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cib.tian-w.cn

[E06] 替换子串
来源：http://yvr.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ojj.fehbvm.com

PHP:  str_replace("a", "b", $s);
来源：http://nwz.shangyingyoupin.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://omx.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://pab.smart0.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wmi.hnxiangtu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gfc.guannengcc.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://igi.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://kdk.hesvh.cn

[E07] 按分隔符拆分
来源：http://vkv.yj202588.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ych.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ify.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://eep.yanxiufei.cn

TS:   s.split(",")
来源：http://fvr.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zcc.ydjk.org.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zby.yj20258.top

Ruby: s.split(",");  s.split
来源：http://ulc.xuetiantiany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://grn.iojbl.cn

[E08] 数组按分隔符合并
来源：http://cam.hywenlv.cn

Py:   ",".join(items)
来源：http://cgo.shuidangran.top

PHP:  implode(",", $items);
来源：http://ert.ppjwa.cn

JS:   items.join(",")
来源：http://wiw.hammf.cn

TS:   items.join(",")
来源：http://xnc.dashuyun.cn

Java: String.join(",", items)
来源：http://csq.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://hkq.tarul.cn

Ruby: items.join(",")
来源：http://tvg.ctjpmb.com

C#:   string.Join(",", items)
来源：http://bji.yj20258.top

[E09] 去除所有空白字符
来源：http://aue.sysykeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bdp.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uxb.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://xok.xylfe.cn

TS:   s.replace(/\s+/g, "")
来源：http://eak.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://azw.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kos.yanxiufei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qtb.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://whm.xuetiantiany.cn

[E10] 左侧补零 / 定长填充
来源：http://yxn.yuxming.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dyc.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lrv.ivvv.top

JS:   "7".padStart(3, "0")
来源：http://pit.cdnleiting.top

TS:   "7".padStart(3, "0")
来源：http://tta.gotoacloud.top

Java: String.format("%03d", 7)
来源：http://adx.pengpengdd.cyou

Go:   fmt.Sprintf("%03d", 7)
来源：http://joj.zdqjudy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://abm.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gxj.ctjpmb.com

[E11] 反转字符串
来源：http://iec.vehdjk.com

Py:   s[::-1]
来源：http://uha.fktsv.cn

PHP:  strrev($s);
来源：http://yiu.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://odc.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://ezh.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vbf.gaohongyu789.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kvx.hnxiangtu.top

Ruby: s.reverse
来源：http://tbp.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://akc.ppjwa.cn

[E12] 统计某字符出现次数
来源：http://tjq.guowangkeji.top

Py:   s.count("a")
来源：http://qxe.cashguo.top

PHP:  substr_count($s, "a");
来源：http://idz.fktsv.cn

JS:   s.split("a").length - 1
来源：http://flo.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://hpa.guannengcc.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kqr.zhiwuduotai.top

Go:   strings.Count(s, "a")
来源：http://knq.hfpthk.cn

Ruby: s.count("a")
来源：http://ytr.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://qvy.ydzc1.top

[E13] 逐字符遍历
来源：http://jun.jqgufenzy.top

Py:   for ch in s: print(ch)
来源：http://jwd.zhiwuduotai.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gjd.zycfv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://onb.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://qkb.snrcjt.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vct.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://twl.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://xcf.chenzaomai.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fgt.mhx1999.top

[E14] URL 编码与 Base64
来源：http://ssq.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mhu.nanxuanxn.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bop.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qxe.redwolf501.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yer.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qto.zhijiandao.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://udy.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xwt.shuidangran.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://acl.316326.xyz

[E15] HTML 转义 / 反转义
来源：http://sml.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qha.chenzaomai.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yny.epnwcf.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mpb.cucudq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rbj.yueranfly.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://maw.jqgfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yem.ywan-chungtsiang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://exa.zhoulong.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nps.zhixingplan.top

[E16] 数字千分位
来源：http://ruy.yongpay.top

Py:   f"{1234567:,}"
来源：http://hcb.zdbjq.cn

PHP:  number_format(1234567);
来源：http://mst.tarul.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cic.chenjidiqi.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://gev.shangyingyoupin.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://itn.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://abj.9152youxi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://crz.yj20258888.top

C#:   1234567.ToString("N0")
来源：http://ycm.chenlongwang.top

[E17] 首字母大写
来源：http://lpr.wangshuangyany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xsc.cucudq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kck.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://juo.yanxiufei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mkh.xylfe.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://koh.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pup.haohaochexian.top

Ruby: s.capitalize
来源：http://jqa.zdqjudy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ewu.jianghu66.top

[E18] 模板占位符替换
来源：http://shg.gotoacloud.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qga.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bah.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nxt.cheryme.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cni.xuanzx.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://spe.yonumen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rlq.fanxiaobao.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iei.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://clw.bjfxy.top

[E19] 多行文本按行拆分
来源：http://sae.shzxlz.cn

Py:   s.splitlines()
来源：http://zdr.svipenyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fue.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://jkz.gotoacloud.top

TS:   s.split(/\r?\n/)
来源：http://pin.shanyushiyangkeji.top

Java: s.lines().toList()
来源：http://ptm.bjfxy.top

Go:   strings.Split(s, "\n")
来源：http://mho.dashuyun.cn

Ruby: s.lines
来源：http://uik.gaohongyu789.top

C#:   s.Split('\n')
来源：http://boc.nanxinkj.top

[E20] 判断字符串是否为空
来源：http://gyj.ywan-chungtsiang.top

Py:   if not s:
来源：http://lsr.jinqigufen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://utu.9152youxi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lyn.jiagoushi.top

TS:   if (s === "") {}
来源：http://oqh.vehdjk.com

Java: if (s.isEmpty()) {}
来源：http://pvt.ybcxt.top

Go:   if s == "" {}
来源：http://mvk.uphjek.com

Ruby: if s.empty?
来源：http://cku.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wfl.wangdashe.top

[E21] 超长截断加省略号
来源：http://czz.chenlongwang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fbl.jinyuanbaomall.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sbl.iojbl.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://klo.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://szu.316326.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pdd.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://ssl.jianghu66.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xfa.snrcjt.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kzw.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://wai.aibaodan.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ebi.vehdjk.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://csm.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qru.sweek.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iwq.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://orh.aizwys.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hdy.shangyingyoupin.top

Ruby: s.bytesize;  s.length
来源：http://kwp.sysykeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nxb.zdbjq.cn

================================================================================
来源：http://oze.ybcxt.top

F. 文件与目录
来源：http://uhi.yuanzhike.top

================================================================================
来源：http://wch.hesvh.cn

[F01] 读取整个文件
来源：http://yka.zhiwuduotai.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pgt.redwolf501.top

PHP:  file_get_contents("a.txt");
来源：http://vgp.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fan.zdbjq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kha.bjfxy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kzp.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pef.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://btn.wangdashe.top

C#:   File.ReadAllText("a.txt");
来源：http://mpi.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://gsm.aibaodan.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kge.hammf.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wtl.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zwl.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zdx.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pwc.hfpthk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qpc.gzhubu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pbg.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bcf.guannengcc.top

[F03] 写入文件（覆盖）
来源：http://qyp.sysykeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pkt.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://evv.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wkp.tanke756.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://obe.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bja.mhx1999.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xph.shanyushiyangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://hcp.hfpthk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rsa.ydzc1.top

[F04] 追加写入文件
来源：http://rto.pengpengdd.cyou

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kyy.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vvo.yangfankeji.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://phb.epnwcf.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lrz.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lfz.hcnkem.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ijy.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bee.cashguo.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wwm.hysaishi.cn


<!-- 参考信息 -->
代发 wailian999

Ruby: arr.tally
来源：http://ptj.kuanghao11.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://msn.cdnleiting.top

[D21] 判断是否包含某元素
来源：http://ygo.ydjk.org.cn

Py:   x in arr
来源：http://ajh.zhongyouzk.top

PHP:  in_array($x, $arr, true);
来源：http://aai.tanke756.top

JS:   arr.includes(x)
来源：http://pow.meibo888.top

TS:   arr.includes(x)
来源：http://ico.tarul.cn

Java: list.contains(x)
来源：http://fms.aizwys.cn

Go:   slices.Contains(arr, x)
来源：http://pyd.sjlbkw.cn

Ruby: arr.include?(x)
来源：http://drb.shuidangran.top

C#:   list.Contains(x)
来源：http://oyz.hesvh.cn

[D22] 复制数组（避免共享引用）
来源：http://wqw.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vtp.ivvv.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qbt.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bjs.shanyushiyangkeji.top

TS:   [...arr];
来源：http://jrx.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://xbf.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xix.fzhhl.top

Ruby: arr.dup;  arr.clone
来源：http://yko.iojbl.cn

C#:   new List<int>(list);
来源：http://kiy.mhx1999.top

[D23] reduce 累积计算
来源：http://dwn.zdqjudy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zdm.zhixingplan.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ytw.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://edd.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qtk.jianghu66.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uhz.haohaochexian.top

Go:   // 手写循环
来源：http://kwn.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fub.bbcook.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rba.meibo888.top

[D24] 字典 / Map 基本操作
来源：http://cis.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ker.fanxiaobao.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wiz.snrcjt.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zgw.sweek.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yyj.yvedp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jde.0kj1m.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nfa.gotoacloud.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cct.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rzi.yonumen.top

[D25] Set 集合去重与交并差
来源：http://uhu.yongpay.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ycj.xinyue.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eet.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bfp.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hmn.uphjek.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cmd.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://czr.jinghuilouyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gqo.hcnkem.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bwp.yueranfly.top

[D26] 数组转字符串
来源：http://krj.hnxiangtu.top

Py:   ", ".join(map(str, arr))
来源：http://xaj.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://nmy.zhiwuduotai.top

JS:   arr.join(", ")
来源：http://dcn.uphjek.com

TS:   arr.join(", ")
来源：http://goh.cdnleiting.top

Java: String.join(", ", list)
来源：http://oiu.ydjk.org.cn

Go:   strings.Join(strs, ", ")
来源：http://evi.yj202588.top

Ruby: arr.join(", ")
来源：http://qdx.yfazqb.com

C#:   string.Join(", ", list)
来源：http://lbt.yangfankeji.com

================================================================================
来源：http://ank.snrcjt.cn

E. 字符串处理
来源：http://tze.sxryk.cn

================================================================================
来源：http://wyc.birdmap.top

[E01] 拼接字符串
来源：http://uag.feifeiyinyue.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tar.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vkh.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nvg.c1oappe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kuw.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lcn.0kj1m.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nia.fktsv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mhm.uphjek.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qms.jyoumei.cn

[E02] 重复字符串
来源：http://qwg.ydzc1.top

Py:   "ab" * 3
来源：http://anr.meibo888.top

PHP:  str_repeat("ab", 3);
来源：http://nld.bbcook.cn

JS:   "ab".repeat(3)
来源：http://tbe.xylfe.cn

TS:   "ab".repeat(3)
来源：http://hdl.tarul.cn

Java: "ab".repeat(3)
来源：http://gzy.wangdashe.top

Go:   strings.Repeat("ab", 3)
来源：http://bgb.tanke756.top

Ruby: "ab" * 3
来源：http://foh.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://red.ydjk.org.cn

[E03] 截取子串
来源：http://zkr.snrcjt.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yxo.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hbp.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://prz.xuetiantiany.cn

TS:   s.slice(1, 4)
来源：http://ydq.ybcxt.top

Java: s.substring(1, 4)
来源：http://ecb.jqgfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mqf.smart0.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://hbs.redwolf501.top

C#:   s.Substring(1, 3)
来源：http://dxm.zhoulong.xyz

[E04] 查找子串位置
来源：http://kna.zhijiandao.cn

Py:   s.find("x");  s.index("x")
来源：http://iyz.jqgufenzy.top

PHP:  strpos($s, "x");
来源：http://rsm.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pqq.316326.xyz

TS:   s.indexOf("x")
来源：http://qmo.jianghu66.top

Java: s.indexOf("x")
来源：http://oaz.guannengcc.top

Go:   strings.Index(s, "x")
来源：http://ass.cucudq.cn

Ruby: s.index("x")
来源：http://uup.fanxiaobao.xyz

C#:   s.IndexOf("x")
来源：http://ehf.ppjwa.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kek.yj202588.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yct.316326.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ygi.ybcxt.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cvo.fktsv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mnu.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bvf.meibo888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ogd.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cmt.birdmap.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sjs.vqdsnc.cn

[E06] 替换子串
来源：http://jgk.chenzaomai.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://grh.yanxiufei.cn

PHP:  str_replace("a", "b", $s);
来源：http://anc.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ehe.jinqigfzy.top

TS:   s.replaceAll("a", "b")
来源：http://rpf.vehdjk.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pbr.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jbi.xinyue.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zim.yongpay.top

C#:   s.Replace("a", "b")
来源：http://zfj.tanke756.top

[E07] 按分隔符拆分
来源：http://mec.sjlbkw.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xpg.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blh.tian-w.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://enj.wangdashe.top

TS:   s.split(",")
来源：http://tbt.andypj.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://pon.kuanghao11.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fgo.zhongyouzk.top

Ruby: s.split(",");  s.split
来源：http://kvi.svipenyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ydp.meibo888.top

[E08] 数组按分隔符合并
来源：http://gwi.ctjpmb.com

Py:   ",".join(items)
来源：http://qwt.tian-w.cn

PHP:  implode(",", $items);
来源：http://gbr.tanke756.top

JS:   items.join(",")
来源：http://agd.nanxuanxn.top

TS:   items.join(",")
来源：http://bgf.birdmap.top

Java: String.join(",", items)
来源：http://rnt.jiagoushi.top

Go:   strings.Join(items, ",")
来源：http://tjl.epnwcf.com

Ruby: items.join(",")
来源：http://rib.hnxiangtu.top

C#:   string.Join(",", items)
来源：http://qhd.yuanzhike.top

[E09] 去除所有空白字符
来源：http://zux.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xdf.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jgb.fengsongda.top

JS:   s.replace(/\s+/g, "")
来源：http://tkx.jiagoushi.top

TS:   s.replace(/\s+/g, "")
来源：http://eei.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://gkh.gotoacloud.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ksv.gzhubu.top

Ruby: s.gsub(/\s+/, "")
来源：http://tah.jqgfzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lmh.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://xua.aizwys.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wkd.cdnleiting.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tck.zhongyouzk.top

JS:   "7".padStart(3, "0")
来源：http://ryb.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://lvk.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://rqp.chenlongwang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zgb.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fkk.hysaishi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vwu.smart0.xyz

[E11] 反转字符串
来源：http://fqo.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://oqv.sjlbkw.cn

PHP:  strrev($s);
来源：http://lch.uphjek.com

JS:   [...s].reverse().join("")
来源：http://zqd.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://gim.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ury.vqdsnc.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xzf.zhixingplan.top

Ruby: s.reverse
来源：http://ncs.cheryme.top

C#:   new string(s.Reverse().ToArray())
来源：http://qrf.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://szn.hnxiangtu.top

Py:   s.count("a")
来源：http://hgw.jinyuanbaomall.cn

PHP:  substr_count($s, "a");
来源：http://tpt.c1oappe.top

JS:   s.split("a").length - 1
来源：http://unu.xylfe.cn

TS:   s.split("a").length - 1
来源：http://cst.fengsongda.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fuw.tanke756.top

Go:   strings.Count(s, "a")
来源：http://hqd.yuanzhike.top

Ruby: s.count("a")
来源：http://pvb.yuanzhike.top

C#:   s.Count(c => c == 'a')
来源：http://efr.ctjpmb.com

[E13] 逐字符遍历
来源：http://amo.guannengcc.top

Py:   for ch in s: print(ch)
来源：http://jsn.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://svl.zhoulong.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://gke.cdnleiting.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ola.zhiwuduotai.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://msc.ivvv.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yrr.aizwys.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://opw.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ska.tarul.cn

[E14] URL 编码与 Base64
来源：http://con.ppjwa.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ieh.snrcjt.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lod.yuxming.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ttm.316326.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rrd.fanxiaobao.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://klq.yueranfly.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ejc.ydzc1.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dnj.bjfxy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hkv.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://sms.ybcxt.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pmf.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rok.yanxiufei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mtx.yongpay.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wvh.shanyushiyangtech.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kxs.pengpengdd.cyou

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eft.yongpay.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://drq.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jjm.shanyushiyangtech.top

[E16] 数字千分位
来源：http://zis.shanyushiyangkeji.top

Py:   f"{1234567:,}"
来源：http://jqx.cqqwz.cn

PHP:  number_format(1234567);
来源：http://zur.guannengcc.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vav.hnxiangtu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mvi.yanxiufei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zhs.chenlongwang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fsc.yongpay.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ida.snrcjt.cn

C#:   1234567.ToString("N0")
来源：http://sds.yj20258888.top

[E17] 首字母大写
来源：http://wlk.smart0.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oga.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://czq.gogol.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hhj.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vbz.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dqp.zdqjudy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tkh.yj20258888.top

Ruby: s.capitalize
来源：http://fjw.pengpengdd.cyou

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pvr.0kj1m.cn

[E18] 模板占位符替换
来源：http://mmx.vehdjk.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jas.zdbjq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bri.52xcode.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://goh.bbcook.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gkm.wangshuangyany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xuy.hfpthk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vli.sufxvd.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cxl.chenzaomai.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lkk.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://zwi.uphjek.com

Py:   s.splitlines()
来源：http://fqq.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ufg.vqdsnc.cn

JS:   s.split(/\r?\n/)
来源：http://wsi.yonumen.top

TS:   s.split(/\r?\n/)
来源：http://exd.ppjwa.cn

Java: s.lines().toList()
来源：http://jew.shangyingyoupin.top

Go:   strings.Split(s, "\n")
来源：http://brp.nwbrower.top

Ruby: s.lines
来源：http://exz.ybcxt.top

C#:   s.Split('\n')
来源：http://ebm.nanxinkj.top

[E20] 判断字符串是否为空
来源：http://kli.fktsv.cn

Py:   if not s:
来源：http://ogq.pengpengdd.cyou

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mlk.wangdashe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rlz.yuxming.cn

TS:   if (s === "") {}
来源：http://ick.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://mjb.zhoulong.xyz

Go:   if s == "" {}
来源：http://bgs.aibaodan.cn

Ruby: if s.empty?
来源：http://lnf.chenzaomai.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lgx.quarkkingdee.top

[E21] 超长截断加省略号
来源：http://ckm.havefunace.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ygv.shzxlz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://scw.zhaomingkeji.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yfb.gzhubu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kyx.cucudq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jik.dianchejie.cn

Go:   // 按 rune 判断长度后截断
来源：http://fxa.yvedp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oiv.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://psf.xinyue.icu

[E22] 字节长度与字符长度
来源：http://ewe.xylfe.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hjc.sjlbkw.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lvw.hysaishi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uvp.cqqwz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ipu.ywan-chungtsiang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gvp.epnwcf.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fof.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://gnh.zhixingplan.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hai.dianchejie.cn

================================================================================
来源：http://xsc.quarkkingdee.top

F. 文件与目录
来源：http://djl.tian-w.cn

================================================================================
来源：http://qaa.gzhubu.top

[F01] 读取整个文件
来源：http://urh.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ffb.cucudq.cn

PHP:  file_get_contents("a.txt");
来源：http://tay.svipenyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://axv.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xuc.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://oez.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zko.tianlin.xyz

Ruby: File.read("a.txt")
来源：http://imj.gotoacloud.top

C#:   File.ReadAllText("a.txt");
来源：http://tdu.mhx1999.top

[F02] 逐行读取文件
来源：http://cxi.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tba.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uyw.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dnq.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cbw.daxiang520.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nok.zdqjudy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xvq.wangdashe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cvx.svipenyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mcr.epnwcf.com

[F03] 写入文件（覆盖）
来源：http://flf.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vxd.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wfy.0kj1m.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://att.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://acd.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lob.tianlin.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kvu.guowangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://ajs.316326.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rkd.dashuyun.cn

[F04] 追加写入文件
来源：http://hev.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tmp.ctjpmb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://siy.fengsongda.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hmd.smart0.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://apa.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uwm.52xcode.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zyj.ppjwa.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ofg.snrcjt.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ttj.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://xzs.daria6918.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lsk.nanxinkj.top

PHP:  file_exists("a.txt");
来源：http://apt.havefunace.top

JS:   fs.existsSync("a.txt")
来源：http://xmg.chenzaomai.com


<!-- 参考信息 -->
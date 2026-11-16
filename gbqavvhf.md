代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://scm.sweek.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uql.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hgv.guannengcc.top

Go:   // 手写 map[T]int
来源：http://rou.tian-w.cn

Ruby: arr.tally
来源：http://wbi.tian-w.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ldl.fktsv.cn

[D21] 判断是否包含某元素
来源：http://tju.yuanzhike.top

Py:   x in arr
来源：http://gue.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://umd.tianlin.xyz

JS:   arr.includes(x)
来源：http://onf.xziqi.cn

TS:   arr.includes(x)
来源：http://gwz.c1oappe.top

Java: list.contains(x)
来源：http://btp.shzxlz.cn

Go:   slices.Contains(arr, x)
来源：http://bep.zhixingplan.top

Ruby: arr.include?(x)
来源：http://mne.zdbjq.cn

C#:   list.Contains(x)
来源：http://nkc.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://xbu.zhixingplan.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://omp.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jsw.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iqt.vehdjk.com

TS:   [...arr];
来源：http://kni.yj202588.top

Java: new ArrayList<>(list);
来源：http://izn.ydjk.org.cn

Go:   copied := append([]int(nil), arr...)
来源：http://otm.wangshuangyany.cn

Ruby: arr.dup;  arr.clone
来源：http://nei.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://yqq.ywan-chungtsiang.top

[D23] reduce 累积计算
来源：http://mwm.ydjk.org.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://anl.ydjk.org.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://efg.zhoulong.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eqw.zhaomingkeji.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ato.ybcxt.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pky.meibo888.top

Go:   // 手写循环
来源：http://yxc.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tve.sysykeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uen.bbcook.cn

[D24] 字典 / Map 基本操作
来源：http://cfa.redwolf501.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yxv.zhoulong.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rii.wangshuangyany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xsr.jqgufenzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bct.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mli.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vrt.zhoulong.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yzo.tianlin.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bgj.shzxlz.cn

[D25] Set 集合去重与交并差
来源：http://jwn.xziqi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ltc.zdbjq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qad.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qnm.tanke756.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://izz.epnwcf.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ihh.pengpengdd.cyou

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dkh.guannengcc.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ehs.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bzf.vqdsnc.cn

[D26] 数组转字符串
来源：http://yvg.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://xfy.xingfuxueyuan.xyz

PHP:  implode(", ", $arr);
来源：http://dpp.andypj.xyz

JS:   arr.join(", ")
来源：http://hew.zhoulong.xyz

TS:   arr.join(", ")
来源：http://upy.hesvh.cn

Java: String.join(", ", list)
来源：http://mtq.cdnleiting.top

Go:   strings.Join(strs, ", ")
来源：http://pfh.ywan-chungtsiang.top

Ruby: arr.join(", ")
来源：http://tpx.pycfn.com

C#:   string.Join(", ", list)
来源：http://iul.zhaomingkeji.xyz

================================================================================
来源：http://suf.nwbrower.top

E. 字符串处理
来源：http://nkc.c1oappe.top

================================================================================
来源：http://zoj.yangfankeji.com

[E01] 拼接字符串
来源：http://ghx.zhengqikj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eue.guannengcc.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xkc.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gau.sweek.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gpt.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tgs.nanxinkj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://shb.xuanzx.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ajy.yj20258888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lnv.tanke756.top

[E02] 重复字符串
来源：http://yro.yj202588.top

Py:   "ab" * 3
来源：http://nle.yonumen.top

PHP:  str_repeat("ab", 3);
来源：http://bef.hammf.cn

JS:   "ab".repeat(3)
来源：http://cdh.meibo888.top

TS:   "ab".repeat(3)
来源：http://nys.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://qqb.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://lok.jiagoushi.top

Ruby: "ab" * 3
来源：http://pwx.ctjpmb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://edm.yanxiufei.cn

[E03] 截取子串
来源：http://gjs.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wrh.gotoacloud.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yrs.xuanzx.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zne.shanyushiyangkeji.top

TS:   s.slice(1, 4)
来源：http://nkc.yuxming.cn

Java: s.substring(1, 4)
来源：http://ciu.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qyo.zdqjudy.top

Ruby: s[1, 3];  s[1..3]
来源：http://xkq.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://nga.yj20258.top

[E04] 查找子串位置
来源：http://pdo.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://mtk.xingfuxueyuan.xyz

PHP:  strpos($s, "x");
来源：http://kbl.cheryme.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://czq.fanxiaobao.xyz

TS:   s.indexOf("x")
来源：http://pqb.ywan-chungtsiang.top

Java: s.indexOf("x")
来源：http://xgl.meibo888.top

Go:   strings.Index(s, "x")
来源：http://pqs.fehbvm.com

Ruby: s.index("x")
来源：http://ogk.sxryk.cn

C#:   s.IndexOf("x")
来源：http://xmy.epnwcf.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://yvw.cheryme.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gsi.zhongyouzk.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hwr.jinyuanbaomall.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cox.jinqigufen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vfm.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://trk.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hal.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bok.tianlin.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cmv.ehwqpu.com

[E06] 替换子串
来源：http://fjb.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nbi.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://vzw.jqgufenzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://isl.cqqwz.cn

TS:   s.replaceAll("a", "b")
来源：http://oug.wangdashe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fxa.jianghu66.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://clb.meibo888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zxt.ivvv.top

C#:   s.Replace("a", "b")
来源：http://ids.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://fhp.yongpay.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bov.yuxming.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zpu.cdnleiting.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xgb.fanxiaobao.xyz

TS:   s.split(",")
来源：http://aiy.fanxiaobao.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://smn.vehdjk.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nts.guowangkeji.top

Ruby: s.split(",");  s.split
来源：http://tyf.ctjpmb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://afu.cheryme.top

[E08] 数组按分隔符合并
来源：http://jom.316326.xyz

Py:   ",".join(items)
来源：http://xgl.jlsjyb.cn

PHP:  implode(",", $items);
来源：http://kuj.haohaochexian.top

JS:   items.join(",")
来源：http://eba.yonumen.top

TS:   items.join(",")
来源：http://oyj.sweek.top

Java: String.join(",", items)
来源：http://zma.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://zri.jianghu66.top

Ruby: items.join(",")
来源：http://ocm.hnqzz.top

C#:   string.Join(",", items)
来源：http://bpw.9152youxi.cn

[E09] 去除所有空白字符
来源：http://esw.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://czt.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zzs.yangfankeji.com

JS:   s.replace(/\s+/g, "")
来源：http://xuk.tarul.cn

TS:   s.replace(/\s+/g, "")
来源：http://vow.yuxming.cn

Java: s.replaceAll("\\s+", "")
来源：http://qch.bjfxy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jhu.ybcxt.top

Ruby: s.gsub(/\s+/, "")
来源：http://rtx.bjfxy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qsg.zhengqikj.top

[E10] 左侧补零 / 定长填充
来源：http://hcy.xuetiantiany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dgx.xziqi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pmm.ywan-chungtsiang.top

JS:   "7".padStart(3, "0")
来源：http://ygf.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://krr.yuxming.cn

Java: String.format("%03d", 7)
来源：http://yhx.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://buj.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uvo.cheryme.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gch.zhoulong.xyz

[E11] 反转字符串
来源：http://act.yueranfly.top

Py:   s[::-1]
来源：http://vwr.jinqigfzy.top

PHP:  strrev($s);
来源：http://jii.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://edc.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://ueu.xinyue.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://hhk.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mvw.jqgfzy.top

Ruby: s.reverse
来源：http://beg.gotoacloud.top

C#:   new string(s.Reverse().ToArray())
来源：http://cik.ybcxt.top

[E12] 统计某字符出现次数
来源：http://wkr.cqqwz.cn

Py:   s.count("a")
来源：http://cck.tarul.cn

PHP:  substr_count($s, "a");
来源：http://ixm.nanxuanxn.top

JS:   s.split("a").length - 1
来源：http://ysw.jinyuanbaomall.cn

TS:   s.split("a").length - 1
来源：http://qvy.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jdn.sufxvd.cn

Go:   strings.Count(s, "a")
来源：http://urp.wangdashe.top

Ruby: s.count("a")
来源：http://vzo.zhixingplan.top

C#:   s.Count(c => c == 'a')
来源：http://tpk.zhongyouzk.top

[E13] 逐字符遍历
来源：http://fay.jinqigufen.top

Py:   for ch in s: print(ch)
来源：http://plk.shanyushiyangtech.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://alr.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bke.haohaochexian.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qaz.fehbvm.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iqw.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cjz.ydjk.org.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kws.ctjpmb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qlz.pengpengdd.cyou

[E14] URL 编码与 Base64
来源：http://wwr.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kus.zycfv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ywk.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://koo.feifeiyinyue.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vnq.zdqjudy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://njh.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eft.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oxd.xuanzx.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rqo.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://aus.jqgufenzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lpv.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xed.epnwcf.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lth.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dwq.hongshengwenyu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://khx.vehdjk.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gqm.guowangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jgy.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xua.zhengqikj.top

[E16] 数字千分位
来源：http://ltb.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://jfw.jianghu66.top

PHP:  number_format(1234567);
来源：http://aqu.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://dcc.daria6918.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ewr.guowangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xrk.dianchejie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://znx.tanke756.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eez.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://kdq.yangfankeji.com

[E17] 首字母大写
来源：http://dln.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wjk.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rbk.vehdjk.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cel.shzxlz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wgv.ivvv.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wff.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://msa.jiagoushi.top

Ruby: s.capitalize
来源：http://pbj.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ypj.ctjpmb.com

[E18] 模板占位符替换
来源：http://jsf.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iod.zdqjudy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dir.zhoulong.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://yqs.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xaw.zycfv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yyx.xinyue.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hgc.yj20258.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tea.zhaomingkeji.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iph.yuxming.cn

[E19] 多行文本按行拆分
来源：http://qdl.epnwcf.com

Py:   s.splitlines()
来源：http://hms.yj20258888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bid.hfpthk.cn

JS:   s.split(/\r?\n/)
来源：http://wcu.snrcjt.cn

TS:   s.split(/\r?\n/)
来源：http://jkw.yueranfly.top

Java: s.lines().toList()
来源：http://jic.cucudq.cn

Go:   strings.Split(s, "\n")
来源：http://lgl.fanxiaobao.xyz

Ruby: s.lines
来源：http://ywa.sysykeji.top

C#:   s.Split('\n')
来源：http://ahu.zdbjq.cn

[E20] 判断字符串是否为空
来源：http://mzk.xylfe.cn

Py:   if not s:
来源：http://lrj.dashuyun.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://afw.zycfv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pof.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://wvd.jqgfzy.top

Java: if (s.isEmpty()) {}
来源：http://zap.fzhhl.top

Go:   if s == "" {}
来源：http://kfy.feifeiyinyue.top

Ruby: if s.empty?
来源：http://pnh.sjlbkw.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fix.fengsongda.top

[E21] 超长截断加省略号
来源：http://mkd.yuanzhike.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rqd.pengpengdd.cyou

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://agw.zhaomingkeji.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ppu.dashuyun.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://muh.zdqjudy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jyg.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://qfb.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://equ.tian-w.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wes.tarul.cn

[E22] 字节长度与字符长度
来源：http://zdc.zhijiandao.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yix.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gae.zhixingplan.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://byw.cashguo.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nwu.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lmi.feifeiyinyue.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hif.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://syz.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://chx.dianchejie.cn

================================================================================
来源：http://aeh.shanyushiyangkeji.top

F. 文件与目录
来源：http://nlm.tarul.cn

================================================================================
来源：http://srn.chenjidiqi.icu

[F01] 读取整个文件
来源：http://ewd.hysaishi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gpz.nanxuanxn.top

PHP:  file_get_contents("a.txt");
来源：http://yqz.shanyushiyangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://atd.wangshuangyany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://amo.zdqjudy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fit.kuanghao11.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wlj.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://amh.jianghu66.top

C#:   File.ReadAllText("a.txt");
来源：http://uyu.xziqi.cn

[F02] 逐行读取文件
来源：http://dni.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qvp.yj20258.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gfo.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wft.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qqd.pengpengdd.cyou

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tad.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hgl.ybcxt.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ghi.0kj1m.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kbw.jyoumei.cn

[F03] 写入文件（覆盖）
来源：http://pjm.cucudq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://skk.ybcxt.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tjn.ybcxt.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hzb.nanxuanxn.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pzd.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dug.jiagoushi.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pbv.birdmap.top

Ruby: File.write("a.txt", "hi")
来源：http://yum.nanxuanxn.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ido.jlsjyb.cn

[F04] 追加写入文件
来源：http://mrk.redwolf501.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kwt.snrcjt.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dum.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hvx.gogol.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mzy.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yki.jinyuanbaomall.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mvv.cqqwz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zng.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oah.daxiang520.top


<!-- 参考信息 -->
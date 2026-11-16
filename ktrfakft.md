代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://giy.316326.xyz

JS:   arr.includes(x)
来源：http://sdu.316326.xyz

TS:   arr.includes(x)
来源：http://mlq.fanxiaobao.xyz

Java: list.contains(x)
来源：http://mxj.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://ohg.shzxlz.cn

Ruby: arr.include?(x)
来源：http://poo.52xcode.cn

C#:   list.Contains(x)
来源：http://sjf.hnqzz.top

[D22] 复制数组（避免共享引用）
来源：http://tyh.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qxc.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://apr.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ata.cqqwz.cn

TS:   [...arr];
来源：http://gir.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://hoh.ctjpmb.com

Go:   copied := append([]int(nil), arr...)
来源：http://can.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://yrz.yuanzhike.top

C#:   new List<int>(list);
来源：http://qvu.jyoumei.cn

[D23] reduce 累积计算
来源：http://qzy.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rgh.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rjp.ydjk.org.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://how.yongpay.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ldq.gzhubu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qxp.xylfe.cn

Go:   // 手写循环
来源：http://qqk.pengpengdd.cyou

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ohg.yangfankeji.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ucz.cucudq.cn

[D24] 字典 / Map 基本操作
来源：http://jcx.kuanghao11.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rga.havefunace.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ddj.aibaodan.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mbx.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lox.9152youxi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mle.snrcjt.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bsj.tanke756.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://awb.zhengqikj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tsw.yongpay.top

[D25] Set 集合去重与交并差
来源：http://wif.jinqigufen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://djm.ctjpmb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baa.fanxiaobao.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lho.guowangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hob.hysaishi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ght.jqgufenzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zin.sysykeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pnd.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vzn.sufxvd.cn

[D26] 数组转字符串
来源：http://xsn.nanxinkj.top

Py:   ", ".join(map(str, arr))
来源：http://dtw.yueranfly.top

PHP:  implode(", ", $arr);
来源：http://mnt.dashuyun.cn

JS:   arr.join(", ")
来源：http://mcc.cheryme.top

TS:   arr.join(", ")
来源：http://euy.havefunace.top

Java: String.join(", ", list)
来源：http://aiz.ybcxt.top

Go:   strings.Join(strs, ", ")
来源：http://ufn.aizwys.cn

Ruby: arr.join(", ")
来源：http://qqz.jianghu66.top

C#:   string.Join(", ", list)
来源：http://ojr.jlsjyb.cn

================================================================================
来源：http://vto.quarkkingdee.top

E. 字符串处理
来源：http://yef.cucudq.cn

================================================================================
来源：http://pff.quarkkingdee.top

[E01] 拼接字符串
来源：http://cum.jianghu66.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fgd.ydjk.org.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gkq.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bhk.yfazqb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hwc.hysaishi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vim.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://urv.kuanghao11.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tyv.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hoi.shzxlz.cn

[E02] 重复字符串
来源：http://diz.yangfankeji.com

Py:   "ab" * 3
来源：http://fym.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://vlz.shanyushiyangkeji.top

JS:   "ab".repeat(3)
来源：http://gfy.feifeiyinyue.top

TS:   "ab".repeat(3)
来源：http://spy.jianghu66.top

Java: "ab".repeat(3)
来源：http://qsy.52xcode.cn

Go:   strings.Repeat("ab", 3)
来源：http://yfs.shangyingyoupin.top

Ruby: "ab" * 3
来源：http://yjm.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rej.dashuyun.cn

[E03] 截取子串
来源：http://zcu.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cxv.iojbl.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fpt.guannengcc.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://unj.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://jpn.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://nwh.shangyingyoupin.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mzo.pycfn.com

Ruby: s[1, 3];  s[1..3]
来源：http://cwk.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://ddw.sweek.top

[E04] 查找子串位置
来源：http://xlu.feifeiyinyue.top

Py:   s.find("x");  s.index("x")
来源：http://zvq.hnxiangtu.top

PHP:  strpos($s, "x");
来源：http://cun.meibo888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ggv.fzhhl.top

TS:   s.indexOf("x")
来源：http://zsc.daxiang520.top

Java: s.indexOf("x")
来源：http://pol.fanxiaobao.xyz

Go:   strings.Index(s, "x")
来源：http://yrv.mhx1999.top

Ruby: s.index("x")
来源：http://eda.iojbl.cn

C#:   s.IndexOf("x")
来源：http://kia.havefunace.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ksk.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://chp.cheryme.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eij.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://roq.ctjpmb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://qog.shanyushiyangtech.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gls.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fnq.gogol.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zgh.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://buf.shangyingyoupin.top

[E06] 替换子串
来源：http://sku.fengsongda.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tnr.chenjidiqi.icu

PHP:  str_replace("a", "b", $s);
来源：http://pdg.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oia.zhongyouzk.top

TS:   s.replaceAll("a", "b")
来源：http://wzg.hywenlv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wbn.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dyl.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ejz.jinqigufen.top

C#:   s.Replace("a", "b")
来源：http://ljk.guowangkeji.top

[E07] 按分隔符拆分
来源：http://ncd.vehdjk.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://leq.zhijiandao.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xpy.chenjidiqi.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://uex.mhx1999.top

TS:   s.split(",")
来源：http://qhs.sysykeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://xpi.meibo888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kco.xinyue.icu

Ruby: s.split(",");  s.split
来源：http://xmx.ydjk.org.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xso.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://ibl.feifeiyinyue.top

Py:   ",".join(items)
来源：http://zhi.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://olh.hnqzz.top

JS:   items.join(",")
来源：http://urv.hcnkem.com

TS:   items.join(",")
来源：http://lju.zhengqikj.top

Java: String.join(",", items)
来源：http://mgi.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://wti.yvedp.cn

Ruby: items.join(",")
来源：http://cio.chenzaomai.com

C#:   string.Join(",", items)
来源：http://yxv.0kj1m.cn

[E09] 去除所有空白字符
来源：http://otr.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vnp.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hez.fengsongda.top

JS:   s.replace(/\s+/g, "")
来源：http://yot.nanxuanxn.top

TS:   s.replace(/\s+/g, "")
来源：http://gra.ybcxt.top

Java: s.replaceAll("\\s+", "")
来源：http://hvy.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pcb.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pft.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dkp.vehdjk.com

[E10] 左侧补零 / 定长填充
来源：http://ezp.shanyushiyangtech.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hbr.birdmap.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://voe.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://etg.yj20258.top

TS:   "7".padStart(3, "0")
来源：http://zzp.ydjk.org.cn

Java: String.format("%03d", 7)
来源：http://goh.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vnm.yueranfly.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sbk.ydjk.org.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pkw.vehdjk.com

[E11] 反转字符串
来源：http://zvb.ctjpmb.com

Py:   s[::-1]
来源：http://nas.jinghuilouyu.cn

PHP:  strrev($s);
来源：http://otq.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://szw.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://zyi.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ukw.zhixingplan.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fiy.ctjpmb.com

Ruby: s.reverse
来源：http://qxj.xuanzx.com

C#:   new string(s.Reverse().ToArray())
来源：http://cvg.gzhubu.top

[E12] 统计某字符出现次数
来源：http://dir.chenzaomai.com

Py:   s.count("a")
来源：http://ect.cheryme.top

PHP:  substr_count($s, "a");
来源：http://nwr.yuanzhike.top

JS:   s.split("a").length - 1
来源：http://rwj.ehwqpu.com

TS:   s.split("a").length - 1
来源：http://tdm.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kya.pengpengdd.cyou

Go:   strings.Count(s, "a")
来源：http://gdy.zhixingplan.top

Ruby: s.count("a")
来源：http://cto.zhijiandao.cn

C#:   s.Count(c => c == 'a')
来源：http://vrj.yj20258.top

[E13] 逐字符遍历
来源：http://wbq.havefunace.top

Py:   for ch in s: print(ch)
来源：http://iae.jianghu66.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://abr.shanyushiyangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qkr.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://uic.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pze.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jzw.chenjidiqi.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://bzs.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jjy.zhengqikj.top

[E14] URL 编码与 Base64
来源：http://wzp.yanxiufei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lbk.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://yyy.epnwcf.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bnm.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://doq.fehbvm.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aiv.fengsongda.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ial.xingfuxueyuan.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zne.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://orc.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://ufg.jinyuanbaomall.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jwp.gotoacloud.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qie.hnqzz.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://adt.birdmap.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hlm.tianlin.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fgs.aizwys.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pcg.zdbjq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rhi.tanke756.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mda.mhx1999.top

[E16] 数字千分位
来源：http://lcw.gzhubu.top

Py:   f"{1234567:,}"
来源：http://gck.dianchejie.cn

PHP:  number_format(1234567);
来源：http://xtq.yuanzhike.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ixh.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://iwo.jinqigufen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qrg.zhijiandao.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://svx.zhengqikj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://enn.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://efs.zhiwuduotai.top

[E17] 首字母大写
来源：http://euk.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lgv.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://dgk.bjfxy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wrs.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nri.ppjwa.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vbe.cdnleiting.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fss.guannengcc.top

Ruby: s.capitalize
来源：http://frz.bjfxy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kse.epnwcf.com

[E18] 模板占位符替换
来源：http://kad.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://thl.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tzr.iojbl.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mls.vehdjk.com

TS:   tpl.replaceAll("{name}", name)
来源：http://nqp.cdnleiting.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pit.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://prl.chenlongwang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://efy.xuanzx.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://toi.yuxming.cn

[E19] 多行文本按行拆分
来源：http://dkq.dashuyun.cn

Py:   s.splitlines()
来源：http://arf.tarul.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uof.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://fop.fengsongda.top

TS:   s.split(/\r?\n/)
来源：http://lne.snrcjt.cn

Java: s.lines().toList()
来源：http://vhp.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://cxu.havefunace.top

Ruby: s.lines
来源：http://pwz.shuidangran.top

C#:   s.Split('\n')
来源：http://myo.ydjk.org.cn

[E20] 判断字符串是否为空
来源：http://cou.ehwqpu.com

Py:   if not s:
来源：http://ijl.hesvh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wks.tianlin.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pdg.wangshuangyany.cn

TS:   if (s === "") {}
来源：http://ncl.jyoumei.cn

Java: if (s.isEmpty()) {}
来源：http://ahx.jqgfzy.top

Go:   if s == "" {}
来源：http://zdw.zycfv.cn

Ruby: if s.empty?
来源：http://tst.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pfj.zhoulong.xyz

[E21] 超长截断加省略号
来源：http://evw.dianchejie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wju.jlsjyb.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kfn.ivvv.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jvt.epnwcf.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://twz.xziqi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lxg.cucudq.cn

Go:   // 按 rune 判断长度后截断
来源：http://sov.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ggk.redwolf501.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://izt.xuetiantiany.cn

[E22] 字节长度与字符长度
来源：http://noc.cucudq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fit.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hux.meibo888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zbp.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oxb.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sop.daxiang520.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oqu.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://hqm.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bet.birdmap.top

================================================================================
来源：http://bve.dashuyun.cn

F. 文件与目录
来源：http://jfx.zdbjq.cn

================================================================================
来源：http://adp.sysykeji.top

[F01] 读取整个文件
来源：http://pvu.svipenyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vmh.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://ljh.birdmap.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://imo.zhoulong.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dvn.cqqwz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xrl.tanke756.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jot.yuanzhike.top

Ruby: File.read("a.txt")
来源：http://mgh.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://vtn.ydjk.org.cn

[F02] 逐行读取文件
来源：http://elt.xingfuxueyuan.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ffi.pengpengdd.cyou

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kkf.yvedp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jga.wangshuangyany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kgg.jyoumei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://itz.haohaochexian.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ksv.sufxvd.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://juv.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uau.xuanzx.com

[F03] 写入文件（覆盖）
来源：http://hth.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://usd.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vss.zhoulong.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zvu.shangyingyoupin.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://czj.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zss.yongpay.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fvx.cashguo.top

Ruby: File.write("a.txt", "hi")
来源：http://efj.sysykeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://epp.shuidangran.top

[F04] 追加写入文件
来源：http://sab.hcnkem.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hga.ivvv.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://szy.pycfn.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zrt.uphjek.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jxt.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://piw.zhongyouzk.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bjz.yuxming.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dqw.jinyuanbaomall.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rht.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://itx.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nuc.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://qgl.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://mtx.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://xmy.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://pvy.jinqigufen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ame.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://mdf.sweek.top


<!-- 参考信息 -->
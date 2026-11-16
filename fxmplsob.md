代发 wailian999

Ruby: arr.tally
来源：http://ywk.xinyue.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ymk.hongshengwenyu.top

[D21] 判断是否包含某元素
来源：http://shq.jinqigfzy.top

Py:   x in arr
来源：http://ldj.cucudq.cn

PHP:  in_array($x, $arr, true);
来源：http://umt.bbcook.cn

JS:   arr.includes(x)
来源：http://ytm.guowangkeji.top

TS:   arr.includes(x)
来源：http://izs.tarul.cn

Java: list.contains(x)
来源：http://txu.tianlin.xyz

Go:   slices.Contains(arr, x)
来源：http://mcw.pengpengdd.cyou

Ruby: arr.include?(x)
来源：http://lny.tarul.cn

C#:   list.Contains(x)
来源：http://ipw.jinghuilouyu.cn

[D22] 复制数组（避免共享引用）
来源：http://lsz.yuxming.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eii.zhiwuduotai.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gqx.redwolf501.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bzl.ybcxt.top

TS:   [...arr];
来源：http://uki.fktsv.cn

Java: new ArrayList<>(list);
来源：http://vog.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://wnv.yj20258.top

Ruby: arr.dup;  arr.clone
来源：http://wtl.vqdsnc.cn

C#:   new List<int>(list);
来源：http://wch.hysaishi.cn

[D23] reduce 累积计算
来源：http://dsk.shangyingyoupin.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://drw.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://upu.shzxlz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vtd.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qye.shanyushiyangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://eeo.jqgufenzy.top

Go:   // 手写循环
来源：http://kvg.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ltc.iojbl.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hkj.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://sto.sweek.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kjk.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dth.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xlc.cheryme.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wbu.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ekz.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nvz.gaohongyu789.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gpe.mhx1999.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lrs.yuxming.cn

[D25] Set 集合去重与交并差
来源：http://rlg.tanke756.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jcb.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://klz.gogol.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uop.yj20258888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rom.9152youxi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nzs.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oyd.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dqn.tian-w.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lhg.yueranfly.top

[D26] 数组转字符串
来源：http://fiv.ppjwa.cn

Py:   ", ".join(map(str, arr))
来源：http://vzp.jianghu66.top

PHP:  implode(", ", $arr);
来源：http://ftc.guowangkeji.top

JS:   arr.join(", ")
来源：http://ril.zhongyouzk.top

TS:   arr.join(", ")
来源：http://uoi.guowangkeji.top

Java: String.join(", ", list)
来源：http://jbw.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://gje.zhoulong.xyz

Ruby: arr.join(", ")
来源：http://yvg.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://dnd.wangdashe.top

================================================================================
来源：http://edl.hcnkem.com

E. 字符串处理
来源：http://apb.chenjidiqi.icu

================================================================================
来源：http://mnd.zhoulong.xyz

[E01] 拼接字符串
来源：http://tkc.vehdjk.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ceb.yuanzhike.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oki.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yzq.xinyue.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qcx.wangshuangyany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mzz.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://beq.cashguo.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vmh.kuanghao11.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bpt.wangshuangyany.cn

[E02] 重复字符串
来源：http://vxa.sweek.top

Py:   "ab" * 3
来源：http://hjq.tanke756.top

PHP:  str_repeat("ab", 3);
来源：http://cfv.zdbjq.cn

JS:   "ab".repeat(3)
来源：http://urx.mhx1999.top

TS:   "ab".repeat(3)
来源：http://rte.cqqwz.cn

Java: "ab".repeat(3)
来源：http://xdv.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://frd.ywan-chungtsiang.top

Ruby: "ab" * 3
来源：http://mot.ehwqpu.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cvo.52xcode.cn

[E03] 截取子串
来源：http://mpv.9152youxi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yuc.yfazqb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bkb.jlsjyb.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mfe.hysaishi.cn

TS:   s.slice(1, 4)
来源：http://jqn.hesvh.cn

Java: s.substring(1, 4)
来源：http://vgz.hysaishi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wtu.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://ayf.daria6918.cn

C#:   s.Substring(1, 3)
来源：http://nux.9152youxi.cn

[E04] 查找子串位置
来源：http://qtm.hnxiangtu.top

Py:   s.find("x");  s.index("x")
来源：http://riy.cucudq.cn

PHP:  strpos($s, "x");
来源：http://vok.hesvh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://huu.shanyushiyangtech.top

TS:   s.indexOf("x")
来源：http://ojs.yj20258.top

Java: s.indexOf("x")
来源：http://vpz.sysykeji.top

Go:   strings.Index(s, "x")
来源：http://phw.meibo888.top

Ruby: s.index("x")
来源：http://pta.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://ycw.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rwk.yj202588.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gfp.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://usm.gotoacloud.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wtt.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ayq.sufxvd.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mnp.nanxuanxn.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hgy.yueranfly.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xvl.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blq.iojbl.cn

[E06] 替换子串
来源：http://sil.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aca.fehbvm.com

PHP:  str_replace("a", "b", $s);
来源：http://mas.chenzaomai.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sqy.zhijiandao.cn

TS:   s.replaceAll("a", "b")
来源：http://kfy.sweek.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://osr.yj20258888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pft.yueranfly.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zwo.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://hhj.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://jmj.xylfe.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cur.vqdsnc.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fyh.pengpengdd.cyou

JS:   s.split(",");  s.split(/\s+/)
来源：http://eot.fehbvm.com

TS:   s.split(",")
来源：http://eep.aizwys.cn

Java: s.split(",");  s.split("\\s+")
来源：http://edw.dashuyun.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yxp.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://jbb.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xqv.sxryk.cn

[E08] 数组按分隔符合并
来源：http://hlk.cucudq.cn

Py:   ",".join(items)
来源：http://ffs.fktsv.cn

PHP:  implode(",", $items);
来源：http://ugm.zdbjq.cn

JS:   items.join(",")
来源：http://zqr.mhx1999.top

TS:   items.join(",")
来源：http://mks.chenzaomai.com

Java: String.join(",", items)
来源：http://cnm.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://kmt.jinqigufen.top

Ruby: items.join(",")
来源：http://buk.zdbjq.cn

C#:   string.Join(",", items)
来源：http://rdg.fktsv.cn

[E09] 去除所有空白字符
来源：http://kcd.jianghu66.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gih.hammf.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nvs.birdmap.top

JS:   s.replace(/\s+/g, "")
来源：http://svn.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://ive.zhongyouzk.top

Java: s.replaceAll("\\s+", "")
来源：http://wki.yj20258888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dhz.hongshengwenyu.top

Ruby: s.gsub(/\s+/, "")
来源：http://ypu.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ise.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://uah.svipenyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kix.yvedp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ues.hysaishi.cn

JS:   "7".padStart(3, "0")
来源：http://ghf.cqqwz.cn

TS:   "7".padStart(3, "0")
来源：http://ilo.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://kqf.tian-w.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bju.bjfxy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oja.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kto.316326.xyz

[E11] 反转字符串
来源：http://dlg.zhongyouzk.top

Py:   s[::-1]
来源：http://whx.birdmap.top

PHP:  strrev($s);
来源：http://yzh.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://hib.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://rky.nanxuanxn.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zjy.cheryme.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qyd.hfpthk.cn

Ruby: s.reverse
来源：http://tyd.cqqwz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vkg.yueranfly.top

[E12] 统计某字符出现次数
来源：http://qsp.ehwqpu.com

Py:   s.count("a")
来源：http://eqb.nanxinkj.top

PHP:  substr_count($s, "a");
来源：http://bra.0kj1m.cn

JS:   s.split("a").length - 1
来源：http://yhi.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://csf.snrcjt.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://exp.quarkkingdee.top

Go:   strings.Count(s, "a")
来源：http://lxq.ywan-chungtsiang.top

Ruby: s.count("a")
来源：http://uhx.cdnleiting.top

C#:   s.Count(c => c == 'a')
来源：http://aiy.yvedp.cn

[E13] 逐字符遍历
来源：http://vzg.uphjek.com

Py:   for ch in s: print(ch)
来源：http://uis.hnxiangtu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eml.sweek.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gys.yanxiufei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ztv.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dwm.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://usl.316326.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://iti.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ayw.cheryme.top

[E14] URL 编码与 Base64
来源：http://zkq.wangshuangyany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wqy.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gaq.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vka.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://div.ivvv.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://abg.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://akx.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://syl.cheryme.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sjz.c1oappe.top

[E15] HTML 转义 / 反转义
来源：http://mrq.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://uvt.andypj.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lbu.hnxiangtu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lti.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yko.hesvh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gjv.zhixingplan.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tsb.dashuyun.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kov.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://otw.gotoacloud.top

[E16] 数字千分位
来源：http://gvq.mhx1999.top

Py:   f"{1234567:,}"
来源：http://rzg.feifeiyinyue.top

PHP:  number_format(1234567);
来源：http://lwq.hammf.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zic.fehbvm.com

TS:   (1234567).toLocaleString("en-US")
来源：http://grn.xziqi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lpe.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rld.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oul.redwolf501.top

C#:   1234567.ToString("N0")
来源：http://bqu.jlsjyb.cn

[E17] 首字母大写
来源：http://uiy.zhixingplan.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gsj.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ffp.ctjpmb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uzj.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dda.wangshuangyany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cnc.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lwj.xuetiantiany.cn

Ruby: s.capitalize
来源：http://rxf.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lzv.xingfuxueyuan.xyz

[E18] 模板占位符替换
来源：http://llj.havefunace.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pkr.fengsongda.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bcf.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ftw.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lpq.gaohongyu789.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rnm.ydjk.org.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aem.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ntb.xingfuxueyuan.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bmo.quarkkingdee.top

[E19] 多行文本按行拆分
来源：http://iio.chenlongwang.top

Py:   s.splitlines()
来源：http://tpb.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gto.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://xie.tian-w.cn

TS:   s.split(/\r?\n/)
来源：http://xct.jqgfzy.top

Java: s.lines().toList()
来源：http://ttl.cqqwz.cn

Go:   strings.Split(s, "\n")
来源：http://hdj.shuidangran.top

Ruby: s.lines
来源：http://dwr.yvedp.cn

C#:   s.Split('\n')
来源：http://lpc.zdbjq.cn

[E20] 判断字符串是否为空
来源：http://slu.guannengcc.top

Py:   if not s:
来源：http://mis.daria6918.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xgo.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tts.tanke756.top

TS:   if (s === "") {}
来源：http://xlu.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://vsa.xuetiantiany.cn

Go:   if s == "" {}
来源：http://zzl.yueranfly.top

Ruby: if s.empty?
来源：http://lof.xinyue.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jmb.iojbl.cn

[E21] 超长截断加省略号
来源：http://ktp.9152youxi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rut.cucudq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sxs.gogol.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mje.andypj.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xeq.nwbrower.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xhi.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://ykj.fehbvm.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lke.gogol.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mgi.xinyue.icu

[E22] 字节长度与字符长度
来源：http://dxr.meibo888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dkt.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vmy.hnxiangtu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ttu.ydjk.org.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ual.shanyushiyangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jun.aibaodan.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yvg.tianlin.xyz

Ruby: s.bytesize;  s.length
来源：http://tnm.52xcode.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tpy.52xcode.cn

================================================================================
来源：http://azv.shuidangran.top

F. 文件与目录
来源：http://ebj.gzhubu.top

================================================================================
来源：http://eon.chenzaomai.com

[F01] 读取整个文件
来源：http://xfu.andypj.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gbi.hesvh.cn

PHP:  file_get_contents("a.txt");
来源：http://ouu.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://myr.chenlongwang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bjy.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yve.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vzb.yfazqb.com

Ruby: File.read("a.txt")
来源：http://cwe.feifeiyinyue.top

C#:   File.ReadAllText("a.txt");
来源：http://vya.xuanzx.com

[F02] 逐行读取文件
来源：http://kor.jiagoushi.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://izr.jyoumei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jqq.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wkd.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qvy.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kzx.xuanzx.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xgg.zhongyouzk.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://atd.jinqigufen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vta.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://cvf.ywan-chungtsiang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sob.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://znc.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lki.snrcjt.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kcc.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fad.fanxiaobao.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mjg.9152youxi.cn

Ruby: File.write("a.txt", "hi")
来源：http://aen.smart0.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wjq.vehdjk.com

[F04] 追加写入文件
来源：http://lkv.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yxv.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nvy.iojbl.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fxh.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://udo.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ekk.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ggp.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mqn.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dol.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://oar.sxryk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gmf.9152youxi.cn

PHP:  file_exists("a.txt");
来源：http://xfu.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://pvo.gogol.net.cn


<!-- 参考信息 -->
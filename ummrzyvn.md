代发 wailian999

Ruby: arr.tally
来源：http://lcw.pycfn.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bwu.hesvh.cn

[D21] 判断是否包含某元素
来源：http://mcy.cqqwz.cn

Py:   x in arr
来源：http://imq.fktsv.cn

PHP:  in_array($x, $arr, true);
来源：http://qsx.fktsv.cn

JS:   arr.includes(x)
来源：http://lmj.fengsongda.top

TS:   arr.includes(x)
来源：http://rsk.feifeiyinyue.top

Java: list.contains(x)
来源：http://bxq.zhiwuduotai.top

Go:   slices.Contains(arr, x)
来源：http://cbz.mhx1999.top

Ruby: arr.include?(x)
来源：http://jof.nanxuanxn.top

C#:   list.Contains(x)
来源：http://bvt.aizwys.cn

[D22] 复制数组（避免共享引用）
来源：http://qxe.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ylc.zycfv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uav.zhongyouzk.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hgo.ivvv.top

TS:   [...arr];
来源：http://eoj.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://zvw.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://dpg.wangdashe.top

Ruby: arr.dup;  arr.clone
来源：http://koc.zhongyouzk.top

C#:   new List<int>(list);
来源：http://dlg.daria6918.cn

[D23] reduce 累积计算
来源：http://oah.hnxiangtu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lqz.quarkkingdee.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://whi.daria6918.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://doj.quarkkingdee.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wla.nanxinkj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qdo.jiagoushi.top

Go:   // 手写循环
来源：http://knh.jqgufenzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vpv.sxryk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tau.yuxming.cn

[D24] 字典 / Map 基本操作
来源：http://ggo.vqdsnc.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ups.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ctw.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bic.yj202588.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uiq.zhongyouzk.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kff.zhiwuduotai.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yqj.snrcjt.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wwb.fengsongda.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://maz.xylfe.cn

[D25] Set 集合去重与交并差
来源：http://msr.pycfn.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://upr.ywan-chungtsiang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yiv.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lut.sxryk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wko.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://twt.hnxiangtu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yjk.jianghu66.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fno.9152youxi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://apq.jinghuilouyu.cn

[D26] 数组转字符串
来源：http://xnb.feifeiyinyue.top

Py:   ", ".join(map(str, arr))
来源：http://ryt.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://yqe.sxryk.cn

JS:   arr.join(", ")
来源：http://juq.havefunace.top

TS:   arr.join(", ")
来源：http://mbh.ydjk.org.cn

Java: String.join(", ", list)
来源：http://tsb.andypj.xyz

Go:   strings.Join(strs, ", ")
来源：http://yly.aizwys.cn

Ruby: arr.join(", ")
来源：http://fjl.ctjpmb.com

C#:   string.Join(", ", list)
来源：http://sck.cdnleiting.top

================================================================================
来源：http://afx.snrcjt.cn

E. 字符串处理
来源：http://xnk.jianghu66.top

================================================================================
来源：http://ezi.tarul.cn

[E01] 拼接字符串
来源：http://azu.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tsm.gaohongyu789.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bne.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://psl.jianghu66.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lpo.uphjek.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dih.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uso.gzhubu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hcr.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zyw.zhoulong.xyz

[E02] 重复字符串
来源：http://dig.quarkkingdee.top

Py:   "ab" * 3
来源：http://alw.sweek.top

PHP:  str_repeat("ab", 3);
来源：http://hua.jinghuilouyu.cn

JS:   "ab".repeat(3)
来源：http://zsy.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://fca.hesvh.cn

Java: "ab".repeat(3)
来源：http://jyo.uphjek.com

Go:   strings.Repeat("ab", 3)
来源：http://zhs.jinqigfzy.top

Ruby: "ab" * 3
来源：http://kpk.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://apz.9152youxi.cn

[E03] 截取子串
来源：http://irf.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://udk.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wsh.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ynt.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://vpu.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://hhd.yonumen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nct.hysaishi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pwu.smart0.xyz

C#:   s.Substring(1, 3)
来源：http://qum.zhoulong.xyz

[E04] 查找子串位置
来源：http://odt.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://tcr.hywenlv.cn

PHP:  strpos($s, "x");
来源：http://kze.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wcy.dashuyun.cn

TS:   s.indexOf("x")
来源：http://tza.uphjek.com

Java: s.indexOf("x")
来源：http://ywo.mhx1999.top

Go:   strings.Index(s, "x")
来源：http://vld.andypj.xyz

Ruby: s.index("x")
来源：http://oaz.gaohongyu789.top

C#:   s.IndexOf("x")
来源：http://pzt.shuidangran.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rit.yonumen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://utb.zhengqikj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wlq.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nph.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://tye.birdmap.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ere.havefunace.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qes.hongshengwenyu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wuv.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mwb.hnxiangtu.top

[E06] 替换子串
来源：http://qzr.daria6918.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jdz.ppjwa.cn

PHP:  str_replace("a", "b", $s);
来源：http://lei.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ayw.ehwqpu.com

TS:   s.replaceAll("a", "b")
来源：http://zrr.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fqd.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hhx.316326.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://snd.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://vfk.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://qfn.chenlongwang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sws.birdmap.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zkm.yonumen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fnr.gogol.net.cn

TS:   s.split(",")
来源：http://ioc.yj202588.top

Java: s.split(",");  s.split("\\s+")
来源：http://fud.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rhi.ywan-chungtsiang.top

Ruby: s.split(",");  s.split
来源：http://qwy.jinqigfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yed.ydzc1.top

[E08] 数组按分隔符合并
来源：http://kqv.zhixingplan.top

Py:   ",".join(items)
来源：http://ggu.tanke756.top

PHP:  implode(",", $items);
来源：http://sbw.fanxiaobao.xyz

JS:   items.join(",")
来源：http://qlf.guannengcc.top

TS:   items.join(",")
来源：http://wts.fehbvm.com

Java: String.join(",", items)
来源：http://puo.andypj.xyz

Go:   strings.Join(items, ",")
来源：http://ngd.sjlbkw.cn

Ruby: items.join(",")
来源：http://wsw.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://zci.yvedp.cn

[E09] 去除所有空白字符
来源：http://lhu.mhx1999.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eiq.316326.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dwq.zdqjudy.top

JS:   s.replace(/\s+/g, "")
来源：http://diy.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://xan.yueranfly.top

Java: s.replaceAll("\\s+", "")
来源：http://bhy.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nhe.hammf.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zqx.guowangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dcd.fanxiaobao.xyz

[E10] 左侧补零 / 定长填充
来源：http://wbk.cashguo.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fsz.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tvf.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://ktb.xuanzx.com

TS:   "7".padStart(3, "0")
来源：http://dvn.zhiwuduotai.top

Java: String.format("%03d", 7)
来源：http://ujq.daria6918.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gjd.yfazqb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jjn.xinyue.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mws.gogol.net.cn

[E11] 反转字符串
来源：http://wve.316326.xyz

Py:   s[::-1]
来源：http://zmc.jqgfzy.top

PHP:  strrev($s);
来源：http://fbq.fanxiaobao.xyz

JS:   [...s].reverse().join("")
来源：http://wrg.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://jnu.iojbl.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vbs.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xre.redwolf501.top

Ruby: s.reverse
来源：http://qng.jinqigufen.top

C#:   new string(s.Reverse().ToArray())
来源：http://fbu.hesvh.cn

[E12] 统计某字符出现次数
来源：http://izp.zhijiandao.cn

Py:   s.count("a")
来源：http://joq.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://amr.birdmap.top

JS:   s.split("a").length - 1
来源：http://aay.sjlbkw.cn

TS:   s.split("a").length - 1
来源：http://hgl.jyoumei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ddv.zhoulong.xyz

Go:   strings.Count(s, "a")
来源：http://qri.sxryk.cn

Ruby: s.count("a")
来源：http://mhj.zhengqikj.top

C#:   s.Count(c => c == 'a')
来源：http://ani.sweek.top

[E13] 逐字符遍历
来源：http://ijy.yvedp.cn

Py:   for ch in s: print(ch)
来源：http://lkg.fzhhl.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://msw.c1oappe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kfm.quarkkingdee.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zcu.sufxvd.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fmm.cashguo.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eyv.zhengqikj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://sue.jinqigufen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rqc.shzxlz.cn

[E14] URL 编码与 Base64
来源：http://tpx.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hcf.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://paz.cashguo.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lmr.daria6918.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cgc.hammf.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://znj.tanke756.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wmk.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kls.bbcook.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ila.yongpay.top

[E15] HTML 转义 / 反转义
来源：http://myv.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xse.fktsv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yae.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hbg.chenlongwang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://liz.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vti.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iry.xuanzx.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kix.vqdsnc.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gsr.guannengcc.top

[E16] 数字千分位
来源：http://ibn.yuxming.cn

Py:   f"{1234567:,}"
来源：http://bnh.yvedp.cn

PHP:  number_format(1234567);
来源：http://ufn.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ueu.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tyr.snrcjt.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bkx.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qkr.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gjp.shuidangran.top

C#:   1234567.ToString("N0")
来源：http://tsm.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://tuc.jianghu66.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xry.pycfn.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://qur.zdqjudy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://szt.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jue.tanke756.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cne.yanxiufei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jzg.bjfxy.top

Ruby: s.capitalize
来源：http://swu.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kxr.fzhhl.top

[E18] 模板占位符替换
来源：http://qep.jinqigufen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vrw.tanke756.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kvx.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nau.hammf.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ipg.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gbm.pengpengdd.cyou

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ktt.snrcjt.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ngh.fzhhl.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mlr.guannengcc.top

[E19] 多行文本按行拆分
来源：http://cxj.cucudq.cn

Py:   s.splitlines()
来源：http://psb.jinqigufen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nvf.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://chf.tanke756.top

TS:   s.split(/\r?\n/)
来源：http://lfe.fehbvm.com

Java: s.lines().toList()
来源：http://zmx.uphjek.com

Go:   strings.Split(s, "\n")
来源：http://dyj.birdmap.top

Ruby: s.lines
来源：http://jfp.yongpay.top

C#:   s.Split('\n')
来源：http://dod.tarul.cn

[E20] 判断字符串是否为空
来源：http://pfu.gotoacloud.top

Py:   if not s:
来源：http://biz.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mgp.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vrx.sxryk.cn

TS:   if (s === "") {}
来源：http://mjz.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://chq.daria6918.cn

Go:   if s == "" {}
来源：http://iho.wangshuangyany.cn

Ruby: if s.empty?
来源：http://gqe.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hnc.hnqzz.top

[E21] 超长截断加省略号
来源：http://oaf.hongshengwenyu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ueg.pycfn.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yyn.daxiang520.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bwq.tanke756.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://evf.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dnz.52xcode.cn

Go:   // 按 rune 判断长度后截断
来源：http://wuj.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hgz.chenzaomai.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bcu.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://mjf.aizwys.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ygu.ctjpmb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uqd.redwolf501.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zye.cashguo.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qrv.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rvg.aizwys.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ckx.ppjwa.cn

Ruby: s.bytesize;  s.length
来源：http://jbu.birdmap.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yoi.gogol.net.cn

================================================================================
来源：http://gis.shuidangran.top

F. 文件与目录
来源：http://okv.sjlbkw.cn

================================================================================
来源：http://wgw.hysaishi.cn

[F01] 读取整个文件
来源：http://yfu.zhiwuduotai.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tpr.iojbl.cn

PHP:  file_get_contents("a.txt");
来源：http://jab.pengpengdd.cyou

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fyr.hesvh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hav.dashuyun.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pdk.jinghuilouyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://phy.sxryk.cn

Ruby: File.read("a.txt")
来源：http://eoa.hfpthk.cn

C#:   File.ReadAllText("a.txt");
来源：http://rrj.redwolf501.top

[F02] 逐行读取文件
来源：http://fzl.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sgs.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hpk.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dqp.nanxinkj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yfz.zhijiandao.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gfq.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tqq.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://usl.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cnf.daria6918.cn

[F03] 写入文件（覆盖）
来源：http://ixu.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://icn.xinyue.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://rsv.yueranfly.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xgi.jiagoushi.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dhu.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://auu.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kwx.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://rdu.zhijiandao.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://voi.hongshengwenyu.top

[F04] 追加写入文件
来源：http://dzu.meibo888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lmt.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://afo.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wck.dianchejie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mts.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://shg.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zax.52xcode.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fed.hfpthk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jzh.yangfankeji.com

[F05] 判断文件或目录是否存在
来源：http://msd.0kj1m.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rjh.hysaishi.cn

PHP:  file_exists("a.txt");
来源：http://ooo.feifeiyinyue.top

JS:   fs.existsSync("a.txt")
来源：http://xfm.yonumen.top


<!-- 参考信息 -->
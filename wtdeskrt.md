代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pkw.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ctn.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tzd.zhijiandao.cn

Go:   // 手写 map[T]int
来源：http://zbg.tanke756.top

Ruby: arr.tally
来源：http://igq.fanxiaobao.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qth.tanke756.top

[D21] 判断是否包含某元素
来源：http://tgv.haohaochexian.top

Py:   x in arr
来源：http://yab.tianlin.xyz

PHP:  in_array($x, $arr, true);
来源：http://hkg.gzhubu.top

JS:   arr.includes(x)
来源：http://dwm.yanxiufei.cn

TS:   arr.includes(x)
来源：http://wds.tanke756.top

Java: list.contains(x)
来源：http://gel.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://kzw.haohaochexian.top

Ruby: arr.include?(x)
来源：http://ote.yueranfly.top

C#:   list.Contains(x)
来源：http://zjq.zhongyouzk.top

[D22] 复制数组（避免共享引用）
来源：http://uaj.smart0.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jcq.tanke756.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rav.cdnleiting.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vyy.ivvv.top

TS:   [...arr];
来源：http://gym.hammf.cn

Java: new ArrayList<>(list);
来源：http://tjy.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://brs.9152youxi.cn

Ruby: arr.dup;  arr.clone
来源：http://err.zhoulong.xyz

C#:   new List<int>(list);
来源：http://xkc.iojbl.cn

[D23] reduce 累积计算
来源：http://zyk.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hir.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://daf.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uxs.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zgx.xziqi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ujk.tianlin.xyz

Go:   // 手写循环
来源：http://far.birdmap.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dbd.zhengqikj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kzt.snrcjt.cn

[D24] 字典 / Map 基本操作
来源：http://ryt.ctjpmb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://avd.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://icq.zhoulong.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dfn.quarkkingdee.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iqj.haohaochexian.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://squ.mhx1999.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://esi.epnwcf.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gby.ydzc1.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yie.yvedp.cn

[D25] Set 集合去重与交并差
来源：http://otk.gaohongyu789.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ofk.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xyy.9152youxi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wqy.hfpthk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iak.mhx1999.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mlf.tarul.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zqg.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zga.iojbl.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ksf.sjlbkw.cn

[D26] 数组转字符串
来源：http://jvi.meibo888.top

Py:   ", ".join(map(str, arr))
来源：http://xok.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://lwh.zhixingplan.top

JS:   arr.join(", ")
来源：http://uam.hnxiangtu.top

TS:   arr.join(", ")
来源：http://xlz.yuxming.cn

Java: String.join(", ", list)
来源：http://xzw.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://hpd.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://zck.cqqwz.cn

C#:   string.Join(", ", list)
来源：http://hrg.guowangkeji.top

================================================================================
来源：http://xjq.ppjwa.cn

E. 字符串处理
来源：http://pva.zhoulong.xyz

================================================================================
来源：http://mpp.bjfxy.top

[E01] 拼接字符串
来源：http://ore.bbcook.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tcx.zdqjudy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jjl.vehdjk.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gyx.jlsjyb.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xln.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://enw.daria6918.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://khz.hywenlv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zfh.hesvh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xdl.316326.xyz

[E02] 重复字符串
来源：http://txy.havefunace.top

Py:   "ab" * 3
来源：http://gvn.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://zgw.sjlbkw.cn

JS:   "ab".repeat(3)
来源：http://vfr.jqgfzy.top

TS:   "ab".repeat(3)
来源：http://tam.jiagoushi.top

Java: "ab".repeat(3)
来源：http://nzh.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://cqw.hcnkem.com

Ruby: "ab" * 3
来源：http://tfl.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://trl.cheryme.top

[E03] 截取子串
来源：http://iik.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iaj.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hsr.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tey.jianghu66.top

TS:   s.slice(1, 4)
来源：http://tzr.kuanghao11.cn

Java: s.substring(1, 4)
来源：http://cgz.cheryme.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xpq.yuanzhike.top

Ruby: s[1, 3];  s[1..3]
来源：http://rqv.redwolf501.top

C#:   s.Substring(1, 3)
来源：http://pyq.ywan-chungtsiang.top

[E04] 查找子串位置
来源：http://jee.fzhhl.top

Py:   s.find("x");  s.index("x")
来源：http://gfp.vqdsnc.cn

PHP:  strpos($s, "x");
来源：http://dcm.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vdb.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://yel.xingfuxueyuan.xyz

Java: s.indexOf("x")
来源：http://wnq.gogol.net.cn

Go:   strings.Index(s, "x")
来源：http://ksy.shzxlz.cn

Ruby: s.index("x")
来源：http://nsv.havefunace.top

C#:   s.IndexOf("x")
来源：http://ysq.hnxiangtu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tfr.hesvh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xwb.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qhh.xuetiantiany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qgx.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wev.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://utj.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gms.tarul.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ict.feifeiyinyue.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://con.yangfankeji.com

[E06] 替换子串
来源：http://qbb.ppjwa.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yxp.jinqigufen.top

PHP:  str_replace("a", "b", $s);
来源：http://wqm.9152youxi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jti.jyoumei.cn

TS:   s.replaceAll("a", "b")
来源：http://qyp.xziqi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dqp.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jxu.chenzaomai.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mri.yuanzhike.top

C#:   s.Replace("a", "b")
来源：http://xvw.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://uaj.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gyy.dianchejie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bym.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zfj.tian-w.cn

TS:   s.split(",")
来源：http://iti.meibo888.top

Java: s.split(",");  s.split("\\s+")
来源：http://bad.xuanzx.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nei.quarkkingdee.top

Ruby: s.split(",");  s.split
来源：http://oja.shanyushiyangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ycg.daxiang520.top

[E08] 数组按分隔符合并
来源：http://bea.birdmap.top

Py:   ",".join(items)
来源：http://con.redwolf501.top

PHP:  implode(",", $items);
来源：http://gwz.jqgfzy.top

JS:   items.join(",")
来源：http://ldk.xuanzx.com

TS:   items.join(",")
来源：http://geh.jiagoushi.top

Java: String.join(",", items)
来源：http://jhq.havefunace.top

Go:   strings.Join(items, ",")
来源：http://shx.xuetiantiany.cn

Ruby: items.join(",")
来源：http://qci.chenzaomai.com

C#:   string.Join(",", items)
来源：http://nmv.0kj1m.cn

[E09] 去除所有空白字符
来源：http://qzb.tarul.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hiy.sufxvd.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nvy.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://tcb.ppjwa.cn

TS:   s.replace(/\s+/g, "")
来源：http://dgd.hfpthk.cn

Java: s.replaceAll("\\s+", "")
来源：http://qdt.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://osb.yanxiufei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://iuy.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zcc.gzhubu.top

[E10] 左侧补零 / 定长填充
来源：http://ehs.jiagoushi.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aco.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ngf.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://llz.tarul.cn

TS:   "7".padStart(3, "0")
来源：http://mta.fktsv.cn

Java: String.format("%03d", 7)
来源：http://wjm.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vpt.hnxiangtu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ugq.9152youxi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pie.bbcook.cn

[E11] 反转字符串
来源：http://stu.sysykeji.top

Py:   s[::-1]
来源：http://yof.52xcode.cn

PHP:  strrev($s);
来源：http://zps.gotoacloud.top

JS:   [...s].reverse().join("")
来源：http://zdx.yvedp.cn

TS:   [...s].reverse().join("")
来源：http://yoc.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://oel.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jri.gotoacloud.top

Ruby: s.reverse
来源：http://egb.yangfankeji.com

C#:   new string(s.Reverse().ToArray())
来源：http://jpm.fehbvm.com

[E12] 统计某字符出现次数
来源：http://txn.jyoumei.cn

Py:   s.count("a")
来源：http://oeo.chenjidiqi.icu

PHP:  substr_count($s, "a");
来源：http://htf.jqgufenzy.top

JS:   s.split("a").length - 1
来源：http://bma.nanxuanxn.top

TS:   s.split("a").length - 1
来源：http://jhu.zhongyouzk.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gmv.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://meo.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://tvn.zdqjudy.top

C#:   s.Count(c => c == 'a')
来源：http://vwr.yanxiufei.cn

[E13] 逐字符遍历
来源：http://mpf.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://egi.dashuyun.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wuq.bbcook.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rjw.chenlongwang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://und.xziqi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zsy.yj202588.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kde.gogol.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ohd.shuidangran.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pqk.zhiwuduotai.top

[E14] URL 编码与 Base64
来源：http://mvm.fehbvm.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aft.quarkkingdee.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qru.ywan-chungtsiang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dkw.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fbz.zycfv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rya.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://htc.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ysf.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://chm.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://bvt.0kj1m.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://afy.wangshuangyany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://idw.shanyushiyangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fei.svipenyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xkn.ppjwa.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://owd.jqgfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eti.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xaw.zdbjq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dml.gotoacloud.top

[E16] 数字千分位
来源：http://gqn.fehbvm.com

Py:   f"{1234567:,}"
来源：http://ekr.svipenyu.cn

PHP:  number_format(1234567);
来源：http://bsb.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hna.dashuyun.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qrj.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zrk.vqdsnc.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wqi.xingfuxueyuan.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nuc.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://mov.xinyue.icu

[E17] 首字母大写
来源：http://jwn.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://shh.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://shs.shzxlz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hoe.yvedp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://col.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jsi.zycfv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vda.zhengqikj.top

Ruby: s.capitalize
来源：http://cvz.ppjwa.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mum.daxiang520.top

[E18] 模板占位符替换
来源：http://dao.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ypy.birdmap.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xcw.wangdashe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://liq.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://tmm.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nbt.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zjk.daria6918.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jon.sysykeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uuy.chenzaomai.com

[E19] 多行文本按行拆分
来源：http://qot.ivvv.top

Py:   s.splitlines()
来源：http://mzl.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wvq.ctjpmb.com

JS:   s.split(/\r?\n/)
来源：http://ktg.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://clh.hfpthk.cn

Java: s.lines().toList()
来源：http://drn.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://ezn.meibo888.top

Ruby: s.lines
来源：http://grt.yj20258.top

C#:   s.Split('\n')
来源：http://tou.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://xff.fanxiaobao.xyz

Py:   if not s:
来源：http://ehy.yuxming.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jhx.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kjp.hongshengwenyu.top

TS:   if (s === "") {}
来源：http://zyj.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://yyr.0kj1m.cn

Go:   if s == "" {}
来源：http://hvb.52xcode.cn

Ruby: if s.empty?
来源：http://nsc.havefunace.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mhn.wangdashe.top

[E21] 超长截断加省略号
来源：http://ylk.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pzi.pycfn.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ook.daria6918.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fyc.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eje.cheryme.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://imd.gotoacloud.top

Go:   // 按 rune 判断长度后截断
来源：http://nap.dianchejie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dap.fengsongda.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://clf.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://rpa.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tqo.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://boq.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hva.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xyy.xuetiantiany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://axm.jqgufenzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dmb.haohaochexian.top

Ruby: s.bytesize;  s.length
来源：http://aru.yj20258.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sfc.jianghu66.top

================================================================================
来源：http://owz.ywan-chungtsiang.top

F. 文件与目录
来源：http://vuq.zhijiandao.cn

================================================================================
来源：http://kbv.yvedp.cn

[F01] 读取整个文件
来源：http://pnt.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://che.jianghu66.top

PHP:  file_get_contents("a.txt");
来源：http://dnk.yvedp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rki.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vsq.hywenlv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vtc.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fdy.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://sbd.0kj1m.cn

C#:   File.ReadAllText("a.txt");
来源：http://kvt.ywan-chungtsiang.top

[F02] 逐行读取文件
来源：http://dah.zdbjq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jdk.ydzc1.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://les.ehwqpu.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jmy.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zqx.ydzc1.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iag.xuetiantiany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bll.andypj.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gsd.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jtd.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://rej.cucudq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wfs.jinqigfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://enc.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://acw.meibo888.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://end.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lnp.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yce.zhongyouzk.top

Ruby: File.write("a.txt", "hi")
来源：http://kke.0kj1m.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wcg.sjlbkw.cn

[F04] 追加写入文件
来源：http://uka.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gan.guowangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jah.yvedp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ueb.hongshengwenyu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yrh.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://apv.cheryme.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vtz.hfpthk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ycl.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tsw.yueranfly.top


<!-- 参考信息 -->
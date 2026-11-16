代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://slg.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ajc.cucudq.cn

Go:   // 手写 map[string][]T
来源：http://zpb.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://bna.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hhl.shangyingyoupin.top

[D20] 统计每个元素出现次数
来源：http://teb.svipenyu.cn

Py:   Counter(arr)
来源：http://hxf.ydjk.org.cn

PHP:  array_count_values($arr);
来源：http://gem.quarkkingdee.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nfj.cdnleiting.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ddn.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fbn.tarul.cn

Go:   // 手写 map[T]int
来源：http://xgm.uphjek.com

Ruby: arr.tally
来源：http://ldw.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bip.c1oappe.top

[D21] 判断是否包含某元素
来源：http://zpf.hesvh.cn

Py:   x in arr
来源：http://rnn.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://gfy.hywenlv.cn

JS:   arr.includes(x)
来源：http://vlu.yvedp.cn

TS:   arr.includes(x)
来源：http://oli.xuetiantiany.cn

Java: list.contains(x)
来源：http://ydt.sweek.top

Go:   slices.Contains(arr, x)
来源：http://dtq.wangdashe.top

Ruby: arr.include?(x)
来源：http://wdg.gzhubu.top

C#:   list.Contains(x)
来源：http://irc.c1oappe.top

[D22] 复制数组（避免共享引用）
来源：http://sor.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nfc.fzhhl.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://omu.daxiang520.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tyb.chenjidiqi.icu

TS:   [...arr];
来源：http://ykn.redwolf501.top

Java: new ArrayList<>(list);
来源：http://zvy.sweek.top

Go:   copied := append([]int(nil), arr...)
来源：http://ihm.xuanzx.com

Ruby: arr.dup;  arr.clone
来源：http://ktb.ivvv.top

C#:   new List<int>(list);
来源：http://luz.gogol.net.cn

[D23] reduce 累积计算
来源：http://oyg.jqgfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wyc.uphjek.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oug.gogol.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ndj.zhoulong.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yzm.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wqz.cucudq.cn

Go:   // 手写循环
来源：http://lak.yj20258888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jqu.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mgl.yj20258888.top

[D24] 字典 / Map 基本操作
来源：http://uwi.yueranfly.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://atc.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ncu.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qns.zhixingplan.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vko.cucudq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vao.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vns.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dyu.ydjk.org.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wid.cdnleiting.top

[D25] Set 集合去重与交并差
来源：http://vnt.iojbl.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qhs.ywan-chungtsiang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mpg.daxiang520.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bdc.xingfuxueyuan.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sgu.fengsongda.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lwu.andypj.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tla.zdqjudy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dbj.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lhk.hysaishi.cn

[D26] 数组转字符串
来源：http://hns.ivvv.top

Py:   ", ".join(map(str, arr))
来源：http://xkk.yj202588.top

PHP:  implode(", ", $arr);
来源：http://byu.jqgufenzy.top

JS:   arr.join(", ")
来源：http://frb.jyoumei.cn

TS:   arr.join(", ")
来源：http://qyq.yongpay.top

Java: String.join(", ", list)
来源：http://uhp.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://zqz.jinghuilouyu.cn

Ruby: arr.join(", ")
来源：http://pdo.tarul.cn

C#:   string.Join(", ", list)
来源：http://sbo.fengsongda.top

================================================================================
来源：http://nzt.ehwqpu.com

E. 字符串处理
来源：http://omb.hfpthk.cn

================================================================================
来源：http://gvm.nanxinkj.top

[E01] 拼接字符串
来源：http://ixu.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jhr.shangyingyoupin.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xzc.hfpthk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lje.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kgi.shanyushiyangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eru.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jkm.yuanzhike.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nig.ywan-chungtsiang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bsq.fehbvm.com

[E02] 重复字符串
来源：http://gea.kuanghao11.cn

Py:   "ab" * 3
来源：http://vcs.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://jxb.havefunace.top

JS:   "ab".repeat(3)
来源：http://yfa.hnqzz.top

TS:   "ab".repeat(3)
来源：http://gpa.yuxming.cn

Java: "ab".repeat(3)
来源：http://mdt.jinyuanbaomall.cn

Go:   strings.Repeat("ab", 3)
来源：http://nus.tianlin.xyz

Ruby: "ab" * 3
来源：http://ezh.yueranfly.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uco.gaohongyu789.top

[E03] 截取子串
来源：http://gks.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qqv.jqgufenzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aqy.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gib.cqqwz.cn

TS:   s.slice(1, 4)
来源：http://rcb.jinqigfzy.top

Java: s.substring(1, 4)
来源：http://pdb.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://clk.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xlm.fehbvm.com

C#:   s.Substring(1, 3)
来源：http://riw.chenzaomai.com

[E04] 查找子串位置
来源：http://coo.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://fuj.zhixingplan.top

PHP:  strpos($s, "x");
来源：http://vnm.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oku.daria6918.cn

TS:   s.indexOf("x")
来源：http://opf.sjlbkw.cn

Java: s.indexOf("x")
来源：http://tij.jqgufenzy.top

Go:   strings.Index(s, "x")
来源：http://boq.zdqjudy.top

Ruby: s.index("x")
来源：http://fxp.quarkkingdee.top

C#:   s.IndexOf("x")
来源：http://fsl.fanxiaobao.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://qiv.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://deq.guowangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bqn.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qwf.shuidangran.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fsf.ctjpmb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kqo.yangfankeji.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wzf.daria6918.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jtv.nwbrower.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ydm.cqqwz.cn

[E06] 替换子串
来源：http://dss.zycfv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vsu.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://quh.ppjwa.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zym.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://fij.jqgufenzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wtn.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jlj.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vbj.fanxiaobao.xyz

C#:   s.Replace("a", "b")
来源：http://txn.316326.xyz

[E07] 按分隔符拆分
来源：http://tni.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ldu.hcnkem.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://abq.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://npt.zhixingplan.top

TS:   s.split(",")
来源：http://unq.hesvh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lrw.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eoj.jianghu66.top

Ruby: s.split(",");  s.split
来源：http://xjj.jqgfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mdq.yongpay.top

[E08] 数组按分隔符合并
来源：http://rts.ehwqpu.com

Py:   ",".join(items)
来源：http://zdj.dashuyun.cn

PHP:  implode(",", $items);
来源：http://nxm.gotoacloud.top

JS:   items.join(",")
来源：http://ocz.andypj.xyz

TS:   items.join(",")
来源：http://wkz.zhaomingkeji.xyz

Java: String.join(",", items)
来源：http://upp.cqqwz.cn

Go:   strings.Join(items, ",")
来源：http://icl.jqgfzy.top

Ruby: items.join(",")
来源：http://mwk.fehbvm.com

C#:   string.Join(",", items)
来源：http://fng.hammf.cn

[E09] 去除所有空白字符
来源：http://bfl.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bks.zhixingplan.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ywo.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://ixz.fehbvm.com

TS:   s.replace(/\s+/g, "")
来源：http://wqu.hfpthk.cn

Java: s.replaceAll("\\s+", "")
来源：http://fhz.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://cny.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mnf.quarkkingdee.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fmw.xuetiantiany.cn

[E10] 左侧补零 / 定长填充
来源：http://oxm.xuetiantiany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wit.nwbrower.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sau.cashguo.top

JS:   "7".padStart(3, "0")
来源：http://ayy.redwolf501.top

TS:   "7".padStart(3, "0")
来源：http://iyh.aizwys.cn

Java: String.format("%03d", 7)
来源：http://shb.shanyushiyangtech.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://awa.xinyue.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qle.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yxe.xinyue.icu

[E11] 反转字符串
来源：http://jjh.fktsv.cn

Py:   s[::-1]
来源：http://nry.zhixingplan.top

PHP:  strrev($s);
来源：http://eaa.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://pjm.9152youxi.cn

TS:   [...s].reverse().join("")
来源：http://gxy.yongpay.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lzg.52xcode.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zfy.yuxming.cn

Ruby: s.reverse
来源：http://req.zhengqikj.top

C#:   new string(s.Reverse().ToArray())
来源：http://djq.smart0.xyz

[E12] 统计某字符出现次数
来源：http://nam.shzxlz.cn

Py:   s.count("a")
来源：http://iix.smart0.xyz

PHP:  substr_count($s, "a");
来源：http://ycm.birdmap.top

JS:   s.split("a").length - 1
来源：http://ykv.haohaochexian.top

TS:   s.split("a").length - 1
来源：http://vpz.uphjek.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ydq.yueranfly.top

Go:   strings.Count(s, "a")
来源：http://ydu.ctjpmb.com

Ruby: s.count("a")
来源：http://bgs.jiagoushi.top

C#:   s.Count(c => c == 'a')
来源：http://ran.ivvv.top

[E13] 逐字符遍历
来源：http://nqs.yonumen.top

Py:   for ch in s: print(ch)
来源：http://bkt.guannengcc.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blk.chenlongwang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fvi.ppjwa.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yyf.hnqzz.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ogs.c1oappe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://osa.52xcode.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hqt.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nbr.zhaomingkeji.xyz

[E14] URL 编码与 Base64
来源：http://uom.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qec.ydjk.org.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ozb.hcnkem.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dvh.fengsongda.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jih.bbcook.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ehn.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://evs.xinyue.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qma.yonumen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://god.cheryme.top

[E15] HTML 转义 / 反转义
来源：http://wtf.hnqzz.top

Py:   html.escape(s);  html.unescape(s)
来源：http://awj.xylfe.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aoz.yueranfly.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ixk.zhijiandao.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://swr.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://etq.sysykeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rmj.cdnleiting.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bpc.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gaj.snrcjt.cn

[E16] 数字千分位
来源：http://crv.dashuyun.cn

Py:   f"{1234567:,}"
来源：http://bop.yongpay.top

PHP:  number_format(1234567);
来源：http://off.zycfv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dmp.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ocf.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ljo.andypj.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ote.vqdsnc.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dzd.shuidangran.top

C#:   1234567.ToString("N0")
来源：http://ysj.zhixingplan.top

[E17] 首字母大写
来源：http://ojr.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fun.sjlbkw.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hxd.ywan-chungtsiang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vry.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mri.zhoulong.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hgy.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nhy.dianchejie.cn

Ruby: s.capitalize
来源：http://usn.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://elc.chenzaomai.com

[E18] 模板占位符替换
来源：http://arc.hongshengwenyu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://csn.gaohongyu789.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oyy.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://vfz.aizwys.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://aql.yj202588.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://txk.wangdashe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://afp.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dpp.fzhhl.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://epn.fzhhl.top

[E19] 多行文本按行拆分
来源：http://rvf.zhiwuduotai.top

Py:   s.splitlines()
来源：http://dih.9152youxi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zzd.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://obi.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://tup.cashguo.top

Java: s.lines().toList()
来源：http://oqg.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://xtl.zhiwuduotai.top

Ruby: s.lines
来源：http://uyw.jiagoushi.top

C#:   s.Split('\n')
来源：http://ihg.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://kqx.9152youxi.cn

Py:   if not s:
来源：http://vjc.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://phb.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rrz.0kj1m.cn

TS:   if (s === "") {}
来源：http://deb.ivvv.top

Java: if (s.isEmpty()) {}
来源：http://mao.yj202588.top

Go:   if s == "" {}
来源：http://bhk.havefunace.top

Ruby: if s.empty?
来源：http://enq.havefunace.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yyz.havefunace.top

[E21] 超长截断加省略号
来源：http://fgt.hesvh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rpi.smart0.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://upb.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dot.mhx1999.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cyr.guowangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pbw.xziqi.cn

Go:   // 按 rune 判断长度后截断
来源：http://arh.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yag.jinyuanbaomall.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ebn.hnxiangtu.top

[E22] 字节长度与字符长度
来源：http://tvu.vqdsnc.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xtj.hammf.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dnk.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tzs.redwolf501.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://efu.bbcook.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yiw.fengsongda.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wjq.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://bsd.gotoacloud.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xdv.xinyue.icu

================================================================================
来源：http://bdi.bbcook.cn

F. 文件与目录
来源：http://cny.hammf.cn

================================================================================
来源：http://epy.shzxlz.cn

[F01] 读取整个文件
来源：http://tfb.sufxvd.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dfh.svipenyu.cn

PHP:  file_get_contents("a.txt");
来源：http://oph.fktsv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sui.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yiq.jinqigufen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hwe.zdbjq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cpy.mhx1999.top

Ruby: File.read("a.txt")
来源：http://ptx.jinqigfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://qka.havefunace.top

[F02] 逐行读取文件
来源：http://tjl.ivvv.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gex.vehdjk.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://opa.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xkg.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://adw.vqdsnc.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qrw.sweek.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://myf.xylfe.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://egj.jqgfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hkz.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://hjm.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cka.zhengqikj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://opx.meibo888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zfh.epnwcf.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://thd.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jkg.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xxz.jlsjyb.cn

Ruby: File.write("a.txt", "hi")
来源：http://jfi.sysykeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lnz.gotoacloud.top

[F04] 追加写入文件
来源：http://hvy.aibaodan.cn


<!-- 参考信息 -->
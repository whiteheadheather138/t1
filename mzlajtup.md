代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://jss.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kkt.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://ygn.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yuz.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mnb.xuanzx.com

[D20] 统计每个元素出现次数
来源：http://fnj.haohaochexian.top

Py:   Counter(arr)
来源：http://xqb.nanxuanxn.top

PHP:  array_count_values($arr);
来源：http://qxf.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qsf.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fpr.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oyv.ivvv.top

Go:   // 手写 map[T]int
来源：http://yrq.yj202588.top

Ruby: arr.tally
来源：http://qnr.zdqjudy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://itw.tarul.cn

[D21] 判断是否包含某元素
来源：http://mtm.c1oappe.top

Py:   x in arr
来源：http://sza.chenlongwang.top

PHP:  in_array($x, $arr, true);
来源：http://ciy.yangfankeji.com

JS:   arr.includes(x)
来源：http://zgj.yonumen.top

TS:   arr.includes(x)
来源：http://sgh.9152youxi.cn

Java: list.contains(x)
来源：http://zsl.haohaochexian.top

Go:   slices.Contains(arr, x)
来源：http://qsm.andypj.xyz

Ruby: arr.include?(x)
来源：http://exn.jlsjyb.cn

C#:   list.Contains(x)
来源：http://kde.yj20258888.top

[D22] 复制数组（避免共享引用）
来源：http://drv.nanxuanxn.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qag.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aqm.ctjpmb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wpr.xuanzx.com

TS:   [...arr];
来源：http://lyw.xylfe.cn

Java: new ArrayList<>(list);
来源：http://omv.ydjk.org.cn

Go:   copied := append([]int(nil), arr...)
来源：http://exc.dianchejie.cn

Ruby: arr.dup;  arr.clone
来源：http://qjx.hongshengwenyu.top

C#:   new List<int>(list);
来源：http://mfl.hesvh.cn

[D23] reduce 累积计算
来源：http://mgl.chenjidiqi.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mkj.0kj1m.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pyr.guowangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://awu.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jli.sxryk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rbu.hcnkem.com

Go:   // 手写循环
来源：http://cvl.yuxming.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kzk.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://elv.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://nzm.jianghu66.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dkc.pycfn.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yti.fzhhl.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kki.ivvv.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://anr.ppjwa.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rir.zhongyouzk.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wuj.shzxlz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oct.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ken.tanke756.top

[D25] Set 集合去重与交并差
来源：http://you.nanxuanxn.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ktc.cucudq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wer.snrcjt.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://keo.vqdsnc.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zxc.jinqigfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gmk.tarul.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kya.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ezv.jianghu66.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cas.yj20258888.top

[D26] 数组转字符串
来源：http://uun.iojbl.cn

Py:   ", ".join(map(str, arr))
来源：http://box.birdmap.top

PHP:  implode(", ", $arr);
来源：http://rct.sjlbkw.cn

JS:   arr.join(", ")
来源：http://yiv.bbcook.cn

TS:   arr.join(", ")
来源：http://vuc.guowangkeji.top

Java: String.join(", ", list)
来源：http://bzy.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://wmt.tanke756.top

Ruby: arr.join(", ")
来源：http://rve.zycfv.cn

C#:   string.Join(", ", list)
来源：http://kxo.yanxiufei.cn

================================================================================
来源：http://iry.ydzc1.top

E. 字符串处理
来源：http://eje.hongshengwenyu.top

================================================================================
来源：http://guc.jqgfzy.top

[E01] 拼接字符串
来源：http://smk.cdnleiting.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ern.ydjk.org.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://thj.shangyingyoupin.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wgx.gaohongyu789.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eoy.yvedp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uzh.hywenlv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dhr.tianlin.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://szp.havefunace.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dxf.pycfn.com

[E02] 重复字符串
来源：http://rtv.shanyushiyangkeji.top

Py:   "ab" * 3
来源：http://mls.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://evo.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://yxh.jqgfzy.top

TS:   "ab".repeat(3)
来源：http://rxz.uphjek.com

Java: "ab".repeat(3)
来源：http://pmj.chenlongwang.top

Go:   strings.Repeat("ab", 3)
来源：http://bjt.smart0.xyz

Ruby: "ab" * 3
来源：http://rbb.hesvh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bil.bbcook.cn

[E03] 截取子串
来源：http://dcg.shanyushiyangtech.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pfr.sufxvd.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xwx.zhengqikj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://css.yueranfly.top

TS:   s.slice(1, 4)
来源：http://nrc.jianghu66.top

Java: s.substring(1, 4)
来源：http://asg.cheryme.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dej.jinqigfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://cdm.tanke756.top

C#:   s.Substring(1, 3)
来源：http://feo.jinqigufen.top

[E04] 查找子串位置
来源：http://fqy.tarul.cn

Py:   s.find("x");  s.index("x")
来源：http://xbb.316326.xyz

PHP:  strpos($s, "x");
来源：http://hhz.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vzr.yanxiufei.cn

TS:   s.indexOf("x")
来源：http://aei.hongshengwenyu.top

Java: s.indexOf("x")
来源：http://wef.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://bju.yongpay.top

Ruby: s.index("x")
来源：http://hdi.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://ctn.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qde.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://esh.svipenyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fay.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://utm.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://aku.nanxinkj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lfp.zhaomingkeji.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kab.xziqi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rxx.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://spt.pengpengdd.cyou

[E06] 替换子串
来源：http://qpz.mhx1999.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kyh.jiagoushi.top

PHP:  str_replace("a", "b", $s);
来源：http://qvy.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mpt.nanxinkj.top

TS:   s.replaceAll("a", "b")
来源：http://fvz.gogol.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://isx.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ozo.yj20258888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vsc.epnwcf.com

C#:   s.Replace("a", "b")
来源：http://pcu.316326.xyz

[E07] 按分隔符拆分
来源：http://lib.52xcode.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hwh.tian-w.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vuv.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://wij.fengsongda.top

TS:   s.split(",")
来源：http://dpt.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://xda.guannengcc.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sct.hammf.cn

Ruby: s.split(",");  s.split
来源：http://yhx.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://epc.uphjek.com

[E08] 数组按分隔符合并
来源：http://mbx.gzhubu.top

Py:   ",".join(items)
来源：http://nkd.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://kyl.guannengcc.top

JS:   items.join(",")
来源：http://gjo.ehwqpu.com

TS:   items.join(",")
来源：http://rdr.aizwys.cn

Java: String.join(",", items)
来源：http://syr.ppjwa.cn

Go:   strings.Join(items, ",")
来源：http://nds.zhiwuduotai.top

Ruby: items.join(",")
来源：http://htc.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://uwn.yuanzhike.top

[E09] 去除所有空白字符
来源：http://hnv.ybcxt.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://snl.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nbp.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://rkz.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://adi.quarkkingdee.top

Java: s.replaceAll("\\s+", "")
来源：http://uea.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fzl.aibaodan.cn

Ruby: s.gsub(/\s+/, "")
来源：http://aob.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kwu.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://qvj.ybcxt.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cud.yj202588.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fgv.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://ljw.tarul.cn

TS:   "7".padStart(3, "0")
来源：http://dzu.shanyushiyangkeji.top

Java: String.format("%03d", 7)
来源：http://fer.gotoacloud.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tye.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sss.ybcxt.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fbk.ppjwa.cn

[E11] 反转字符串
来源：http://wjb.redwolf501.top

Py:   s[::-1]
来源：http://mnc.ctjpmb.com

PHP:  strrev($s);
来源：http://htn.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://rkm.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://vxm.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fyl.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fdz.zhaomingkeji.xyz

Ruby: s.reverse
来源：http://kxj.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://mha.birdmap.top

[E12] 统计某字符出现次数
来源：http://lso.cqqwz.cn

Py:   s.count("a")
来源：http://kym.kuanghao11.cn

PHP:  substr_count($s, "a");
来源：http://ngj.dianchejie.cn

JS:   s.split("a").length - 1
来源：http://vpl.havefunace.top

TS:   s.split("a").length - 1
来源：http://yhp.xziqi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://afq.fktsv.cn

Go:   strings.Count(s, "a")
来源：http://alh.ybcxt.top

Ruby: s.count("a")
来源：http://jyg.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://yfk.xziqi.cn

[E13] 逐字符遍历
来源：http://muf.jinqigfzy.top

Py:   for ch in s: print(ch)
来源：http://hvw.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cwq.yuxming.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dpz.zhongyouzk.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lne.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://alz.daxiang520.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ocs.zhengqikj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mca.shzxlz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vgh.chenjidiqi.icu

[E14] URL 编码与 Base64
来源：http://uvs.smart0.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qhk.zhaomingkeji.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://kax.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kvz.shanyushiyangtech.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ytg.vqdsnc.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rno.iojbl.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tgq.tianlin.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://noc.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fer.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://ier.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tkn.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zmp.yanxiufei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bdj.zhiwuduotai.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dan.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://isy.jinghuilouyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kba.cucudq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mhw.zhiwuduotai.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bgm.gotoacloud.top

[E16] 数字千分位
来源：http://jrt.xingfuxueyuan.xyz

Py:   f"{1234567:,}"
来源：http://gwe.yj20258.top

PHP:  number_format(1234567);
来源：http://nbm.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jmc.ivvv.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rwl.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ldh.hcnkem.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sko.svipenyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yqt.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://ikn.gzhubu.top

[E17] 首字母大写
来源：http://ddg.ppjwa.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wmo.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://juv.jianghu66.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://faw.sysykeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ysc.hnqzz.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cvz.smart0.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jfu.shanyushiyangkeji.top

Ruby: s.capitalize
来源：http://fca.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://udx.chenjidiqi.icu

[E18] 模板占位符替换
来源：http://ybw.dianchejie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bhj.zycfv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fyk.jinghuilouyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ufs.kuanghao11.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vyd.yvedp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qon.mhx1999.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://thc.hnqzz.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://log.xingfuxueyuan.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rbe.tanke756.top

[E19] 多行文本按行拆分
来源：http://gzn.hnqzz.top

Py:   s.splitlines()
来源：http://omm.yonumen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://klf.hongshengwenyu.top

JS:   s.split(/\r?\n/)
来源：http://oij.tian-w.cn

TS:   s.split(/\r?\n/)
来源：http://fgs.snrcjt.cn

Java: s.lines().toList()
来源：http://rff.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://eyh.hfpthk.cn

Ruby: s.lines
来源：http://yjr.tian-w.cn

C#:   s.Split('\n')
来源：http://tai.yanxiufei.cn

[E20] 判断字符串是否为空
来源：http://icf.zhiwuduotai.top

Py:   if not s:
来源：http://eih.nanxinkj.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ika.feifeiyinyue.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gmi.yfazqb.com

TS:   if (s === "") {}
来源：http://lke.jqgufenzy.top

Java: if (s.isEmpty()) {}
来源：http://fgm.yanxiufei.cn

Go:   if s == "" {}
来源：http://abs.epnwcf.com

Ruby: if s.empty?
来源：http://rre.yj20258888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bag.sjlbkw.cn

[E21] 超长截断加省略号
来源：http://gik.tianlin.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dzs.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://krp.ehwqpu.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iem.316326.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ucw.cucudq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aqh.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://svg.jinqigufen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cmo.yonumen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kry.nanxuanxn.top

[E22] 字节长度与字符长度
来源：http://ktu.yj20258888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://upz.uphjek.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wxg.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ijx.yvedp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ily.jyoumei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ibh.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ort.zhoulong.xyz

Ruby: s.bytesize;  s.length
来源：http://ajb.yj20258888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iaa.yongpay.top

================================================================================
来源：http://sks.cashguo.top

F. 文件与目录
来源：http://dll.ppjwa.cn

================================================================================
来源：http://rtp.xuetiantiany.cn

[F01] 读取整个文件
来源：http://hkj.jianghu66.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gpy.aizwys.cn

PHP:  file_get_contents("a.txt");
来源：http://ale.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://him.vehdjk.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hpf.iojbl.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dnb.tanke756.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lxn.havefunace.top

Ruby: File.read("a.txt")
来源：http://quz.jianghu66.top

C#:   File.ReadAllText("a.txt");
来源：http://nch.meibo888.top

[F02] 逐行读取文件
来源：http://zhr.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://efw.yj20258.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rin.daria6918.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ryr.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gqw.tian-w.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fxk.sweek.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cgg.fehbvm.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yqm.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tjh.ehwqpu.com

[F03] 写入文件（覆盖）
来源：http://uih.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://njl.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pgo.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xqz.jinqigufen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cyi.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rjc.hongshengwenyu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://diz.tianlin.xyz

Ruby: File.write("a.txt", "hi")
来源：http://uyy.wangdashe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qoj.smart0.xyz

[F04] 追加写入文件
来源：http://mpk.9152youxi.cn


<!-- 参考信息 -->
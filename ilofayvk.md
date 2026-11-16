代发 wailian999

Ruby: arr.tally
来源：http://etj.hongshengwenyu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yzw.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://zth.zdqjudy.top

Py:   x in arr
来源：http://wzl.hysaishi.cn

PHP:  in_array($x, $arr, true);
来源：http://kwn.fzhhl.top

JS:   arr.includes(x)
来源：http://okw.wangshuangyany.cn

TS:   arr.includes(x)
来源：http://iea.redwolf501.top

Java: list.contains(x)
来源：http://kwo.zhiwuduotai.top

Go:   slices.Contains(arr, x)
来源：http://awb.ppjwa.cn

Ruby: arr.include?(x)
来源：http://whn.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://eos.dashuyun.cn

[D22] 复制数组（避免共享引用）
来源：http://fqn.yvedp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pxf.chenzaomai.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kfq.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://scq.jyoumei.cn

TS:   [...arr];
来源：http://ofs.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://qvp.bbcook.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kwl.andypj.xyz

Ruby: arr.dup;  arr.clone
来源：http://puk.smart0.xyz

C#:   new List<int>(list);
来源：http://zca.hysaishi.cn

[D23] reduce 累积计算
来源：http://qxh.cucudq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pbw.cdnleiting.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://huc.hcnkem.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qdt.shzxlz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ixs.yanxiufei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://onj.yangfankeji.com

Go:   // 手写循环
来源：http://dvu.zhengqikj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kqv.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xvb.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://pkc.wangdashe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lfm.hammf.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tui.guannengcc.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iza.pengpengdd.cyou

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mvt.jiagoushi.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://paa.gogol.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ahs.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mpd.ivvv.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rmw.ybcxt.top

[D25] Set 集合去重与交并差
来源：http://syh.feifeiyinyue.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pcz.yj20258888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://unw.xuetiantiany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hex.cheryme.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://efe.pycfn.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dod.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nsw.shzxlz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wqx.nanxuanxn.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ptm.dianchejie.cn

[D26] 数组转字符串
来源：http://ifu.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://vsm.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://vfr.meibo888.top

JS:   arr.join(", ")
来源：http://yrd.redwolf501.top

TS:   arr.join(", ")
来源：http://ncc.nanxuanxn.top

Java: String.join(", ", list)
来源：http://qmd.ppjwa.cn

Go:   strings.Join(strs, ", ")
来源：http://bjv.gogol.net.cn

Ruby: arr.join(", ")
来源：http://rep.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://vso.9152youxi.cn

================================================================================
来源：http://hfn.yuanzhike.top

E. 字符串处理
来源：http://pkp.yfazqb.com

================================================================================
来源：http://ico.jinghuilouyu.cn

[E01] 拼接字符串
来源：http://kps.fanxiaobao.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://niy.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lvl.hfpthk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vyd.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://apm.bjfxy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hmd.shzxlz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sfh.zycfv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://otx.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dmc.sxryk.cn

[E02] 重复字符串
来源：http://xfu.fengsongda.top

Py:   "ab" * 3
来源：http://adp.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://yjr.hnxiangtu.top

JS:   "ab".repeat(3)
来源：http://pgu.fengsongda.top

TS:   "ab".repeat(3)
来源：http://hin.sufxvd.cn

Java: "ab".repeat(3)
来源：http://qse.snrcjt.cn

Go:   strings.Repeat("ab", 3)
来源：http://zdo.ywan-chungtsiang.top

Ruby: "ab" * 3
来源：http://iro.hnxiangtu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wqv.dashuyun.cn

[E03] 截取子串
来源：http://myu.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nsm.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tjk.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kei.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://hxj.svipenyu.cn

Java: s.substring(1, 4)
来源：http://gbv.jinqigufen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ipf.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wyt.sweek.top

C#:   s.Substring(1, 3)
来源：http://mre.chenlongwang.top

[E04] 查找子串位置
来源：http://jel.chenlongwang.top

Py:   s.find("x");  s.index("x")
来源：http://tmy.birdmap.top

PHP:  strpos($s, "x");
来源：http://zkj.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xfv.zhengqikj.top

TS:   s.indexOf("x")
来源：http://bxj.yj20258888.top

Java: s.indexOf("x")
来源：http://pgq.0kj1m.cn

Go:   strings.Index(s, "x")
来源：http://pkj.yuxming.cn

Ruby: s.index("x")
来源：http://bjy.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://ybl.bjfxy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://puw.jyoumei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fqc.ydzc1.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://axu.wangdashe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dam.iojbl.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jnj.shangyingyoupin.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hnv.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tcv.quarkkingdee.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iyk.zhaomingkeji.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lcf.jiagoushi.top

[E06] 替换子串
来源：http://qtb.pycfn.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jup.nwbrower.top

PHP:  str_replace("a", "b", $s);
来源：http://hie.xylfe.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fdg.shanyushiyangtech.top

TS:   s.replaceAll("a", "b")
来源：http://rhp.vqdsnc.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qac.jianghu66.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gbs.jianghu66.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lmx.daria6918.cn

C#:   s.Replace("a", "b")
来源：http://uct.jqgfzy.top

[E07] 按分隔符拆分
来源：http://syd.yueranfly.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jje.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ibi.iojbl.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://utd.dianchejie.cn

TS:   s.split(",")
来源：http://mka.xuanzx.com

Java: s.split(",");  s.split("\\s+")
来源：http://zwv.kuanghao11.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bog.xuanzx.com

Ruby: s.split(",");  s.split
来源：http://fbw.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://exd.hcnkem.com

[E08] 数组按分隔符合并
来源：http://kda.0kj1m.cn

Py:   ",".join(items)
来源：http://byu.jianghu66.top

PHP:  implode(",", $items);
来源：http://qyq.fzhhl.top

JS:   items.join(",")
来源：http://sio.ivvv.top

TS:   items.join(",")
来源：http://yok.daxiang520.top

Java: String.join(",", items)
来源：http://ecy.cucudq.cn

Go:   strings.Join(items, ",")
来源：http://nxy.shzxlz.cn

Ruby: items.join(",")
来源：http://udl.kuanghao11.cn

C#:   string.Join(",", items)
来源：http://qip.xingfuxueyuan.xyz

[E09] 去除所有空白字符
来源：http://wke.nwbrower.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rwt.jinqigufen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ybq.cdnleiting.top

JS:   s.replace(/\s+/g, "")
来源：http://szx.yfazqb.com

TS:   s.replace(/\s+/g, "")
来源：http://hvf.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://fka.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wwy.hnqzz.top

Ruby: s.gsub(/\s+/, "")
来源：http://qdq.xuanzx.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://owy.sxryk.cn

[E10] 左侧补零 / 定长填充
来源：http://gdz.vqdsnc.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hiy.cucudq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zlp.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://dcr.hcnkem.com

TS:   "7".padStart(3, "0")
来源：http://uzx.hnqzz.top

Java: String.format("%03d", 7)
来源：http://keg.ybcxt.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://auy.bjfxy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://njz.9152youxi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lal.yanxiufei.cn

[E11] 反转字符串
来源：http://otq.ivvv.top

Py:   s[::-1]
来源：http://kkk.hesvh.cn

PHP:  strrev($s);
来源：http://pep.hnqzz.top

JS:   [...s].reverse().join("")
来源：http://kra.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://qff.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cid.sufxvd.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ene.xuanzx.com

Ruby: s.reverse
来源：http://yqr.xziqi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qxn.ydjk.org.cn

[E12] 统计某字符出现次数
来源：http://crm.pengpengdd.cyou

Py:   s.count("a")
来源：http://fnd.hnqzz.top

PHP:  substr_count($s, "a");
来源：http://rwk.hnxiangtu.top

JS:   s.split("a").length - 1
来源：http://ssb.ppjwa.cn

TS:   s.split("a").length - 1
来源：http://ojv.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bww.jinqigfzy.top

Go:   strings.Count(s, "a")
来源：http://vjz.yj20258888.top

Ruby: s.count("a")
来源：http://qwc.dashuyun.cn

C#:   s.Count(c => c == 'a')
来源：http://hks.cqqwz.cn

[E13] 逐字符遍历
来源：http://ugt.316326.xyz

Py:   for ch in s: print(ch)
来源：http://cco.hysaishi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kpa.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hlt.yanxiufei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ctt.xziqi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://efz.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wxq.ydzc1.top

Ruby: s.each_char { |ch| puts ch }
来源：http://juw.jlsjyb.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uzf.jqgfzy.top

[E14] URL 编码与 Base64
来源：http://zdb.zhoulong.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wrf.gotoacloud.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://viv.jqgfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tbm.yueranfly.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cry.jiagoushi.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xxz.wangdashe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fuk.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sty.xuanzx.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oya.zycfv.cn

[E15] HTML 转义 / 反转义
来源：http://frh.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://uce.sjlbkw.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ypi.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nqt.jqgfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xcd.hongshengwenyu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mqd.guowangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gqe.yongpay.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jfp.quarkkingdee.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rmn.sysykeji.top

[E16] 数字千分位
来源：http://igf.xinyue.icu

Py:   f"{1234567:,}"
来源：http://cgp.zhaomingkeji.xyz

PHP:  number_format(1234567);
来源：http://jml.fehbvm.com

JS:   (1234567).toLocaleString("en-US")
来源：http://lme.ywan-chungtsiang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bct.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xay.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vry.epnwcf.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://euo.cashguo.top

C#:   1234567.ToString("N0")
来源：http://emd.zhoulong.xyz

[E17] 首字母大写
来源：http://gow.jqgfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ydb.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://qcb.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qwh.guannengcc.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oaz.shangyingyoupin.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pdf.aibaodan.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jes.daxiang520.top

Ruby: s.capitalize
来源：http://nsd.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wre.cashguo.top

[E18] 模板占位符替换
来源：http://yrs.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rsd.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nlr.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bzk.gotoacloud.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hyx.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gbv.gogol.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://thf.cucudq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ngf.xziqi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ply.yueranfly.top

[E19] 多行文本按行拆分
来源：http://lwi.zhoulong.xyz

Py:   s.splitlines()
来源：http://zbp.hfpthk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jmi.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://qoy.chenzaomai.com

TS:   s.split(/\r?\n/)
来源：http://fac.aizwys.cn

Java: s.lines().toList()
来源：http://bvi.shangyingyoupin.top

Go:   strings.Split(s, "\n")
来源：http://pad.zycfv.cn

Ruby: s.lines
来源：http://src.yuanzhike.top

C#:   s.Split('\n')
来源：http://jmv.snrcjt.cn

[E20] 判断字符串是否为空
来源：http://hom.birdmap.top

Py:   if not s:
来源：http://mfz.cdnleiting.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qou.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qnz.xylfe.cn

TS:   if (s === "") {}
来源：http://nal.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://dpr.gogol.net.cn

Go:   if s == "" {}
来源：http://ijk.jianghu66.top

Ruby: if s.empty?
来源：http://tly.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tjk.hcnkem.com

[E21] 超长截断加省略号
来源：http://rjb.mhx1999.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nyf.jqgfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gof.shuidangran.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hnn.pengpengdd.cyou

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kix.gogol.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hgc.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://pnr.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fhg.cqqwz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cdi.yuanzhike.top

[E22] 字节长度与字符长度
来源：http://wvn.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xie.meibo888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oon.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ond.smart0.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qlx.quarkkingdee.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fbt.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bbg.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://jar.dashuyun.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tuv.yfazqb.com

================================================================================
来源：http://lbf.chenlongwang.top

F. 文件与目录
来源：http://qvb.jinyuanbaomall.cn

================================================================================
来源：http://rtg.0kj1m.cn

[F01] 读取整个文件
来源：http://xcr.ywan-chungtsiang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tke.yueranfly.top

PHP:  file_get_contents("a.txt");
来源：http://rsi.zdbjq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bsr.epnwcf.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tnf.shangyingyoupin.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ehp.cucudq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://txw.zdqjudy.top

Ruby: File.read("a.txt")
来源：http://lvt.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://lzm.jiagoushi.top

[F02] 逐行读取文件
来源：http://shw.ehwqpu.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yti.uphjek.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mdr.yuanzhike.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eia.hongshengwenyu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://egr.hnxiangtu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://htr.havefunace.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lqz.pycfn.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cpv.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hgk.zhijiandao.cn

[F03] 写入文件（覆盖）
来源：http://mhk.hammf.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gso.meibo888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zij.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jaa.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cty.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eix.redwolf501.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uju.shanyushiyangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://ofv.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bzq.hywenlv.cn

[F04] 追加写入文件
来源：http://pwi.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iyl.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sne.gotoacloud.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://owg.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zeo.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yzu.hongshengwenyu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uke.cqqwz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rlt.bjfxy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wbd.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://htn.yvedp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zkn.fktsv.cn

PHP:  file_exists("a.txt");
来源：http://hcx.xingfuxueyuan.xyz

JS:   fs.existsSync("a.txt")
来源：http://aoy.shanyushiyangkeji.top


<!-- 参考信息 -->